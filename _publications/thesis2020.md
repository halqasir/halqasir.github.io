---
title: "Deep Learning for Chairlift Scene Analysis: Boosting Generalization in Multi-Domain Context"
collection: publications
permalink: /publication/thesis2020
excerpt: ' '
date: 2020-12-17
venue: ' '
paperurl: ' '
citation: 'Hiba Alqasir. &quot;Deep Learning for Chairlift Scene Analysis: Boosting Generalization in Multi-Domain
Context. Signal and Image Processing.&quot; Université de Lyon, 2020. English.'
---
A dissertation submitted in partial fulfillment of the requirements for the degree of Doctor of Philosophy.

Supervisors:
- Christophe Ducottet
- Damien Muselet

Reporters:
- Nicolas THOME       
- Joost VAN DE WEIJER

Keywords:
Deep learning . Chairlift safety . Generalization . Multi-domain . Object deletion . Image classification . Domain adaptation . Siamese Networks .


This thesis presents our work on chairlift safety using deep learning techniques as part of \textsc{Mivao} project, which aims to develop a computer vision system that acquires images of the chairlift boarding station, analyzes the crucial elements, and detects dangerous situations. 
In this scenario, different chairlifts spread over different ski resorts, with a high diversity of acquisition conditions and geometries; thus, each chairlift is considered a domain. When the system is installed for a new chairlift, the objective is to perform an accurate and reliable scene analysis, given the lack of labeled data on this new domain (chairlift).

In this context, we mainly concentrate on the chairlift safety bar and propose to classify each image into two categories, depending on whether the safety bar is closed (safe) or open (unsafe). Thus, it is an image classification problem with three specific features: (i) the image category depends on a small detail (the safety bar) in a cluttered background, (ii) manual annotations are not easy to obtain, (iii) a classifier trained on some chairlifts should provide good results on a new one (generalization). To guide the classifier towards the important regions of the images, we have proposed two solutions: object detection and Siamese networks. Furthermore, we analyzed the generalization property of these two approaches. 

Object detection is a solution that allows guiding the model towards the crucial regions of the image. At test time, we can use it as a classification model by ignoring the location of the detected instances. In this thesis, we show that such an approach helps increase the classification accuracy for our specific problem compared to a classical classification network. The main weakness is the need for bounding box annotations to train the model. Thus, we have proposed to automatically create bounding box annotations by exploiting the results of an existing algorithm based on hand-crafted features. Then, since the safety bar geometry varies across chairlifts, we have proposed an original unsupervised domain adaptation step designed for object detection.

The second solution we have proposed to guide the classification model is to insert shape priors in the model using a Siamese network. The idea consists in providing pairs of images to the network, one colored image of the chairlift and one binary mask representing the safety bar. This solution requires only two masks for each chairlift, which we could obtain easily. If the safety bar in the colored image and binary mask are both open or both closed, we enforce the network to extract similar features from the image and the mask, while when the safety bar is open (resp. closed) in the colored image and closed (resp. open) in the binary mask, the features have to be different. This approach forces the network to concentrate on the safety bar in the image while ignoring the background. Furthermore, we show that specific virtual masks boost the generalization property of the network for new unseen chairlifts without requiring any images from these chairlifts.

Our solutions are motivated by the need to minimize human annotation efforts while improving the accuracy of the chairlift safety problem.  However, these contributions are not necessarily limited to this specific application context, and they may be applied to other problems in a multi-domain context.



[Download paper here](https://tel.archives-ouvertes.fr/tel-03324255/document)


