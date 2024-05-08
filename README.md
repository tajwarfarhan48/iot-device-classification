# Intro

A set of IoT-device classifiers that can detect the type of an IoT device based on link-level network traffic. This code was written for a research paper which was presented at ICISSP (International Conference on Information Systems Security and Privacy) 2024 in Rome, Italy. Our novel contribution was the use of LLMs in conjunction with traditional ML models for this type of task.

The paper uses two primary datasets:
1. UNSW - A dataset of 900,000+ IoT devices by the University of New South Wales (UNSW) 
2. ZBW - An in-house dataset of IoT devices from our lab

These datasets were processed using a program called Protoflow (created by another paper author - Gabriel Morales) to extract the link-level network information.

The actual paper is provided in the repo (paper.pdf).

Conference Link: https://www.insticc.org/node/TechnicalProgram/icissp/2024/presentationDetails/123657

# Research Paper Abstract

Technological advancement has made strides due in part to added convenience in our daily lives. This addition of automation and quick access to information has given rise to the Internet-of-Things (IoT), where otherwise normal items such as kitchen appliances, smartphones, and even electrical meters are interconnected and can access the Internet. Since IoT devices can be accessed anywhere and have user-set behaviors, they transmit data frequently over various networking standards which can be obtained by a malicious actor. While network data is often encrypted, the patterns they construct can be used by such an adversary to infer user behavior, device behavior, or the device itself. In this work, we evaluate various traditional machine learning models for device classification using network traffic features generated from link-level flows to overcome both encryption and differences in protocols/standards. We also demonstrate the viability of the GPT 3.5 large language model (LLM) to perform the same task. Our experiments show the viability of flow-based classification across 802.11 Wi-Fi, Zigbee, and Bluetooth Low Energy devices. Furthermore, with a considerably smaller dataset, the LLM was able to identify devices with an overall accuracy of 79% through the use of prompt-tuning, and an overall accuracy of 63.73% for a larger more common dataset using fine-tuning. Compared to traditional models, the LLM closely matches the performance of the lowest-performing models and even achieves higher accuracy
than the best-performing models.
