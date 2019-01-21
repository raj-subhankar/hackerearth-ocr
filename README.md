# Handwriting detection

The pipeline is composed of 3 steps:
- Detecting the handwritten area in a form 
- Detecting lines of handwritten texts 
- Recognising characters and applying a language model to correct errors. 

![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/pipeline.png)


## Dataset:
* To use test_iam_dataset.ipynb, create credentials.json using credentials.json.example and editing the appropriate field. The username and password can be obtained from http://www.fki.inf.unibe.ch/DBs/iamDB/iLogin/index.php.

Randomly select 4 images from the data set.
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-1.jpg)

## Paragraph segmentation
Given the image of a form in the IAM dataset, predict a bounding box of the handwriten component.
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-2.jpg)

## Image processing
Crop the handwriting component out of the original IAM form.
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-3.jpg)

## Line/word segmentation
Given a form with only handwritten text, predict a bounding box for each word.
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-4.jpg)

## Word to line image processing
Algorithm to sort then group all words within a line together.
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-5.jpg)

## Handwriting recognition
Given each line of text, predict a string of the handwritten text.
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-6.jpg)
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-7.jpg)
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-8.jpg)
![](https://github.com/raj-subhankar/hackerearth-ocr/blob/master/images/ocr-9.jpg)


