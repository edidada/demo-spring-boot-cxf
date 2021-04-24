# README

wsdl4j jar包

- javax.jws.WebMethod;
- javax.jws.WebParam;
- javax.jws.WebResult;
- javax.jws.WebService;

[spring boot整合cxf发布webservice服务和cxf客户端调用](https://blog.csdn.net/pharaohsprince/article/details/75579630)

soap形式部署的http接口
Dubbo是一样的

```shell script
15:45:43.603 [main] DEBUG org.apache.cxf.common.logging.LogUtils - Using org.apache.cxf.common.logging.Slf4jLogger for logging.
15:45:43.791 [main] INFO org.apache.cxf.wsdl.service.factory.ReflectionServiceFactoryBean - Creating Service {http://webservice.leftso.com/}CommonServiceService from class com.leftso.webservice.CommonService
15:45:44.006 [main] DEBUG org.apache.cxf.jaxb.JAXBDataBinding - Created JAXBContext "jar:file:/Users/ibqo/.m2/repository/com/sun/xml/bind/jaxb-impl/2.2.11/jaxb-impl-2.2.11.jar!/com/sun/xml/bind/v2/runtime/JAXBContextImpl.class Build-Id: 2.2.11
Classes known to this context:
  [B
  boolean
  byte
  char
  com.leftso.webservice.jaxws_asm.SayHello
  com.leftso.webservice.jaxws_asm.SayHelloResponse
  com.sun.xml.bind.api.CompositeStructure
  double
  float
  int
  java.awt.Image
  java.io.File
  java.lang.Boolean
  java.lang.Byte
  java.lang.Character
  java.lang.Class
  java.lang.Double
  java.lang.Float
  java.lang.Integer
  java.lang.Long
  java.lang.Object
  java.lang.Short
  java.lang.String
  java.lang.Void
  java.math.BigDecimal
  java.math.BigInteger
  java.net.URI
  java.net.URL
  java.util.Calendar
  java.util.Date
  java.util.GregorianCalendar
  java.util.UUID
  javax.activation.DataHandler
  javax.xml.bind.JAXBElement
  javax.xml.datatype.Duration
  javax.xml.datatype.XMLGregorianCalendar
  javax.xml.namespace.QName
  javax.xml.transform.Source
  long
  short
  void
" with classes [class com.leftso.webservice.jaxws_asm.SayHello, class com.leftso.webservice.jaxws_asm.SayHelloResponse].
15:45:44.148 [main] DEBUG org.apache.cxf.resource.DefaultResourceManager - resolving resource <org.apache.cxf.wsdl11.WSDLManagerImpl/bus> type <interface org.apache.cxf.Bus>
15:45:44.149 [main] DEBUG org.apache.cxf.resource.DefaultResourceManager - resolving resource <null> type <interface org.apache.cxf.Bus>
15:45:44.307 [main] DEBUG org.apache.cxf.jaxws.handler.AnnotationHandlerChainBuilder - building handler chain
15:45:44.307 [main] DEBUG org.apache.cxf.jaxws.handler.AnnotationHandlerChainBuilder - Checking for HandlerChain annotation on com.leftso.webservice.CommonService
15:45:44.307 [main] DEBUG org.apache.cxf.jaxws.handler.AnnotationHandlerChainBuilder - no HandlerChain annotation on interface com.leftso.webservice.CommonService
15:45:44.314 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Invoke, operation info: [BindingOperationInfo: {http://webservice.leftso.com/}sayHello], params: [Leftso]
15:45:44.315 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - set requestContext to message be{org.apache.cxf.jaxws.context.WrappedMessageContext.SCOPES={org.apache.cxf.message.Message.ENDPOINT_ADDRESS=APPLICATION}, org.apache.cxf.message.Message.ENDPOINT_ADDRESS=http://localhost:8080/services/CommonService?wsdl, java.lang.reflect.Method=public abstract java.lang.String com.leftso.webservice.CommonService.sayHello(java.lang.String)}
15:45:44.318 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by bus: [org.apache.cxf.ws.policy.PolicyOutInterceptor@942a29c]
15:45:44.318 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by client: []
15:45:44.318 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by endpoint: [org.apache.cxf.interceptor.MessageSenderInterceptor@1ed6388a, org.apache.cxf.jaxws.interceptors.SwAOutInterceptor@5a45133e, org.apache.cxf.jaxws.interceptors.WrapperClassOutInterceptor@534a5a98, org.apache.cxf.jaxws.interceptors.HolderOutInterceptor@4f80542f]
15:45:44.318 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by binding: [org.apache.cxf.interceptor.AttachmentOutInterceptor@60bd273d, org.apache.cxf.interceptor.StaxOutInterceptor@121314f7, org.apache.cxf.binding.soap.interceptor.SoapHeaderOutFilterInterceptor@130c12b7, org.apache.cxf.wsdl.interceptors.WrappedOutInterceptor@5e600dd5, org.apache.cxf.wsdl.interceptors.BareOutInterceptor@576d5deb, org.apache.cxf.binding.soap.interceptor.SoapPreProtocolOutInterceptor@5d534f5d, org.apache.cxf.binding.soap.interceptor.SoapOutInterceptor@2e3967ea]
15:45:44.318 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by databinding: []
15:45:44.325 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.ws.policy.PolicyOutInterceptor@942a29c to phase setup
15:45:44.325 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.interceptor.MessageSenderInterceptor@1ed6388a to phase prepare-send
15:45:44.325 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.jaxws.interceptors.SwAOutInterceptor@5a45133e to phase pre-logical
15:45:44.325 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.jaxws.interceptors.WrapperClassOutInterceptor@534a5a98 to phase pre-logical
15:45:44.325 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.jaxws.interceptors.HolderOutInterceptor@4f80542f to phase pre-logical
15:45:44.325 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.interceptor.AttachmentOutInterceptor@60bd273d to phase pre-stream
15:45:44.325 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.interceptor.StaxOutInterceptor@121314f7 to phase pre-stream
15:45:44.325 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.SoapHeaderOutFilterInterceptor@130c12b7 to phase pre-logical
15:45:44.326 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.wsdl.interceptors.WrappedOutInterceptor@5e600dd5 to phase marshal
15:45:44.326 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.wsdl.interceptors.BareOutInterceptor@576d5deb to phase marshal
15:45:44.326 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.SoapPreProtocolOutInterceptor@5d534f5d to phase post-logical
15:45:44.326 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.SoapOutInterceptor@2e3967ea to phase write
15:45:44.367 [main] DEBUG org.apache.cxf.transport.http.HTTPConduit - Conduit '{http://webservice.leftso.com/}CommonServicePort.http-conduit' has been (re)configured for plain http.
15:45:44.367 [main] DEBUG org.apache.cxf.transport.http.HTTPConduit - No Trust Decider configured for Conduit '{http://webservice.leftso.com/}CommonServicePort.http-conduit'
15:45:44.367 [main] DEBUG org.apache.cxf.transport.http.HTTPConduit - No Auth Supplier configured for Conduit '{http://webservice.leftso.com/}CommonServicePort.http-conduit'
15:45:44.370 [main] DEBUG org.apache.cxf.transport.http.HTTPConduit - Conduit '{http://webservice.leftso.com/}CommonServicePort.http-conduit' has been configured for plain http.
15:45:44.371 [main] DEBUG org.apache.cxf.transport.http.HTTPConduit - registering incoming observer: org.apache.cxf.endpoint.ClientImpl@742ff096
15:45:44.371 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Chain org.apache.cxf.phase.PhaseInterceptorChain@1c5920df was created. Current flow:
  setup [PolicyOutInterceptor]
  pre-logical [HolderOutInterceptor, SwAOutInterceptor, WrapperClassOutInterceptor, SoapHeaderOutFilterInterceptor]
  post-logical [SoapPreProtocolOutInterceptor]
  prepare-send [MessageSenderInterceptor]
  pre-stream [AttachmentOutInterceptor, StaxOutInterceptor]
  write [SoapOutInterceptor]
  marshal [WrappedOutInterceptor, BareOutInterceptor]

15:45:44.372 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.ws.policy.PolicyOutInterceptor@942a29c
15:45:44.374 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.jaxws.interceptors.HolderOutInterceptor@4f80542f
15:45:44.374 [main] DEBUG org.apache.cxf.jaxws.interceptors.HolderOutInterceptor - op: [OperationInfo: {http://webservice.leftso.com/}sayHello]
15:45:44.374 [main] DEBUG org.apache.cxf.jaxws.interceptors.HolderOutInterceptor - op.hasOutput(): true
15:45:44.374 [main] DEBUG org.apache.cxf.jaxws.interceptors.HolderOutInterceptor - op.getOutput().size(): 1
15:45:44.374 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.jaxws.interceptors.SwAOutInterceptor@5a45133e
15:45:44.375 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.jaxws.interceptors.WrapperClassOutInterceptor@534a5a98
15:45:44.381 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.SoapHeaderOutFilterInterceptor@130c12b7
15:45:44.382 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.SoapPreProtocolOutInterceptor@5d534f5d
15:45:44.382 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.interceptor.MessageSenderInterceptor@1ed6388a
15:45:44.447 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.interceptor.MessageSenderInterceptor$MessageSenderEndingInterceptor@5f8e8a9d to phase prepare-send-ending
15:45:44.447 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Chain org.apache.cxf.phase.PhaseInterceptorChain@1c5920df was modified. Current flow:
  setup [PolicyOutInterceptor]
  pre-logical [HolderOutInterceptor, SwAOutInterceptor, WrapperClassOutInterceptor, SoapHeaderOutFilterInterceptor]
  post-logical [SoapPreProtocolOutInterceptor]
  prepare-send [MessageSenderInterceptor]
  pre-stream [AttachmentOutInterceptor, StaxOutInterceptor]
  write [SoapOutInterceptor]
  marshal [WrappedOutInterceptor, BareOutInterceptor]
  prepare-send-ending [MessageSenderEndingInterceptor]

15:45:44.447 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.interceptor.AttachmentOutInterceptor@60bd273d
15:45:44.454 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.interceptor.StaxOutInterceptor@121314f7
15:45:44.490 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.interceptor.StaxOutEndingInterceptor@64b0598 to phase pre-stream-ending
15:45:44.490 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Chain org.apache.cxf.phase.PhaseInterceptorChain@1c5920df was modified. Current flow:
  setup [PolicyOutInterceptor]
  pre-logical [HolderOutInterceptor, SwAOutInterceptor, WrapperClassOutInterceptor, SoapHeaderOutFilterInterceptor]
  post-logical [SoapPreProtocolOutInterceptor]
  prepare-send [MessageSenderInterceptor]
  pre-stream [AttachmentOutInterceptor, StaxOutInterceptor]
  write [SoapOutInterceptor]
  marshal [WrappedOutInterceptor, BareOutInterceptor]
  pre-stream-ending [StaxOutEndingInterceptor]
  prepare-send-ending [MessageSenderEndingInterceptor]

15:45:44.490 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.SoapOutInterceptor@2e3967ea
15:45:44.491 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.SoapOutInterceptor$SoapOutEndingInterceptor@28194a50 to phase write-ending
15:45:44.492 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Chain org.apache.cxf.phase.PhaseInterceptorChain@1c5920df was modified. Current flow:
  setup [PolicyOutInterceptor]
  pre-logical [HolderOutInterceptor, SwAOutInterceptor, WrapperClassOutInterceptor, SoapHeaderOutFilterInterceptor]
  post-logical [SoapPreProtocolOutInterceptor]
  prepare-send [MessageSenderInterceptor]
  pre-stream [AttachmentOutInterceptor, StaxOutInterceptor]
  write [SoapOutInterceptor]
  marshal [WrappedOutInterceptor, BareOutInterceptor]
  write-ending [SoapOutEndingInterceptor]
  pre-stream-ending [StaxOutEndingInterceptor]
  prepare-send-ending [MessageSenderEndingInterceptor]

15:45:44.492 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.wsdl.interceptors.WrappedOutInterceptor@5e600dd5
15:45:44.492 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.wsdl.interceptors.BareOutInterceptor@576d5deb
15:45:44.505 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.SoapOutInterceptor$SoapOutEndingInterceptor@28194a50
15:45:44.506 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.interceptor.StaxOutEndingInterceptor@64b0598
15:45:44.506 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.interceptor.MessageSenderInterceptor$MessageSenderEndingInterceptor@5f8e8a9d
15:45:44.506 [main] DEBUG org.apache.cxf.transport.http.Headers - Accept: */*
15:45:44.506 [main] DEBUG org.apache.cxf.transport.http.Headers - SOAPAction: ""
15:45:44.507 [main] DEBUG org.apache.cxf.transport.http.HTTPConduit - No Trust Decider for Conduit '{http://webservice.leftso.com/}CommonServicePort.http-conduit'. An affirmative Trust Decision is assumed.
15:45:44.513 [main] DEBUG org.apache.cxf.transport.http.HTTPConduit - Sending POST Message with Headers to http://localhost:8080/services/CommonService?wsdl Conduit :{http://webservice.leftso.com/}CommonServicePort.http-conduit

15:45:44.716 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by bus: [org.apache.cxf.ws.policy.PolicyInInterceptor@536dbea0]
15:45:44.716 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by client: []
15:45:44.716 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by endpoint: [org.apache.cxf.jaxws.interceptors.WrapperClassInInterceptor@47c81abf, org.apache.cxf.jaxws.interceptors.HolderInInterceptor@776a6d9b, org.apache.cxf.jaxws.interceptors.SwAInInterceptor@21d03963, org.apache.cxf.frontend.WSDLGetInterceptor@1f760b47]
15:45:44.716 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by binding: [org.apache.cxf.interceptor.AttachmentInInterceptor@18ece7f4, org.apache.cxf.interceptor.StaxInInterceptor@3cce57c7, org.apache.cxf.binding.soap.interceptor.SoapActionInInterceptor@1cf56a1c, org.apache.cxf.wsdl.interceptors.DocLiteralInInterceptor@33f676f6, org.apache.cxf.binding.soap.interceptor.SoapHeaderInterceptor@4c5ae43b, org.apache.cxf.binding.soap.interceptor.ReadHeadersInterceptor@264f218, org.apache.cxf.binding.soap.interceptor.StartBodyInterceptor@3576ddc2, org.apache.cxf.binding.soap.interceptor.CheckFaultInterceptor@35b74c5c, org.apache.cxf.binding.soap.interceptor.MustUnderstandInterceptor@2e570ded]
15:45:44.716 [main] DEBUG org.apache.cxf.endpoint.ClientImpl - Interceptors contributed by databinging: [org.apache.cxf.jaxb.attachment.JAXBAttachmentSchemaValidationHack@b86de0d]
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.ws.policy.PolicyInInterceptor@536dbea0 to phase receive
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.jaxws.interceptors.WrapperClassInInterceptor@47c81abf to phase post-logical
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.jaxws.interceptors.HolderInInterceptor@776a6d9b to phase pre-invoke
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.jaxws.interceptors.SwAInInterceptor@21d03963 to phase pre-invoke
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.frontend.WSDLGetInterceptor@1f760b47 to phase read
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.interceptor.AttachmentInInterceptor@18ece7f4 to phase receive
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.interceptor.StaxInInterceptor@3cce57c7 to phase post-stream
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.SoapActionInInterceptor@1cf56a1c to phase read
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.wsdl.interceptors.DocLiteralInInterceptor@33f676f6 to phase unmarshal
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.SoapHeaderInterceptor@4c5ae43b to phase unmarshal
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.ReadHeadersInterceptor@264f218 to phase read
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.StartBodyInterceptor@3576ddc2 to phase read
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.CheckFaultInterceptor@35b74c5c to phase post-protocol
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.binding.soap.interceptor.MustUnderstandInterceptor@2e570ded to phase pre-protocol
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.jaxb.attachment.JAXBAttachmentSchemaValidationHack@b86de0d to phase post-protocol
15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Chain org.apache.cxf.phase.PhaseInterceptorChain@81d9a72 was created. Current flow:
  receive [PolicyInInterceptor, AttachmentInInterceptor]
  post-stream [StaxInInterceptor]
  read [WSDLGetInterceptor, ReadHeadersInterceptor, SoapActionInInterceptor, StartBodyInterceptor]
  pre-protocol [MustUnderstandInterceptor]
  post-protocol [CheckFaultInterceptor, JAXBAttachmentSchemaValidationHack]
  unmarshal [DocLiteralInInterceptor, SoapHeaderInterceptor]
  post-logical [WrapperClassInInterceptor]
  pre-invoke [SwAInInterceptor, HolderInInterceptor]

15:45:44.717 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.ws.policy.PolicyInInterceptor@536dbea0
15:45:44.721 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.ws.policy.PolicyVerificationInInterceptor@2ca923bb to phase pre-invoke
15:45:44.721 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Chain org.apache.cxf.phase.PhaseInterceptorChain@81d9a72 was modified. Current flow:
  receive [PolicyInInterceptor, AttachmentInInterceptor]
  post-stream [StaxInInterceptor]
  read [WSDLGetInterceptor, ReadHeadersInterceptor, SoapActionInInterceptor, StartBodyInterceptor]
  pre-protocol [MustUnderstandInterceptor]
  post-protocol [CheckFaultInterceptor, JAXBAttachmentSchemaValidationHack]
  unmarshal [DocLiteralInInterceptor, SoapHeaderInterceptor]
  post-logical [WrapperClassInInterceptor]
  pre-invoke [SwAInInterceptor, HolderInInterceptor, PolicyVerificationInInterceptor]

15:45:44.721 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.interceptor.AttachmentInInterceptor@18ece7f4
15:45:44.722 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.interceptor.StaxInInterceptor@3cce57c7
15:45:44.769 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Adding interceptor org.apache.cxf.interceptor.StaxInEndingInterceptor@651aed93 to phase pre-invoke
15:45:44.769 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Chain org.apache.cxf.phase.PhaseInterceptorChain@81d9a72 was modified. Current flow:
  receive [PolicyInInterceptor, AttachmentInInterceptor]
  post-stream [StaxInInterceptor]
  read [WSDLGetInterceptor, ReadHeadersInterceptor, SoapActionInInterceptor, StartBodyInterceptor]
  pre-protocol [MustUnderstandInterceptor]
  post-protocol [CheckFaultInterceptor, JAXBAttachmentSchemaValidationHack]
  unmarshal [DocLiteralInInterceptor, SoapHeaderInterceptor]
  post-logical [WrapperClassInInterceptor]
  pre-invoke [StaxInEndingInterceptor, SwAInInterceptor, HolderInInterceptor, PolicyVerificationInInterceptor]

15:45:44.769 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.frontend.WSDLGetInterceptor@1f760b47
15:45:44.769 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.ReadHeadersInterceptor@264f218
15:45:44.778 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.SoapActionInInterceptor@1cf56a1c
15:45:44.779 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.StartBodyInterceptor@3576ddc2
15:45:44.779 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.MustUnderstandInterceptor@2e570ded
15:45:44.779 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.CheckFaultInterceptor@35b74c5c
15:45:44.779 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.jaxb.attachment.JAXBAttachmentSchemaValidationHack@b86de0d
15:45:44.779 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.wsdl.interceptors.DocLiteralInInterceptor@33f676f6
15:45:44.790 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.binding.soap.interceptor.SoapHeaderInterceptor@4c5ae43b
15:45:44.790 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.jaxws.interceptors.WrapperClassInInterceptor@47c81abf
15:45:44.793 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.interceptor.StaxInEndingInterceptor@651aed93
15:45:44.794 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.jaxws.interceptors.SwAInInterceptor@21d03963
15:45:44.794 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.jaxws.interceptors.HolderInInterceptor@776a6d9b
15:45:44.794 [main] DEBUG org.apache.cxf.phase.PhaseInterceptorChain - Invoking handleMessage on interceptor org.apache.cxf.ws.policy.PolicyVerificationInInterceptor@2ca923bb
15:45:44.794 [main] DEBUG org.apache.cxf.ws.policy.PolicyVerificationInInterceptor - Verified policies for inbound message.
返回结果:Hello ,Leftso
```

```shell script
2021-04-24 15:44:23.777  INFO 7450 --- [           main] com.leftso.Application                   : Starting Application on ibqodeMacBook-Pro.local with PID 7450 (/Users/ibqo/Develop/git/github/demo-spring-boot-cxf/target/classes started by ibqo in /Users/ibqo/Develop/git/github/demo-spring-boot-cxf)
2021-04-24 15:44:23.779  INFO 7450 --- [           main] com.leftso.Application                   : No active profile set, falling back to default profiles: default
2021-04-24 15:44:23.822  INFO 7450 --- [           main] ationConfigEmbeddedWebApplicationContext : Refreshing org.springframework.boot.context.embedded.AnnotationConfigEmbeddedWebApplicationContext@63a65a25: startup date [Sat Apr 24 15:44:23 CST 2021]; root of context hierarchy
2021-04-24 15:44:24.218  INFO 7450 --- [           main] o.s.b.f.xml.XmlBeanDefinitionReader      : Loading XML bean definitions from class path resource [META-INF/cxf/cxf.xml]
2021-04-24 15:44:24.868  INFO 7450 --- [           main] s.b.c.e.t.TomcatEmbeddedServletContainer : Tomcat initialized with port(s): 8080 (http)
2021-04-24 15:44:24.877  INFO 7450 --- [           main] o.apache.catalina.core.StandardService   : Starting service Tomcat
2021-04-24 15:44:24.878  INFO 7450 --- [           main] org.apache.catalina.core.StandardEngine  : Starting Servlet Engine: Apache Tomcat/8.5.11
2021-04-24 15:44:24.941  INFO 7450 --- [ost-startStop-1] o.a.c.c.C.[Tomcat].[localhost].[/]       : Initializing Spring embedded WebApplicationContext
2021-04-24 15:44:24.941  INFO 7450 --- [ost-startStop-1] o.s.web.context.ContextLoader            : Root WebApplicationContext: initialization completed in 1121 ms
2021-04-24 15:44:25.084  INFO 7450 --- [ost-startStop-1] o.s.b.w.servlet.ServletRegistrationBean  : Mapping servlet: 'dispatcherServlet' to [/]
2021-04-24 15:44:25.086  INFO 7450 --- [ost-startStop-1] o.s.b.w.servlet.ServletRegistrationBean  : Mapping servlet: 'CXFServlet' to [/services/*]
2021-04-24 15:44:25.092  INFO 7450 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'characterEncodingFilter' to: [/*]
2021-04-24 15:44:25.092  INFO 7450 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'hiddenHttpMethodFilter' to: [/*]
2021-04-24 15:44:25.092  INFO 7450 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'httpPutFormContentFilter' to: [/*]
2021-04-24 15:44:25.092  INFO 7450 --- [ost-startStop-1] o.s.b.w.servlet.FilterRegistrationBean   : Mapping filter: 'requestContextFilter' to: [/*]
2021-04-24 15:44:25.242  INFO 7450 --- [           main] o.a.c.w.s.f.ReflectionServiceFactoryBean : Creating Service {http://webservice.leftso.com/}CommonService from class com.leftso.webservice.CommonService
2021-04-24 15:44:25.601  INFO 7450 --- [           main] org.apache.cxf.endpoint.ServerImpl       : Setting the server's publish address to be /CommonService
2021-04-24 15:44:25.775  INFO 7450 --- [           main] s.w.s.m.m.a.RequestMappingHandlerAdapter : Looking for @ControllerAdvice: org.springframework.boot.context.embedded.AnnotationConfigEmbeddedWebApplicationContext@63a65a25: startup date [Sat Apr 24 15:44:23 CST 2021]; root of context hierarchy
2021-04-24 15:44:25.821  INFO 7450 --- [           main] s.w.s.m.m.a.RequestMappingHandlerMapping : Mapped "{[/error],produces=[text/html]}" onto public org.springframework.web.servlet.ModelAndView org.springframework.boot.autoconfigure.web.BasicErrorController.errorHtml(javax.servlet.http.HttpServletRequest,javax.servlet.http.HttpServletResponse)
2021-04-24 15:44:25.821  INFO 7450 --- [           main] s.w.s.m.m.a.RequestMappingHandlerMapping : Mapped "{[/error]}" onto public org.springframework.http.ResponseEntity<java.util.Map<java.lang.String, java.lang.Object>> org.springframework.boot.autoconfigure.web.BasicErrorController.error(javax.servlet.http.HttpServletRequest)
2021-04-24 15:44:25.840  INFO 7450 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/webjars/**] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2021-04-24 15:44:25.841  INFO 7450 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/**] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2021-04-24 15:44:25.864  INFO 7450 --- [           main] o.s.w.s.handler.SimpleUrlHandlerMapping  : Mapped URL path [/**/favicon.ico] onto handler of type [class org.springframework.web.servlet.resource.ResourceHttpRequestHandler]
2021-04-24 15:44:25.956  INFO 7450 --- [           main] o.s.j.e.a.AnnotationMBeanExporter        : Registering beans for JMX exposure on startup
2021-04-24 15:44:26.085  INFO 7450 --- [           main] s.b.c.e.t.TomcatEmbeddedServletContainer : Tomcat started on port(s): 8080 (http)
2021-04-24 15:44:26.093  INFO 7450 --- [           main] com.leftso.Application                   : Started Application in 2.577 seconds (JVM running for 3.437)
2021-04-24 15:46:44.565  INFO 7450 --- [       Thread-7] ationConfigEmbeddedWebApplicationContext : Closing org.springframework.boot.context.embedded.AnnotationConfigEmbeddedWebApplicationContext@63a65a25: startup date [Sat Apr 24 15:44:23 CST 2021]; root of context hierarchy
2021-04-24 15:46:44.568  INFO 7450 --- [       Thread-7] o.s.j.e.a.AnnotationMBeanExporter        : Unregistering JMX-exposed beans on shutdown
```
