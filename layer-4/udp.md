---
description: User Datagram Protocol
---

# UDP

Many network applications do not require reliable host to host communications. For example, if we are streaming audio or video, there is no point adding back a missing frame two seconds after it should have been in the audio stream. We also have _multi-cast_ traffic; traffic which egresses from one node but is received by many. UDP provides an unreliable service and datagrams may arrive out of order, appear duplicated, or go missing without notice.

UDP is encapsulated in the IP packet.

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

We use this type of unreliable protocol for services like DNS and SYSLOG.
