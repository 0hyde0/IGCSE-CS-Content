# Chapter 2.1: Types and methods of data transmission

Objectives

```
Understand that data is broken down into packets for transmission
Can describe how packet switching works
Can describe how data is transmitted from one device to another and explain which data transmission method to use, for a given scenario
```

## Packet Anatomy 101

``Packets`` are used everywhere on the internet. They're also the ones powering Minecraft and how the server connects with the client. 

Packets are the result of ``packet switching``, which is a process where ``data is broken down into packets``. These ``packets may take a different route``, which are ``controlled by the router``, and ``could arrive out of order to the receiver``. They can however be ``reordered once the last packet has arrived``.

The structure of a packet begins with the ``packet header``, which contains the ``destination address`` and ``originator's address``. They represent where the packet should be sent and where it came from. It also contains the ``packet number``, which represents which packet is which out of a group of packets.

The next one would be the ``payload``, which contains a chunk of the original data. Of course, the payload may sometimes be tampered with due to interference. This is where the ``trailer`` comes in, which contains the data for any error-checking systems used and also marks the end of a packet.

In a nutshell, a packet contains

* The header, which contains the destination address and the originator's address, and also includes a packet number for reordering.
* The payload, which is the actual transmitted data.
* The trailer, which contains error-checking information and indicates the end of a packet.

Packet switching is a process where
* Data is broken down into packets
* ... and are sent to their destination via different routes.
* Routers dictate the best route for each packet
* ... and are reordered once arrive since they may arrive out of order.

## Types of data transmission methods

``Serial`` and ``parallel``, they somewhat represent how roads work. 

Take ``serial``, it represents a road that can go as far as possible but would take a large amount of time to reach from point A to B, especially if it is somewhat crowded.
``Parallel`` is more of like a highway, where multiple cars can drive faster, within a short distance, all at about the same time.

In computer science, a ``serial`` data transmission would have data travelling over a single wire, while a ``parallel`` data transmission has data passing through multiple.

There is also another factor to this, ``simplex``, for example, has data travelling in only one direction. An example of a ``simplex`` data transmission would be sending data from a computer to a monitor.

``Full-duplex``, however, is the complete opposite of simplex. It allows data to travel in both directions at the same time, at a high cost. One example would be a network cable. 

``Half-duplex`` is somewhat the middle child among the 3, with it allowing data to travel in both directions, but only one at a time. It's cheaper than simplex for bidirectional transmission but is slower than full-duplex. An example would be when a printer receives data from a computer and sends an error message back once completed.


These data transmission methods can combine each, with all combinations present below.

``Serial-simplex``
* Unidirectional data transmission one bit at a time.

``Serial-half-duplex``
* Bidirectional data transmission, a bit in one direction at a time.

``Serial-full-duplex``
* Bidirectional data transmission, a bit in both directions at a time.

``Parallel-simplex``
* Multi unidirectional data transmission.

``Parallel-half-duplex``
* Multi-bidirectional data transmission, multiple bits in one direction at a time.

``Parallel-full-duplex``
* Multi-bidirectional data transmission, multiple bits in both directions simultaneously.