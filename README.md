# COMP3100 Distributed Systems

This is an assignment attempted by the students of Macquarie under the unit of Distributed Systems COMP3100. The aim of this assignment is to create a job scheduler based of priority scheduling, implemented into a client-server communication model.

## Introduction

Job schedulers have been used different areas; some uses are more common that others however they are most often in charge of the execution of jobs for unattended background programs. Job schedulers have the task of allocating system resources for the execution of different tasks or jobs by a system.

As for the priority at which the jobs are done, that is entirely dependent on the pre-defined set of rules and the algorithm that the assigned to the job scheduler. It is essentially an automated system that initiates and manages job. Typically, job schedulers are created such that they can easily be controlled by a user; this is done by implementing a GUI that allows users to have a single access point of control.

## Project Description

The project revolves around the concept of job or task scheduling with client-server models. The server is set up to be a Linux based server with the use of a VM. The use of a Linux based server was chosen for its stability and reliability. The code for the client and the server is written in Java as per the ease of use and familiarity from students involved in the project. This job scheduler is created with the topic of implementation in a distributed system in mind.

## Design Philosophy
To create an Intelligent Job Scheduler for distributed systems that allows for improved user interfaces that rival traditional desktop software that performs simulations and visualisations. We will also be using free or open source software (FOSS) libraries and frameworks on both the client-side and server-side that facilitate low-cost and rapid application development that complies to modern practices. 

## Client-side Simulator
A client-side simulator is a simulation program that runs on a computer that makes a request for services. Our client-side simulator will be implementing socket programming and will be using networking services that will be provided to us by the transport layer. The Transport Control Protocol (TCP) will provide a reliable flow of data between client-side simulators whereas the User Datagram Protocol (UDP) will send independent packets of data from one client-side to another with no guarantees about arrival and sequencing. However, in order to utilise the client-side to the best of its ability the group will have to ensure prior to the client-side simulator running,  that no firewall is active and blocks the communication between the client-side and server-side. 


## Server-Side Simulator
A server-side simulator a simulation program that runs on a computer that offers requested services from one or more clients. The server-side simulator provided to all students uses socket programming and is assigned to a specific port. The server-side simulator will then listen to the socket and wait for the client-side to make a connection request.  When the server-side simulator accepts the connection, it will receive a new socket that is assigned to a different port. It is important to note that the server-side will continue to require a new socket and port number so that it can continue to listen to the original socket for connection requests while serving the connected client. 

## Considerations
A consideration of the client-side simulator is the possibility of client-side attacks occurring. Client-side attacks are attacks that initiate when a user downloads malicious content off the internet. They also take advantage of weaknesses in the software that are loaded onto clients. Two types of client-side attacks that need to be considered include content spoofing which tricks a user into believing that the content on a website is true and is not from an external source whereas cross-site Scripting (XSS) enables an attacker to execute scripts in a user’s web browser. 

## Constraints 
A major constraint that needs to be considered for both client-side and server-side simulators is how fast the user is able to catch invalid data on the client-side. If the user is able to catch invalid data on the client-side, they can fix it right away, however if the data gets to the server-side and is rejected, a significant delay is instigated by a round-trip to the server-side and then back to the client-side to inform the user to fix the data. 

