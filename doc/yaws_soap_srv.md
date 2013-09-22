

# Module yaws_soap_srv #
* [Function Index](#index)
* [Function Details](#functions)

__Behaviours:__ [`gen_server`](gen_server.md).
<a name="index"></a>

## Function Index ##


<table width="100%" border="1" cellspacing="0" cellpadding="2" summary="function index"><tr><td valign="top"><a href="#code_change-3">code_change/3</a></td><td></td></tr><tr><td valign="top"><a href="#handle_call-3">handle_call/3</a></td><td></td></tr><tr><td valign="top"><a href="#handle_cast-2">handle_cast/2</a></td><td></td></tr><tr><td valign="top"><a href="#handle_info-2">handle_info/2</a></td><td></td></tr><tr><td valign="top"><a href="#handler-4">handler/4</a></td><td></td></tr><tr><td valign="top"><a href="#init-1">init/1</a></td><td></td></tr><tr><td valign="top"><a href="#setup-1">setup/1</a></td><td></td></tr><tr><td valign="top"><a href="#setup-2">setup/2</a></td><td></td></tr><tr><td valign="top"><a href="#setup-3">setup/3</a></td><td></td></tr><tr><td valign="top"><a href="#start_link-0">start_link/0</a></td><td></td></tr><tr><td valign="top"><a href="#start_link-1">start_link/1</a></td><td></td></tr><tr><td valign="top"><a href="#terminate-2">terminate/2</a></td><td></td></tr></table>


<a name="functions"></a>

## Function Details ##

<a name="code_change-3"></a>

### code_change/3 ###

`code_change(OldVsn, State, Extra) -> any()`


<a name="handle_call-3"></a>

### handle_call/3 ###

`handle_call(X1, From, State) -> any()`


<a name="handle_cast-2"></a>

### handle_cast/2 ###

`handle_cast(Msg, State) -> any()`


<a name="handle_info-2"></a>

### handle_info/2 ###

`handle_info(Info, State) -> any()`


<a name="handler-4"></a>

### handler/4 ###

`handler(Args, Id, Payload, SessionValue) -> any()`


<a name="init-1"></a>

### init/1 ###

`init(L) -> any()`


<a name="setup-1"></a>

### setup/1 ###

`setup(ConfigFile) -> any()`


<a name="setup-2"></a>

### setup/2 ###

`setup(Id, WsdlFile) -> any()`


<a name="setup-3"></a>

### setup/3 ###

`setup(Id, WsdlFile, PrefixOrOptions) -> any()`


<a name="start_link-0"></a>

### start_link/0 ###

`start_link() -> any()`


<a name="start_link-1"></a>

### start_link/1 ###

`start_link(L) -> any()`


<a name="terminate-2"></a>

### terminate/2 ###

`terminate(Reason, State) -> any()`


