# OSI Model

## Learning goals

- Understand what the OSI model represents and learn what each layer stands for

## Introduction

Now that we've become acquainted with the inner-workings of the internet, let's take a look at how it all comes together by breaking down the anatomy of a network. A very commonly used conceptual model used to explain networks is the *OSI* model.

## OSI

The **OSI** (Open Systems Interconnection) model is a *conceptual framework* frequently used to describe the way information is transmitted over a network. It consists of a whopping *seven* layers, each of which describes a specific function in the transmission of data.

Let's break down what each of the layers represent, with some examples of what it looks like in practice!

## L1 - Physical Layer

The **physical layer** is the most immediately apparent in a network connection. It is the part responsible for actual physical transmission of data over a network. It defines the characteristics of the physical connection, such as the type of cable used and the type of signals that are sent and received.

An example of this layer would be a network cable (e.g. ethernet cable) connecting a computer to a router or another computer.

## L2 - Data Link Layer

The **data link layer** is responsible for the transmission of data between two points (nodes) on a network. It tries to ensure that data is sent in the correct order, in an error-free fashion.

A network switch forwarding data between computers in a network would be an example of this layer.

## L3 - Network Layer

The **network layer** is similar to the data link layer, in that it is also responsible for the transmission of data between two points. The difference is the network layer focuses on routing data between different networks. It determines what the best (fastest and most reliable) path data can take, as well as handling congestion control.

A good example of the network layer is a router transferring data to another network.

## L4 - Transport Layer

The **transport layer** establishes a connection between two nodes, and then focuses on ensuring that data is transmitted reliably between them. Additionally, it can provide certain features like error correction and flow control. 

Examples of the transport layer includes network protocols that handle data transmission, such as TCP or UDP as seen in earlier chapters.

## L5 - Session Layer

The **session layer** is responsible for managing and *coordinating* communications between two nodes on a network, while also optionally handling security and authentication.

An example of the session layer would be something like two devices (server and web browser) using HTTPS to establish and maintain a secure connection.

## L6 - Presentation Layer

The **presentation layer** focuses on *formatting* and *arranging* the data being transferred in such a way that it can be understood by the next layer, the application layer. It can handle things like compression (reducing the size of the data), encryption (securing the data), as well as translating between different data formats.

A web browser displaying an image makes use of the presentation layer, as that image was most likely compressed beforehand to reduce the file size and network load.

## L7 - Application Layer

The final layer is the **application layer**, which is responsible for providing network access to applications. This includes protocols we've gone over like HTTP for web browsing and SMTP for email.

Any application using network services qualifies as an example; for instance, a web browser using HTTP to retrieve a website from a web server and display it on your screen.

## Conclusion

![OSI layers summarized](https://curriculum-content.s3.amazonaws.com/6685/devops-m1-osi/osi.jpg)

The OSI model provides us with a framework that is useful for understanding the various steps that go into transmitting data over a network. Hopefully this lesson helps to demystify the way networks operate, and how the protocols we have covered so far factor into it!