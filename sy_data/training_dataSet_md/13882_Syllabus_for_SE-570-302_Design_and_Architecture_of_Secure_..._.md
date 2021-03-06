#  Syllabus for SE-570-101 Design and Architecture of Secure Software Systems,
Fall 2002

## Overview

This course will investigate the design and implementation of secure systems
using cryptographic techniques and the security mechanisms found in the
runtime environments of modern programming languages such as Java or C#. You
will learn about ciphers and models of access control, as well as how class-
loaders, byte-code verification, security managers, access control, and
permissions are used to ensure security within Java. There will be a strong
emphasis upon applying the theory that is discussed (using Java).

## Lecture Plan

The following lecture plan is tentative and subject to change as the course
progresses.

  * **Week 1:** (2002/09/17) course overview; DES; key distribution. 
  * **Week 2:** (2002/09/23) Implementing DES; PKCS #5 padding; cipher modes; validating plaintext; naive key distribution 
  * **Week 3:** (2002/10/01) Ciphers; multiple encryption; key establishment protocols using symmetric-key ciphers; cryptographic hash functions. 
  * **Week 4:** (2002/10/08) Asymmetric Ciphers and RSA 
  * **Week 5:** (2002/10/15) _midterm exam_
  * **Week 6:** (2002/10/22) Certificates and JCE 
  * **Week 7:** (2002/10/29) Authentication; authorisation; access matrices; access-control lists (ACLs); capability lists; access control in Java. 
  * **Week 8:** (2002/11/05) Security models; multi-level access control; information flow; state-machine models; access control in Java (permissions, stack-walking, guarded objects, delegates). 
  * **Week 9:** (2002/11/12) To be announced 
  * **Week 10:** (2002/11/19) Runtime-system integrity; buffer overflows; dynamic loading and linking; untrusted code; static analysis / bytecode verification. 
  * **Week 11:** (2002/11/26) _final exam_

Lecture slides will be available after each lecture. They will not normally be
available before the lecture.

## Prerequisites

You _must_ have considerable experience with Java (at least CSC 224 and SE
450) and some exposure to C or C++ (including pointer arithmetic).

Very useful, but optional:

  * CSC 447 Concepts of Programming Languages 
  * DS 420 Foundations of Distributed Systems 
  * SE 550 Distributed Software Development 

## Detailed Overview

We will study:

  * Symmetric-key ciphers: DES; DES3; cipher modes of operation; how to use symmetric-key ciphers securely; implementation details; efficiency concerns. 
  * Cryptographic hash functions: MD5; comparison with MACs; using digest algorithms to build MACs. 
  * Asymmetric-key ciphers: RSA; using asymmetric-key ciphers for authentication and digital signatures; public-key infrastructure; implementation details; efficiency concerns. 
  * Cryptographic protocols: Dolev-Yao threat model; Needham-Schroeder protocol (symmetric-key and asymmetric-key versions); Yahalom protocol; Wide-Mouthed Frog protocol; using nonces and timestamps. 
  * Java Cryptography Architecture (JCA): provider architecture; symmetric-key ciphers, message digests, and asymmetric-key ciphers with Java Cryptography Extension (JCE); key management. 
  * Runtime-system integrity: use of stacks; pointers into the stack; using pointer arithmetic to violate stack integrity; buffer overflow example in C (on x86); byte-code verification. 
  * Dynamic loading and linking: class loading; signing code. 
  * Authorization and access control: authentication vs. authorization; design principles; authorization lists; capabilities; permissions; protection domains; access control based upon stack-walking; security manager; access controller; circumventing stack-walking using privileged code. 

## Course Objectives

By the end of this course you should:

  * Be very familiar with common cryptographic algorithms such as DES and RSA. 
  * Be able to implement cryptographic algorithms from their specifications. 
  * Have practical experience with the majority of the Java Cryptography Architecture. 
  * Be familiar with common vulnerabilities in cryptographic protocols, and how they can be avoided. 
  * Be able to recognize unsound security practices in software systems. 
  * Understand Java's class-loading mechanism. 
  * Understand Java's security model for the execution of untrusted code. 
  * Have practical experience with designing APIs that cross security boundaries. 

## Textbooks

**Required:**

  * Java Security, by Scott Oaks, 2nd edition, May 2001, ISBN 0596001576. 
  * Security Engineering, 2001, by Ross Anderson, published by Wiley, ISBN 0471389226. 

**Optional:**

You may want a cryptography or cryptology reference. There are several
options.

The best option is the most expensive, unfortunately. The  "Dr. Dobb's Journal
Essential Books on Cryptography & Security CD" contains seven very good books
on cryptography and security in PDF. Some of these books are out of print,
and, individually, some of the hardcopies are as expensive as the CD. Of
course, you do have to read them online or print them. The CD contains the
following books:

  * Applied Cryptography: Protocols, Algorithms, and Source Code in C, second edition 
  * Cryptography: A New Dimension in Computer Data Security 
  * Contemporary Cryptology: The Science of Information 
  * Cryptography and Data Security  (this would be required if still in print) 
  * Applied Cryptography, Cryptographic Protocols, and Computer Security 
  * Cryptography: Theory and Practice 
  * Handbook of Applied Cryptography 
  * Military Cryptanalysis, Volume I-IV 
  * RSA Laboratories FAQ on Cryptography, RSA Laboratories Technical Reports, RSA Laboratories Security Bulletins, and CryptoBytes Newsletter 

If the link to  "Dr. Dobb's Journal Essential Books on Cryptography & Security
CD" does not work, go to the  Dr. Dobb's CDROM store , and you will be
forwarded to the Digital River site. Follow the link for "Essential Book
Collections on CD-ROM", and you should then see the link for "Dr. Dobb's
Journal Essential Books on Cryptography & Security CD".

If you would prefer a physical book, I recommend the following books in this
order:

  * Cryptography & Network Security: Principles & Practice 
  * Applied Cryptography: Protocols, Algorithms, and Source Code in C, second edition 
  * Handbook of Applied Cryptography  (very good, but difficult unless you have a strong mathematical background) 

The following books are very good, but not necessary for this course. Ask me
before you order them.

  * SSL and TLS: Designing and Building Secure Systems 
  * SSL & TLS Essentials: Securing the Web 
  * Securing Java: Getting Down to Business with Mobile Code, second edition 
  * Java Cryptography 
  * Codes and Cryptography 
  * Modelling and Analysis of Security Protocols 

## Contact Information

 **Instructor:** Corin Pitcher  
 **Instructor Home Page:** ` http://fpl.cs.depaul.edu/cpitcher/`  
 **Instructor Email:** ` cpitcher@cs.depaul.edu`  
 **Phone:** 312/362-5248  
 **Office:** Room 838, Suite 401, School of CTI, DePaul University, 243 South
Wabash Avenue, Chicago, IL 60604-2301, USA  
 **Office Hours:** TO BE ANNOUNCED  
**Course Home Page:** ` http://fpl.cs.depaul.edu/cpitcher/se570/`  

## Attendance

_You must attend both the midterm (Tuesday 2002/10/15) and final (Tuesday
2002/11/26) exams. A medical note will be required for an absence. Business
trips or vacations are not valid reasons for missing the exams. Block out
those dates now!_

Class attendance is strongly encouraged, but not mandatory. However, if you
are absent from class you are responsible for understanding the material and
for finding out about any announcements made in that class.

## Assessment

Your final grade will be based on:

  * Homework: 50% 
  * Midterm and final exams: 25% each 

Assessment for homework assignments will be based on whether they achieve the
set task _and_ quality of the code.

Unless otherwise stated, homework assignments are due by 5:45PM on the day of
the class after the class in which they are assigned. You are expected to
complete all of the homework assignments by the deadline. Late homework
submissions will not be accepted, and all homework assignments will count
towards the final grade.

Homework assignments must be submitted through the online system. _Email
submissions will not be accepted._

There will be no extra credit homework and/or projects.

