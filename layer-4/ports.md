# Ports

We may establish communications between two hosts for a purpose; for example, a web server and client.&#x20;

But how would we allow another application to run between the two hosts at the same time?

How we would distinguish between packets for each application?&#x20;

We do this by using _port numbers_. There is a 16-bit field in the headers of the UDP and TCP protocol which allow us to distinguish one application from another and _multiplex_ multiple protocols to the same IP address. For example,&#x20;

* All unencrypted web traffic will arrive with a destination port of 80
* All encrypted web traffic will arrive with a destination port of 443
* All Telnet traffic will arrive with a port number of 23, etc.
