# Simple Web Stack

![Image of a simple web stack](https://i.imgur.com/PdoOZ0l.png)

## Description

This is a simple web infrastructure, in which a website is reachable via "www.foobar.com". in this infrastructure there are no firewalls or SSL certificates for pretexting the server's network, and all components share the resources (CPU, RAM and SSD) provided by the server.

## Specifics About This Infrastructure

+ What is a server ?<br/>A server is a computer hardware or software that provides services to other computers, which are usually referred to as *clients*.

+ What is the role of a domaine name ?<br/>To provide a human-friendly (text-based) alias for an IP Address. For example, the domain name `www.wikipedia.org` is easier to recognize and remember than `91.198.174.192`. The IP address and domain name alias is mapped in the Domain Name System (DNS)

+ What type of DNS record `www` is in `www.foobar.com`?<br/>`www.foobar.com` uses the **A record**.
<i>Address Mapping record (A Record)—also known as a DNS host record, stores a hostname and its corresponding IPv4 address.</i>

+ What is the role of a web server ?<br/>The web server is a software/hardware that accepts requests via HTTP or secure HTTP (HTTPS) and responds with the content of the requested resource or an error messsage.

+ What is the role of the application server ?<br/>To install, operate and host applications and associated services for end users, IT services and organizations and facilitates the hosting and delivery of high-end consumer or business applications

+ What is the role of the database?<br/>The role of a database is to maintain a collection of organized information that can easily be accessed, managed and updated

+ What the server uses to communicate with the client (computer of the user requesting the website)?<br/>Communication between the client and the server occurs over the internet network through the TCP/IP protocol suite.

## Issues With This Infrastructure

+ There are multiple SPOF (Single Point Of Failure) in this infrastructure;<br/>For example, if the MySQL database server is down, the entire site would be down.

+ Downtime when maintenance needed;<br/>When we need to run some maintenance checks on any component, they have to be put down or the server has to be turned off. Since there's only one server, the website would be experiencing a downtime.

+ Cannot scale if there's too much incoming traffic;<br/>It would be hard to scale this infrastructure becauses one server contains the required components. The server can quickly run out of resources or slow down when it starts receiving a lot of requests.
