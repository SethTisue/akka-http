<a id="http-client-side-java"></a>
# Consuming HTTP-based Services (Client-Side)

All client-side functionality of Akka HTTP, for consuming HTTP-based services offered by other endpoints, is currently
provided by the `akka-http-core` module.

Depending on your application's specific needs you can choose from three different API levels:

@ref[Connection-Level Client-Side API](connection-level.md#connection-level-api-java)
:   for full-control over when HTTP connections are opened/closed and how requests are scheduled across them

@ref[Host-Level Client-Side API](host-level.md#host-level-api-java)
:   for letting Akka HTTP manage a connection-pool to *one specific* host/port endpoint

@ref[Request-Level Client-Side API](request-level.md#request-level-api-java)
:   for letting Akka HTTP perform all connection management

You can interact with different API levels at the same time and, independently of which API level you choose,
Akka HTTP will happily handle many thousand concurrent connections to a single or many different hosts.

@@toc { depth=3 }

@@@ index

* [connection-level](connection-level.md)
* [host-level](host-level.md)
* [request-level](request-level.md)
* [client-https-support](client-https-support.md)
* [websocket-support](websocket-support.md)

@@@
