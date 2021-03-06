
# CRLF
 - CRLF refers to the special character elements "Carriage Return" and "Line Feed."
These elements are embedded in HTTP headers and other software code to signify an End of Line (EOL) marker.

 - The empty line denotes the end of the request/response headers.

# URL
 - Uniform Resource Locator (URL)
 - A URL - a reference to a web resource that (location on a network a& a mechanism for retrieving it)
 - A URL - a type of URI (Uniform Resource Identifier)
 - Protocol, Host, Port, Path, Query String, Fragment

 - (Default) Ports 80 (HTTP) and 443 (HTTPS) 

 - Hypertext Transfer Protocol Secure (https) is a combination of the Hypertext Transfer Protocol (HTTP)
with the Secure Socket Layer (SSL)/Transport Layer Security (TLS) protocol. TLS is an authentication
and security protocol widely implemented in browsers and Web servers.

 - URLs are encoded according RFC 1738
    - All other characters are escaped by "%[character hex code]"

# MIME (& Media Types)
 - Multi-Purpose Internet Mail Extensions
 - Internet standard for encoding resources
    (Originally) developed for email attachments
    Used in Internet protocols like HTTP and SMTP
 - MIME Type / Subtype
    - application/json, image/png, image/gif, text/html, text/plain, text/xml, video/mp4, application/pdf

# HTTP Request Message
 - Request message sent by a client consists of:
    - HTTP request line
	- Request method (GET / POST / PUT / DELETE / …)
	- Resource URI (URL)
	- Protocol version
    - HTTP request headers
	- Additional parameters
    - HTTP request body
	– optional data e.g., posted form fields

### POST Request Method 
 - The POST method transfers data in the HTTP body
 - POST can send text and binary data e.g., upload files


# HTTP Response Message
 - The response message sent by the HTTP server consists of:
    - HTTP response status line
		- Protocol version
		- Status code
		- Status text
    - Response headers
		- Provide meta data about the returned resource
    - Response body
		- The content of the HTTP response (data)

# HTTP response code classes
 - status code <=> status text
 	- 1xx: informational (e.g., "100 Continue")
 	- 2xx: successful (e.g., "200 OK", "201 Created")
 	- 3xx: redirection (e.g., "301 Moved Permanently", "302 Found", "304 Not Modified")
 	- 4xx: client error (e.g., "400 Bad Request", "401 Unauthorized", "404 Not Found", "409 Conflict")
 	- 5xx: server error (e.g., "500 Internal Server Error", "503 Service Unavailable")

### Browser Redirection
 - This HTTP response (301 Moved Permanently) tells the browser to request another URL:
	HTTP/1.1 301 Moved Permanently
	Location: [enter URL here]
	...

# Content-Type (& Content-Disposition)
 - Content-Type response header the server specifies how the output should be processed

 - Content-Type: text/html; charset=utf-8
 - Content-Type: application/pdf
   Content-Disposition: attachment; filename="[some_file_name]"



# ASCII
 - American Standard Code for Information Interchange, a standard data-encoding format for electronic communication between computers.
ASCII assigns standard numeric values to letters, numerals, punctuation marks, and other characters used in computers.
 - It is a code for representing 128 English characters as numbers, with each letter assigned a number from 0 to 127.
For example, the ASCII code for uppercase M is 77.
Most computers use ASCII codes to represent text, which makes it possible to transfer data from one computer to another.


# UUID
 - A UUID (Universal Unique Identifier) is a 128-bit value used to uniquely identify an object or entity on the internet.
Depending on the specific mechanisms used, a UUID is either guaranteed to be different or is, at least,
extremely likely to be different from any other UUID generated until A.D. 3400.

 - Универсален уникален идентификатор е 128-битов етикет, използван за информация в компютърните системи.
Използва се и терминът глобално уникален идентификатор. Когато се генерират съгласно стандартните методи,
UUID са уникални за практически цели.

