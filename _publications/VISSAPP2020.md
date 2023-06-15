---
title: "Mask-guided Image Classification with Siamese Networks"
collection: publications
permalink: /publication/VISSAPP2020
excerpt: ' '
date: 2020-03-01
venue: 'International Joint Conference on Computer Vision, Imaging and Computer Graphics Theory and Applications'
paperurl: ' '
citation: 'Alqasir Hiba, Damien Muselet, and Christophe Ducottet. &quot;Mask-guided Image Classification with Siamese Networks.&quot; <i>International Conference on Computer Vision Theory and Applications</i>. 2020.'
---
This paper deals with a CNN-based image classification task where the class of each image depends on a small detail in the image. Our original idea consists in providing a binary mask to the network so that it knows where is located the important information. This mask as well as the color image are provided as inputs to a siamese network. A contrastive loss function controls the projection of the network outputs in an embedding space enforcing the extraction of image features at the location proposed by the mask. This solution is tested on a real application whose aim is to secure the boarding on ski chairlifts by checking if the safety bar of the carrier is open or closed. Each chairlift has its own safety bar masks (open and close) and we propose to exploit this additional data to help the image classification between close or open safety bar. We show that the use of a siamese network allows to learn a single model that performs very well on 20 different skilifts.

[Download paper here](https://hal-ujm.archives-ouvertes.fr/ujm-02899908/document)


