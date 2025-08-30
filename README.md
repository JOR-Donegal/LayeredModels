# Introduction

Once systems become very complex, they can become unmanageable. I don’t know if anyone has a rule of thumb, but if not, I’ll claim this one (JOR’s first law of complexity!).&#x20;

_**When you double the number of components in a system, you square its complexity.**_&#x20;

So, there we have it, a completely new hypothesis (arbitrary and unproven) in the lexicon of Science!&#x20;

Is it true…… I have no idea!&#x20;

Does it roughly describe what we experience…yes!&#x20;

For much of the past 60 years we have struggled with the notion of complexity. We really started understanding the magnitude of the problem as very complex projects occurred; the space race in the 1960s resulted in the development of many new forms of logistical planning and tracking.&#x20;

For a while, we found ways of mitigating the problems of complexity. We had seen spaghetti code; programs which were so complex and unwieldy as to be unmaintainable. We addressed those problems with structure, functions and later object orientation and code reuse. In early UNIX development, the folks had a great ideology; each tool does one and one job only. Make each tool as simple as possible. This was a great way of mitigating some of the early issues.&#x20;

In telecommunications, we often take the same approach. Suppose we look at the physical way of connecting things. We could use wires of many different types, fiber optics, radio, smoke signals, carrier pigeons etc. Does an application like a web browser need to know how data packets are being carried?&#x20;

Probably not.

The easy way to approach these things is to compartmentalize all the things we want to be able to do into layers and let each layer be independent of the others. If we need to change a layer, we just need to worry about its inter-connectedness to other layers, not what is in the layer itself. So an application which can work on a modem, can work on Ethernet or on a radio network.&#x20;

In the early days of development of this layered approach to communications there were many contributors, none of whom agreed. The result was a compromise which didn’t really suit anybody, but that we still use to this day to describe the layers and inter-relations in a communications model.&#x20;

In the next few pages, we will look at how layered models allow us to describe how nodes (computer, printers, etc.) connected to networks, interconnect with each other. In each case we will look at the most typical protocols you are likely to be exposed to. Keep in mind that there are many other alternatives out there!
