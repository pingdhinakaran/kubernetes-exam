For interview, please brush up on Networking as well - 

1. Load average - done 

2. DNS flow -done 

1) You type maps.google.com into the address bar of your browser.

2) The browser checks the cache for a DNS record to find the corresponding IP address of maps.google.com.

3)If the requested URL is not in the cache, ISP’s DNS server initiates a DNS query to find the IP address of the server that hosts maps.google.com.

4)The browser initiates a TCP connection with the server.

5)The browser sends an HTTP request to the webserver.

6)The server handles the request and sends back a response.

7)The server sends out an HTTP response.

8)The browser displays the HTML content (for HTML responses, which is the most common).


Http vs https, 

Http:                     Https

Plain text               Encrypted data
layer 7 (application)    layer 4 ( Transport)
insecure                 key exchange
light weight             heaviver then http
                         certificate authority (CA)
                         port 443
                         Http over TLS / SSL 
SLL certificate

webserver

proxy vs redirection

With a redirect,  the server tells the client to look elsewhere for the resource. The client will be aware of this new location. The new location must be reachable from the client.

A reverse proxy instead forwards the request of the client to some other location itself and sends the response from this location back to the client. 
This means that the client is not aware of the new location and that the new location does not need to be directly reachable by the client. server can routes to internal ip to proxy server 

HTTP request vs HTTP response.

HttpRequest is one such data which is sent to the server by a client while making a request, 

HttpResponse is the other set of data which is sent back to the client from the server

TCP/UDP


Hardlink/softlink
Kubernetes, Ingress, 
docker, 
Linux, 
AWS, 
Terraform
Linux commands -
Free-m
Netstat
lowait
Inode
Telnet/nc
Tracerroute
HELM - Package Management
Load balancers
differences b/w ELB/ALB/NLB