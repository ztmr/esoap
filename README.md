# SOAP library for Erlang
## Client HOWTO
### Dependencies
Add `ibrowse` as your project's dependency.
Esoap uses inets as a fallback if the `ibrowse` is not available, but `ibrowse` is much better for multiple reasons.

### Prepare record definitions
```Erlang
M = yaws_soap_lib:initModel ("http://xyz.com/foo.wsdl"), % or /tmp/foo.wsdl
yaws_soap_lib:write_hrl (M, "include/foo_web_service.hrl").
```

### Implement client proxy module
```Erlang
-module (foo_client).
-export ([call_echo/0]).
-include ("foo_web_service.hrl").

%% Of course, this is not necessary: you should know
%% whether you have ibrowse added in your rebar deps!
ensure_deps_started () ->
    % ibrowse is better, fallback is inets
    case code:ensure_loaded (ibrowse) of
        {module, ibrowse} -> {ok, _} = ibrowse:start ();
        {error, _}        -> ok = inets:start ()
    end.

call_echo () ->
    ensure_deps_started (),
    M = yaws_soap_lib:initModel ("/tmp/foo.wsdl"), % can be http(s) too
    case yaws_soap_lib:call (M, "EchoMethod", ["Hello", "World"]) of
        %% #'Nsp:EchoResponse' record is defined in the included .hrl
        {ok, _, #'Nsp:EchoResponse' { 'EchoResultValue' = X }} ->
            {ok, X};
        Error ->
            {error, Error}
    end.
```

### Recommendations
- performance: parse .wsdl once and cache the model for future use (you can use `ets` cache or simply make a simple `gen_server` with internal state holding the WSDL model)

## Server HOWTO
Server is not supported yet. YAWS implements it but we haven't made it working standalone since we don't need it at the moment.

# Resources
- http://hyber.org/soap_intro.yaws
