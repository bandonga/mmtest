---
title: Sysadmin - Basic concepts
date: 2018-04-20 00:00:00 +01:00
header:
  teaser: "/assets/images/academy/sysadmin.png"
  image: "/assets/images/academy/sysadmin.png"
categories:
- academy
tags:
- academy
- sysadmin
excerpt: "Basic concepts for a Sysadmin."
toc: true
toc_hmax: 5
---

> Related with: [Sysadmin]({{ site.baseurl }}{% post_url /academy/2018-05-18-sysadmin %})

##### AS
An *AS* is software framework that handles application operations from the end user to the back-end business processes and databases and provide an environment to run them.

##### XA/Open XA
*XA/Open XA* (Extended Architecture) describes the interface between the global transaction manager and the local resource manager. The goal of XA is to allow multiple resources (such as databases, application servers, message queues, transactional caches, etc.) to be accessed within the same transaction, thereby preserving the ACID (Atomicity, Consistency, Isolation, Durability) properties across applications. XA uses a two-phase commit to ensure that all resources either commit or roll back any particular transaction consistently.

##### Distributed System
A *distributed system* is a model in which components located on networked computers communicate and coordinate their actions by passing messages. The work is divided across similar modules and demand increases, more can be added making the system more scalable. The failure of a single module has less impact on the system, which makes the system more available. The goal is to better manage the complexity and resulting cost of providing highly available and scalable systems.

##### Scalability
*Scalability* is how well a system can adapt to increased demands.

##### High availability
*High availability* requires that a system is up and running as close to 24/7 as possible, by using load balancing and failover techniques. Availability is a measure of a system's ability to process client requests without downtime.

##### RPC
A *RPC* (Remote Procedure Call) is when a computer program causes a procedure  to execute in a different address space, which is coded as if it were a local procedure call.

##### SOA
With *SOA* (Service Oriented architecture) services are provided to the other components by application components, through a communication protocol over a network. The basic principles of service-oriented architecture are independent of vendors, products and technologies: it logically represents a business activity with a specified outcome, self-contained and a black box for its consumers and may consist of other underlying services.

##### ESB
An *ESB* (Enterprise Service Bus) implements a communication system between mutually interacting software applications in a SOA.

##### EAI
*EAI* (Enterprise Application Integration) is an integration framework composed of a collection of technologies and services which form a middleware to enable integration of systems and applications across an enterprise.

##### MOM
*MOM* (Message Oriented Middleware) makes use of messaging provider to mediate messaging operations between distributed systems.

The basic elements of a MOM system are clients, messages, and the MOM provider, which includes an API and administrative tools.
A client makes an API call to send a message to a destination managed by the provider. The provider services route and deliver the message, retaining the message until a receiving client retrieves it.

The messaging provider have administrative tools, to monitor and tune performance. Since it's an asynchronous system, the clients can continue to load work and can use all resources, failing the message handling.

The MOM provider uses different architectures to route and deliver messages: it can use a centralized message server or it can distribute routing and delivery functions to each client machine. Some MOM products combine these two approaches.

##### Message Broker
*Message broker* is a system which handles messages (sending and receiving), routing messages to the specific consumer/recipient. It's built upon a *MOM*, that provides the base communication among the applications, message persistence and guaranteed delivery.
