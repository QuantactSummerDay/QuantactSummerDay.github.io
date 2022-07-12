---
name: "Vision Systems for Finance: LOB Data Augmentation"
speakers:
  - Timothy C DeLise
categories:
  - Talk
---

## "Vision Systems for Finance: LOB Data Augmentation"

#### Timothy C DeLise

CNNs are good at representation learning on images in ways comparable to humans. The appeal of projects like DeepLOB, which uses CNNs in a similar fashion as image recognition problems, is to allow the model to discover representations from the data which have spatial aspects. To this end, the standard way of constructing 2-dimensional matrices, or images, from order book data arranges time along the y-axis, with the x-axis containing columns which describe the levels of the order book, from 1 to 10. While this is one way of presenting order book data as an image, it doesn't create a coherent picture to humans. We think the advertised power of CNNs is not being fully exploited by the current data representation. This paper presents a data augmentation technique which rearranges each data point (image) onto the pixels, which act as a price grid, where bid and ask prices are defined by their relative positions in the image. The bid and ask sizes are thus the values contained at each pixel creating an understandable image. This simple technique increases baseline out-of-sample accuracy scores by 25% as a drop-in replacement for original FI-2010 data representation, using original DeepLOB code. We show this trend in several practical applications and intend to set a new high-water mark for this experiment.

