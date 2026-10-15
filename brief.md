Version: NAFATH-V2
Track: AI

## Overview

<text>

<url>


## Software

Safe methods like GET, HEAD, OPTIONS, TRACE are those who does not ask the server to change their state and they are read-only methods. Idempotent methods like all safe methods with PUT and DELETE which are repeating the identical requests with same effect when sending them. They all are important when the connection failed before response, with idempotent methods clients are able to send another request without having effect unlike POST method which is non-idempotent method.

Resource: RFC 9110: STD 97: HTTP Semantics - https://www.rfc-editor.org/info/rfc9110/#section-9.2.1


## AI

Overfitting means that the model learns the training data too well, especially the noise data from the old network, but it cannot predict the new data. To solve this problem by using Cross-validation by divide the data in many parts, then we train the model in many parts to make sure whether it is learning or just saving the data. If the result is good in training data and bad in testing data, that is may be overfitting.

Resource: Scikit Learn: Underfitting vs. Overfitting - https://scikit-learn.org/stable/auto_examples/model_selection/plot_underfitting_overfitting.html


## Mobile

The responder's mobile app must support working without internet by saving the data in mobile itself and allowing users to reach and save the important information anytime when the app is offline. It also must synchronize the local data with server whenever the internet returns back. Also, it should update the latest information which the user may change them by solving any conflicts to prevent losing the data.

Resource: Android Developers: Build an offline-first app - https://developer.android.com/topic/architecture/data-layer/offline-first


## Networking

5G network slicing means to divide one network into different virtual networks, and each one of them have its own requirements and purpose based on users need, for example one of these parts is for emergency. This can help more when there is an accident in a crowded street, all people are using their phones in same time, but with 5G network slicing technique police and emergency can use their virtual network for fast working.

Resource: Geeks for Geeks: Network Slicing in 5G Networks - https://www.geeksforgeeks.org/computer-networks/network-slicing-in-5g-networks/


## Cybersecurity

Incident response lifecycle. It is sequence steps to handle attacks and protect systems. Preparation, to prepare a security system, plan, and the tools. Detection and Analysis, to detect the attack and understand what's happening. Containment, to stop the attack from spreading other systems. Eradication, to remove the reason of attack, such as malware. Recovery, to restore the service, and check it. Learn a Lesson, by write everything happens, understand the mistake and improve the security to prevent future attacks.

Resource: NIST SP 800-61 Revision 2: Computer Security Incident Handling Guide - https://csrc.nist.gov/pubs/sp/800/61/r2/final

## Data

Both of them are way to save data in the database. Star schema have a central fact table, which connected to other tables. It's easy to understand and use. Snowflake schema have a fact table connected with others, but the other tables also connect with many others. It decreases the duplication and just complex to understand. Star schema is best choice because it's simple and easy to connect data with services based on dates and region to provide fast reporting.

Resource: Kimball Group: Dimensional Modeling Techniques - https://www.kimballgroup.com/data-warehouse-business-intelligence-resources/kimball-techniques/dimensional-modeling-techniques/


## Misconception in My Track

<text>

<url>


## Open Question

<text>

<url>
