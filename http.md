# Difference between http 1.1 and http 2<br>
## HTTP<br>
- In 1989, Tim Berners-Lee invented HTTP.<br>
- HTTP (Hypertext Transfer Protocol) is the set of rules for transferring files -- such as text, images, sound, video and other multimedia files -- over the web.<br> 
- It enables the transfer of data between a client and a server.<br>
- It defines how messages are formatted and transmitted, and how web servers and browsers should respond to various commands.


## HTTP 1.1
&nbsp; HTTP/1.1 is the version of the Hypertext Transfer Protocol (HTTP) that was standardized in 1997. It was a significant upgrade over the previous version, HTTP/1.0, and introduced several improvements and new features that are still widely used today.

### Key Features:
- It allowed multiple requests and responses to be sent over a single TCP connection, known as "persistent connections," reducing the overhead of opening and closing connections for each request.
- It introduced the use of request pipelining, which allows multiple requests to be sent without waiting for each response, improving performance.
_ It supported chunked transfer encoding, allowing data to be sent in chunks rather than in a single block, which is useful for streaming large files.