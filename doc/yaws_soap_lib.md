

# Module yaws_soap_lib #
* [Function Index](#index)
* [Function Details](#functions)


<a name="index"></a>

## Function Index ##


<table width="100%" border="1" cellspacing="0" cellpadding="2" summary="function index"><tr><td valign="top"><a href="#call-3">call/3</a></td><td></td></tr><tr><td valign="top"><a href="#call-4">call/4</a></td><td></td></tr><tr><td valign="top"><a href="#call-5">call/5</a></td><td></td></tr><tr><td valign="top"><a href="#call-6">call/6</a></td><td></td></tr><tr><td valign="top"><a href="#call_attach-4">call_attach/4</a></td><td></td></tr><tr><td valign="top"><a href="#call_attach-5">call_attach/5</a></td><td></td></tr><tr><td valign="top"><a href="#call_attach-7">call_attach/7</a></td><td></td></tr><tr><td valign="top"><a href="#config_file_xsd-0">config_file_xsd/0</a></td><td></td></tr><tr><td valign="top"><a href="#findHeader-2">findHeader/2</a></td><td></td></tr><tr><td valign="top"><a href="#get_operation-2">get_operation/2</a></td><td></td></tr><tr><td valign="top"><a href="#initModel-1">initModel/1</a></td><td></td></tr><tr><td valign="top"><a href="#initModel-2">initModel/2</a></td><td></td></tr><tr><td valign="top"><a href="#initModelFile-1">initModelFile/1</a></td><td></td></tr><tr><td valign="top"><a href="#is_wsdl-1">is_wsdl/1</a></td><td></td></tr><tr><td valign="top"><a href="#makeFault-2">makeFault/2</a></td><td></td></tr><tr><td valign="top"><a href="#parseMessage-2">parseMessage/2</a></td><td></td></tr><tr><td valign="top"><a href="#qtest-0">qtest/0</a></td><td></td></tr><tr><td valign="top"><a href="#write_hrl-2">write_hrl/2</a></td><td></td></tr><tr><td valign="top"><a href="#write_hrl-3">write_hrl/3</a></td><td></td></tr><tr><td valign="top"><a href="#wsdl_model-1">wsdl_model/1</a></td><td></td></tr><tr><td valign="top"><a href="#wsdl_op_action-1">wsdl_op_action/1</a></td><td></td></tr><tr><td valign="top"><a href="#wsdl_op_address-1">wsdl_op_address/1</a></td><td></td></tr><tr><td valign="top"><a href="#wsdl_op_binding-1">wsdl_op_binding/1</a></td><td></td></tr><tr><td valign="top"><a href="#wsdl_op_operation-1">wsdl_op_operation/1</a></td><td></td></tr><tr><td valign="top"><a href="#wsdl_op_port-1">wsdl_op_port/1</a></td><td></td></tr><tr><td valign="top"><a href="#wsdl_op_service-1">wsdl_op_service/1</a></td><td></td></tr><tr><td valign="top"><a href="#wsdl_operations-1">wsdl_operations/1</a></td><td></td></tr></table>


<a name="functions"></a>

## Function Details ##

<a name="call-3"></a>

### call/3 ###

`call(WsdlURL, Operation, ListOfData) -> any()`


<a name="call-4"></a>

### call/4 ###

`call(WsdlURL, Operation, Header, Msg) -> any()`


<a name="call-5"></a>

### call/5 ###

`call(WsdlURL, Operation, ListOfData, X4, Prefix) -> any()`


<a name="call-6"></a>

### call/6 ###

`call(Wsdl, Operation, Port, Service, Headers, Message) -> any()`


<a name="call_attach-4"></a>

### call_attach/4 ###

`call_attach(WsdlURL, Operation, ListOfData, Attachments) -> any()`


<a name="call_attach-5"></a>

### call_attach/5 ###

`call_attach(WsdlURL, Operation, Header, Msg, Attachments) -> any()`


<a name="call_attach-7"></a>

### call_attach/7 ###

`call_attach(Wsdl, Operation, Port, Service, Headers, Message, Attachments) -> any()`


<a name="config_file_xsd-0"></a>

### config_file_xsd/0 ###

`config_file_xsd() -> any()`


<a name="findHeader-2"></a>

### findHeader/2 ###

`findHeader(Label, Headers) -> any()`


<a name="get_operation-2"></a>

### get_operation/2 ###

`get_operation(T, X) -> any()`


<a name="initModel-1"></a>

### initModel/1 ###

`initModel(WsdlFile) -> any()`


<a name="initModel-2"></a>

### initModel/2 ###

`initModel(WsdlFile, PrefixOrOptions) -> any()`


<a name="initModelFile-1"></a>

### initModelFile/1 ###

`initModelFile(ConfigFile) -> any()`


<a name="is_wsdl-1"></a>

### is_wsdl/1 ###

`is_wsdl(Wsdl) -> any()`


<a name="makeFault-2"></a>

### makeFault/2 ###

`makeFault(FaultCode, FaultString) -> any()`


<a name="parseMessage-2"></a>

### parseMessage/2 ###

`parseMessage(Message, Wsdl) -> any()`


<a name="qtest-0"></a>

### qtest/0 ###

`qtest() -> any()`


<a name="write_hrl-2"></a>

### write_hrl/2 ###

`write_hrl(WsdlURL, Output) -> any()`


<a name="write_hrl-3"></a>

### write_hrl/3 ###

`write_hrl(WsdlURL, Output, PrefixOrOptions) -> any()`


<a name="wsdl_model-1"></a>

### wsdl_model/1 ###

`wsdl_model(Wsdl) -> any()`


<a name="wsdl_op_action-1"></a>

### wsdl_op_action/1 ###

`wsdl_op_action(Operation) -> any()`


<a name="wsdl_op_address-1"></a>

### wsdl_op_address/1 ###

`wsdl_op_address(Operation) -> any()`


<a name="wsdl_op_binding-1"></a>

### wsdl_op_binding/1 ###

`wsdl_op_binding(Operation) -> any()`


<a name="wsdl_op_operation-1"></a>

### wsdl_op_operation/1 ###

`wsdl_op_operation(Operation) -> any()`


<a name="wsdl_op_port-1"></a>

### wsdl_op_port/1 ###

`wsdl_op_port(Operation) -> any()`


<a name="wsdl_op_service-1"></a>

### wsdl_op_service/1 ###

`wsdl_op_service(Operation) -> any()`


<a name="wsdl_operations-1"></a>

### wsdl_operations/1 ###

`wsdl_operations(Wsdl) -> any()`


