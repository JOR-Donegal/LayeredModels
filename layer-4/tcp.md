---
description: Transmission Control Protocol
---

# TCP

The first trick we have is to ensure that if a packet is lost, we can identify it and ask for a resend of exactly that packet. Or if packets arrive out of sequence that we can rearrange the data into the correct order. We do this by numbering each packet We send with a unique 32-bit number to do this. Each packet sent is acknowledged by a return packet which also has a unique 32-bit number. Rather than sending packets into a black hole, the effect of this is to establish host to host communications.&#x20;

TCP also includes a flow control mechanism. We could send just one packet and wait for an acknowledgement, but this would be very slow. A better way to send packets is to use a _sliding window_. The sender will send a fixed number of packets before getting an acknowledgement. If everything works, the sender will now increase the number of packets it will send without waiting for an acknowledgement. Eventually, packets will be lost and the sender will reduce the number of packets in transit again, a sliding window. There are many other features in the TCP stack, some of the features are arguably layer 5. Do some background reading on it.

TCP is encapsulated in the IP packet.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

It is very important that you understand the concept of _encapsulation_.
