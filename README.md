# Machine Learning Project
## Rice type classification: Jasmine and Gonen


## Knime Workflow
2021/22 Machine Learning Project @ University of Milano-Bicocca

### Team
* Aurora Cerabolini
* Kevin Capano
* Federico Pirola
* Corinna Strada

## Abstract
In order to ensure an effective and fruitful rice cultivation process, it is essential that the seeds belonging to a specific species are provided to farmers.  <br>
In this regard, Machine Learning models were built with the aim of distinguishing between two species of rice (Jasmine and Gonen) in the most effective way possible. In addition, it was researched which of the two was the simplest type of rice to identify.  <br>
The results may be useful, in the future, to ensure a more effective and faster selection of seeds compared to the selection method used today.

## Introduction 
Rice is one of the most consumed products in the world. Its cultivation begins with the selection of seeds, which are planted after suitable soil preparation. <br>
<br>
For the entire life cycle of the plant, it is essential to control the management of water levels and nutrient absorption, determining, if necessary, the use of fertilizers. At the right time, we move on to the harvest and any post-harvest treatments.<br>
<br>
The presence of problems relating to the seed selection step could delay or stop the entire production cycle: in particular, a fundamental step in this case is to ensure that there is no contamination or mix between different categories of rice.<br>
<br>
In order for only one type of rice to be supplied to the growers, selection processes are carried out. However, these processes are manual and are based on a small number of samples. The results, therefore, are often extremely unreliable. For this reason, the use of automated rice classification methods is recommended to ensure fast and reliable categorization.<br>
<br>
In the dataset used for this project, two different categories of rice are considered: “Jasmine” and “Gonen”.<br>
<br>
Jasmine rice originates in Thailand and is characterized by a very high level of appearance, quality and aroma. Gonen rice, on the other hand, comes from Turkey and is the third rice in the world in terms of productivity and, like all other Turkish rice seed varieties, is characterized by high germination rates.<br>
<br>
The primary goal, in this case, is to determine with the greatest possible success the type of rice grain based on the variables identified in the dataset, thus identifying the best classification model.<br>
<br>
The secondary goal, on the other hand, is to establish which of the two varieties of rice is more easily identifiable.<br>
<br>
The initial part of this article is dedicated to the description of the dataset and a preliminary analysis of the information contained within it. After that, there is a presentation of the developed classification models, the best hyper-parameters chosen, and the performance measures used.<br>
<br>
The final part of the work is therefore dedicated to the description of the analyses carried out and the results achieved, based on the two different research goals.

## Dataset
There are no missing values in the dataset and all the variables, with the exception of the id and the target, are numeric.
The variables considered are 12 and were extracted from high-definition images of the beans:
* Id: identification code of each instance. This variable was not taken into account for the analyzes.
* Area: number of pixels in the region generated by the grain.
* Eccentricity: this measure presupposes the consideration of the grain of rice as an ellipse. In particular, it considers the relationship between the foci of the ellipse having the same second moments of the region generated by the grain and the length of its major axis.
* MajorAxisLength: length of the major axis of the ellipse which has the same second moments as the grain region.
* MinorAxisLength: length of the minor axis of the ellipse which has the same second moments as the grain region.
* ConvexArea: consists of the number of pixels that belong to the convex image, that is a binary image that contains all the pixels within the convex envelope. It is generated by the intersection of all subsets that contain a certain vector space.
* EquivDiameter: is the diameter of a circle that has the same area as that of the region of the grain of rice.
* Extent: returns the ratio between the number of pixels relating to the grain region and those of the bounding box5, i.e. the box with the smallest size in which the element can be contained.
* Perimeter: count of the number of pixels present on the outline of the grain of rice.
* Roundness: it is relative to the roundness of the grain of rice.
* AspectRation: is the ratio between the major axis and the minor axis of the ellipse that represents the grain.
* Class: is the target variable. It is binary, where 0 represents Gonen rice (45.1%), while 1 represents Jasmine (54.9%): the distribution is equal between the two classes, so the dataset is not unbalanced.


<u>*Please read the report for more details!*</u>

## License
[MIT](https://choosealicense.com/licenses/mit/)
demo vedio:https://www.loom.com/share/a0f32e73a1ff44f9827e4040bd0633be?sid=c2fef9f8-2566-46ed-af70-9a21bc746a6e
