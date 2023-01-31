# Lesson Title

## Learning Goals

- Give an overview of the OSI model.
- Give an overview of the TCP/IP model.
- Explain the main differences between the two models.

## Introduction

In the previous lesson, we learned about layered architecture. We will be
looking at two of the most common models of computer network organization.

## Packets

## The OSI Model

The Open Systems Interconnection (OSI) is a theoretical model developed by the
International Organization for Standardization (ISO). It defines a standard for
various computer systems to communicate with each other. It’s split into the
seven layers.

![Untitled](https://curriculum-content.s3.amazonaws.com/modern-app-dev-managers-leadership/the-osi-and-tcpip-model/01.png)

A brief overview of each layer:

- Application: Represents the interface the user will interact with.
- Presentation: Manages and shapes data to make it easier for the application to
  use it.
- Session: Manages user sessions. You can think of a session as a way for
  determining which user is signed in.
- Transport: Segments data into smaller chunks and encodes/decodes transmission
  information in messages.
- Network: Determines the best routes for message transmission across systems.
- Data Link: Deals with a single link between hosts.
- Physical: Represents the hardware that allows data transmission.

## The TCP/IP Model

While the OSI model is a theoretical model, the TCP/IP model is actually used in
the real world. The OSI model is too complex to be implemented so engineers
developed the TCP/IP system and mapped it to a reference model with 5 abstract
layers.

![Untitled](https://curriculum-content.s3.amazonaws.com/modern-app-dev-managers-leadership/the-osi-and-tcpip-model/02.png)

The layers in the two models perform similarly except for the application layer.
In the TCP/IP model, the application layer encompasses the functionality of the
application, presentation, and session layers from the OSI model.

So why was the OSI model too difficult to implement? It’s because implementing
the logic for the various layers in networking devices would be too expensive.
Instead, the complex logic is implemented on edge devices, i.e., devices that
send and receive messages but don’t handle transmission. These would be devices
like laptops, mobile phones, smart appliances.

All the layers below the application layer in the TCP/IP model involves only the
necessary logic to handle relay messages which makes the overall system more
resilient and faster.

## Conclusion

We have learned about the common models for network organization and why certain
design decisions were made when implementing the TCP/IP model.
