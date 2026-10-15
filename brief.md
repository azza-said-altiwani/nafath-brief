Version: NAFATH-V2
Track: AI

## Overview

In this track, I learned important concepts from six fields, Software, AI, Mobile, Networking, Cybersecurity, and Data. From Software, I learned how save and idempotent HTTP methods help to prevent unwanted changes, especially when requests are repeated. In AI, I learned how the overfitting affects the model performance and how I can use cross-validation to help evaluate models. In Mobile, I learned the importance of offline access and synchronizing data when the internet returns back. In Networking, I learned how 5G network slicing can support emergency services, especially when accidents happen. In Cybersecurity, I learned the main phases of incident response lifecycle, step by step. In Data, I compared star schema with snowflake schema and learned which one is suitable for reporting. Finally, I learned that accuracy alone cannot fully evaluate machine learning models, especially with imbalanced data. These concepts helped me understand how to build reliable, secure, and efficient systems. 


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

Accuracy is enough to judge a machine learning model. This is a misconception. But the truth is, accuracy is not always enough to say this model is good, especially with imbalanced data, which means one class has more examples than the other class. When we predict a model with high amount of data in class A, and low amount of data in class B. The accuracy will be high, but it will fail to detect class B. This means it's a high accuracy model, but it performs poorly to detect the other class. Therefore, using evaluation metrics such as recall and F1 score to understand the model performance is better than using accuracy alone.

Resource: Machine Learning: Classification: Accuracy, recall, precision, and related metrics - https://developers.google.com/machine-learning/crash-course/classification/accuracy-precision-recall


## Open Question

I would like to learn how to select the most suitable machine learning algorithm for a specific task and verify which algorithm provides the best results on new data.
