# Difference between http 1.1 and http 2<br>
## HTTP<br>
- In 1989, Tim Berners-Lee invented HTTP.<br>
- HTTP (Hypertext Transfer Protocol) is the set of rules for transferring files -- such as text, images, sound, video and other multimedia files -- over the web.<br> 
- It enables the transfer of data between a client and a server.<br>
- It defines how messages are formatted and transmitted, and how web servers and browsers should respond to various commands.


## HTTP 1.1
&nbsp; HTTP/1.1 is the version of the Hypertext Transfer Protocol (HTTP) that was standardized in 1997. It was a significant upgrade over the previous version, HTTP/1.0, and introduced several improvements and new features that are still widely used today.

### Advantages:
- Widespread Support: HTTP/1.1 is supported by virtually all web servers and browsers, making it a reliable choice for web communication.

- Backward Compatibility: It is backward compatible with HTTP/1.0, allowing servers and clients that support HTTP/1.1 to communicate with older systems that may not support newer versions.

- Simple Implementation: HTTP/1.1 is relatively simple to implement compared to newer versions like HTTP/2, making it an attractive choice for developers working on simpler projects or those with limited resources.

- Caching: HTTP/1.1 includes features for caching resources, which can improve performance by reducing the need to re-fetch resources that have not changed.

- Range Requests: It supports range requests, allowing clients to request specific portions of a resource, which can be useful for resuming interrupted downloads or streaming media.

- Proven Reliability: HTTP/1.1 has been in use for many years and is a well-established protocol with proven reliability in a wide range of web applications.


### Limitations:
- Performance: HTTP/1.1 opens a new connection for each request/response, which can lead to increased latency, especially for websites with many resources (images, scripts, etc.).

- Head-of-Line Blocking: In HTTP/1.1, if one resource is slow to load, it can block other resources from loading, even if they could be loaded more quickly.

- Security: While HTTP/1.1 supports TLS for encryption (resulting in HTTPS), it doesn't require it by default, leaving connections vulnerable to eavesdropping and man-in-the-middle attacks.

- Compression: While HTTP/1.1 supports gzip compression, it's not always used, leading to larger-than-necessary data transfers.

- Multiplexing: HTTP/1.1 doesn't support multiplexing, meaning only one request can be sent on a connection at a time, further increasing latency.

## HTTP 2
HTTP/2, the second major version of the HTTP network protocol, was developed by the HTTP Working Group of the Internet Engineering Task Force (IETF). It was designed to address the limitations of HTTP/1.1 and improve the performance of web applications.

### Advantages
- Multiplexing: HTTP/2 allows multiple requests and responses to be sent and received over a single TCP connection, eliminating the need for multiple connections and reducing latency.

- Header Compression: HTTP/2 uses HPACK compression for HTTP headers, reducing overhead and improving performance, especially for websites with many small resources.

- Server Push: Servers can proactively push resources to clients that they think the client will need, reducing the need for additional round trips and improving performance.

- Stream Prioritization: HTTP/2 allows clients to assign priority to different resources, ensuring that more important resources are delivered first, even if they are requested later.

- Binary Protocol: HTTP/2 is a binary protocol, which allows for more efficient parsing and serialization of data compared to the text-based format of HTTP/1.1.

- Backward Compatibility: HTTP/2 is designed to be backward compatible with HTTP/1.1, allowing servers to support both protocols and gradually transition to HTTP/2.


### Disadvantages:
- Multiplexing: HTTP/2 allows multiple requests and responses to be sent and received over a single TCP connection, eliminating the need for multiple connections and reducing latency.

- Header Compression: HTTP/2 uses HPACK compression for HTTP headers, reducing overhead and improving performance, especially for websites with many small resources.

- Server Push: Servers can proactively push resources to clients that they think the client will need, reducing the need for additional round trips and improving performance.

- Stream Prioritization: HTTP/2 allows clients to assign priority to different resources, ensuring that more important resources are delivered first, even if they are requested later.

- Binary Protocol: HTTP/2 is a binary protocol, which allows for more efficient parsing and serialization of data compared to the text-based format of HTTP/1.1.

- Backward Compatibility: HTTP/2 is designed to be backward compatible with HTTP/1.1, allowing servers to support both protocols and gradually transition to HTTP/2.