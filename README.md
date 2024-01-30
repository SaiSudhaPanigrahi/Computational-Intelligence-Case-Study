
***In partial fulfilment of the requirements for the COURSE - 15CSE338(Computational Intelligence)***

1. **Abstract** 

Content-based image retrieval, also known as query by image content [(QBIC)](https://en.wikipedia.org/wiki/Content-based_image_retrieval#QBIC) and content-based visual information retrieval (CBVIR), is the application of[ computer vision ](https://en.wikipedia.org/wiki/Computer_vision)techniques to the[ image retrieval ](https://en.wikipedia.org/wiki/Image_retrieval)problem, that is, the problem of searching for[ digital images ](https://en.wikipedia.org/wiki/Digital_image)in large[ databases.](https://en.wikipedia.org/wiki/Database)In the current era of digital communication, the use of digital images has increased for expressing, sharing and interpreting information. While working with digital images, quite often it is necessary to search for a specific image for a particular situation based on the visual contents of the image. This task looks easy if you are dealing with tens of images but it gets more difficult when the number of images goes from tens to hundreds and thousands, and the same content-based searching task becomes extremely complex when the number of images is in the millions. To deal with the situation, some intelligent way of content-based searching is required to fulfill the searching request with right visual contents in a reasonable amount of time. There are some really smart techniques proposed by researchers for efficient and robust content-based image retrieval. In this research, the aim is to highlight the efforts of researchers who conducted some brilliant work and to provide a[ proof of concept ](https://www.sciencedirect.com/topics/engineering/proof-of-concept)for intelligent content-based image retrieval techniques.

2. **Objective / Problem Definition** 

To use the technology of computational intelligence to search and display the images based on the text query given by the user. We propose to investigate efficient methods apart from the traditional methods for easy access and convenience of images in a database. Some of day to day applications are Google image search, e-commerce websites that search for products and simple querying of images from large databases.

3. **Introduction** 

Database technologies for pictorial applications were discussed for the first time in that era and the researchers got attraction for this domain since then. Former image retrieval techniques were not that intelligent and sophisticated and they were not able to search for images based on its visual features instead those techniques were based on text-based metadata of images. All images stored in the database were first tagged with the metadata and then images were searched based on the image  metadata.  Text-based  image  retrieval  methods  were  used  for  conventional  database applications. They were used with a lot of business applications and purposes but increasing usage and volume of digital images created performance and accuracy issues for text-based image retrieval methods. New methods proposed for image retrieval considered color, texture, and shapes of objects in an image. 

4. **Literature Survey ![](Aspose.Words.327d7396-30f0-4434-8142-73c6787c2caa.002.png)**

a)G. Raju, Madhu S. Nair, 
A fast and efficient color image enhancement method based on fuzzy-logic and histogram, 
AEU - International Journal of Electronics and Communications, 
Volume 68, Issue 3, 
2014 

A new fuzzy logic and[ histogram ](https://www.sciencedirect.com/topics/mathematics/histograms)based algorithm for enhancing low contrast color images has been proposed here. The method is computationally fast compared to conventional and other advanced enhancement techniques. It is based on two important parameters *M* and *K*, where *M* is the average intensity value of the image, calculated from the histogram and *K* is the contrast intensification parameter. The given[ RGB image ](https://www.sciencedirect.com/topics/computer-science/rgb-image)is converted into HSV color space to preserve the chromatic information contained in the original image. To enhance the image, only the V component is stretched under the control of the parameters *M* and *K*. The proposed method has been compared with conventional contrast enhancement techniques as well as with advanced algorithms. All the above techniques were based on the principle of transforming the skewed histogram of the original image into a uniform histogram.The performance of the different contrast enhancement algorithms are evaluated based on the visual quality,and the computational time.The inter comparison of different techniques was carried out on different low contrast color images. Based on the performance analysis, we advocate that our proposed Fuzzy Logic method is well suited for contrast enhancement of low contrast color images. 

b) Zhou M., Tanimura Y., Nakada H. (2020) One-Shot Learning Using Triplet Network with kNN Classifier. In: Ohsawa Y. et al. (eds) Advances in Artificial Intelligence. JSAI 2019. Advances in Intelligent Systems and Computing, vol 1128. Springer, Cham 

One-shot Learning using Triplet Network with kNN classifier (2019) 

In this paperwork, they described  a Triplet Network model, inspired by the Siamese Network based on distance metric, which can be used for one-shot learning. They proposed a triplet network with a kNN classifier for the problem of one-shot learning, in which they predict the query images by giving a single example of each class. This triplet network learns a mapping from sample images to the Euclidean space.For this,they used the embeddings of training points trained on the kNN classifier and predicted the label with the embedding of testing points by the classifier. A significant improvement can be obtained by the effectiveness of data augmentation. Of the 3 approaches tested, best results were achieved by augmenting the initial dataset with Triplet Network model. Input triplets for Triplet Network were generated in two ways. One kind of triplets was produced by the augmented dataset, while another one was created by the initial dataset which was not augmented. For the first type,  one sample was selected(used as the anchor ![](Aspose.Words.327d7396-30f0-4434-8142-73c6787c2caa.003.png)instance) from the dataset, then chose another one (used as the positive instance) from the same label. Then the other sample was randomly obtained (used as the negative instance) from any other label. Finally, they concatenated them as a triplet pair. However, for the other type created by the initial dataset, they used the same image as the positive instance to overcome the limitation of lack of samples. 

5. **Dataset Description**

The dataset consists of google images of around 50 animals. Each animal set contains roughly 500 images. Data captured are the image, title, and caption for the image. 


6. **Tools Description**
- Packages used: Keras, PIL, Image, Sklearn, Numpy, Pandas, Tensorflow 
- Model used:VGG16, Fuzzy algorithms, Genetic algorithms 
- Activation function used: LeakyRelu,SoftMax, Relu 
- Language: Python 3 

10. **Comparison/ Performance Analysis** 

While in the contrast experiment on CNN model, data augmentation resulted in accuracy of 20.8%. However, the experiment on the Triplet model with initial dataset resulted in accuracy of 9.8%, where almost all the data trained with one sample cannot be recognized. This study therefore indicates that the benefits gained from data augmentation may work well on one-shot learning problems. Although the experiment demonstrates a great improvement, the results are subject to certain limitations. Also, the experiments were unable to explore approaches that work on other much larger and complex datasets. For fuzzy logic and genetic algorithm, the parameters were fine tuned to achieve more accuracy as seen in our results. 

11. **Conclusion** 

In this case study, we have experimented with models such as Conventional Neural Networks and Triplet Neural Networks for the text query of images. We did this in order to compare the performance of traditional neural networks and an improvised one. Traditional neural net takes in text queries passed after minimal preprocessing and resultant images are generated. In order to improve the image quality and validation of image search we have used fuzzy and triple neural nets. We have used a fuzzy algorithm for the image enhancement process. We have used a Genetic algorithm for producing a set of child images from a target image. In the process we have tried fine tuning the parameters and have come up with enhanced results. 

12. **References And Related Articles** 
- Reed, Scott, Zeynep  Akata, Xinchen Yan, Lajanugen  Logeswaran, Bernt Schiele, and Honglak Lee. "Generative adversarial text to image synthesis." arXiv preprint arXiv:1605.05396 (2016). 
- G. Raju, Madhu S. Nair, A fast and efficient color image enhancement method based  on  fuzzy-logic  and  histogram,  AEU  -  International  Journal  of Electronics and Communications, Volume 68, Issue 3, 2014 
- Zhou M., Tanimura Y., Nakada H. (2020) One-Shot Learning Using Triplet Network  with  kNN  Classifier.  In:  Ohsawa  Y.  et  al.  (eds)  Advances  in Artificial  Intelligence.  JSAI  2019.  Advances  in  Intelligent  Systems  and Computing, vol 1128. Springer, Cham. https://doi.org/10.1007/978-3-030- 39878-1\_21 
- [https://missinglink.ai/guides/computer-vision/neural-networks-image- recognition-methods-best-practices-applications/ ](https://missinglink.ai/guides/computer-vision/neural-networks-image-recognition-methods-best-practices-applications/)
- [https://www.sciencedirect.com/science/article/pii/S1665642314716098 ](https://www.sciencedirect.com/science/article/pii/S1665642314716098)
- [https://www.researchgate.net/publication/303626451_Query-by- Example_Image_Retrieval_in_Microsoft_SQL_Server ](https://www.researchgate.net/publication/303626451_Query-by-Example_Image_Retrieval_in_Microsoft_SQL_Server)
- [https://link.springer.com/chapter/10.1007/11840930_3 ](https://link.springer.com/chapter/10.1007/11840930_3)

For implementation details and complete report, please view: Report_group_6_Text Query of Images.pdf 
