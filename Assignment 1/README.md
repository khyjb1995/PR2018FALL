
# Pattern Recognition
## Assignment 1 Report - Extraction of Pixels of Ducks
### Tools
 - Jupyter Notebook(Python)
 - Github for Desktop
 - OpenCV Library
 - SKLearn Naïve Bayes Library
 - Numpy Library
#
### Assignment Requirements
 - An image of duck farm taken from a drone, use the Bayes classifier to extract the pixels of duck bodies from the image.
 -  Must output an image which keeps every duck-body pixel classified with classifier and replaces all nonduck-body pixels with black pixels.
#
### Flowchart of program
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/flowchart.jpg)
#
### Result & Conclusion
In this program, first time to learn how to use these library for Python. These library helps us to reduce many works on the data training, data clustering, data convert and more. This program show the result by using the simple Naïve Bayes, I using the OpenCV to read image with 3-dimension on each dot R,G,B put it in to array and using another list to label it is a part of duck feature or not. After finish that step, make an array convert to numpy array format to fitting it into Gaussian Naïve Bayes train the data. Then I using the predict function to predict each dot result and output the image with the classifier. At last I using an algorithm myself, I scan the Black Pixel of the result image by different size of the box, when the box contains the black pixel smaller than a number, I mark it as a duck, and output to Red Mark image.

#### A Part of Image (Small)
##### Recognition Image
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/count03.jpg)
##### Black Pixel of the result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count03/Blackback_Result.jpg)
##### Red Pixel of the result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count03/RedDot_Result.jpg)
##### Red Mark of the result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count03/Circle_Result.jpg)

#### A Part of Image (Medium)
##### Recognition Image
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/count02.jpg)
##### Black Pixel of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count02/Blackback_Result.jpg)
##### Red Pixel of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count02/RedDot_Result.jpg)
##### Red Mark of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count02/Circle_Result.jpg)

#### A Part of Image (Large)
##### Recognition Image
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/count04.jpg)
##### Black Pixel of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count04/Blackback_Result.jpg)
##### Red Pixel of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count04/RedDot_Result.jpg)
##### Red Mark of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_count04/Circle_Result.jpg)

#### A Part of Image (Full)
##### Recognition Image
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/full_duck.jpg)
##### Black Pixel of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_full_duck/Blackback_Result.jpg)
##### Red Pixel of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_full_duck/RedDot_Result.jpg)
##### Red Mark of the Result
![](https://github.com/khyjb1995/PR2018FALL/blob/master/Assignment%21/result_full_duck/Circle_Result.jpg)

#### Details of the Result

|  | Pixel | FileSize | Speed | Approximately |
|---|---|---|---|---|
| Small | 216x257 | 27.2KB | 0h 1min | 12 ducks |
| Medium | 1099x907 | 306KB | 0h 4min | ? ducks |
| Large | 1529x813 | 361KB | 0h 36min | ? ducks |
| Full | 5946x13816 | 8.41MB | 3h 03min | 4983 ducks |