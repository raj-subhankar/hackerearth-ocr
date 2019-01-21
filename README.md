# Handwriting detection


The pipeline is composed of 3 steps:
- Detecting the handwritten area in a form 
- Detecting lines of handwritten texts 
- Recognising characters and applying a language model to correct errors. 


## Dataset:
* To use test_iam_dataset.ipynb, create credentials.json using credentials.json.example and editing the appropriate field. The username and password can be obtained from http://www.fki.inf.unibe.ch/DBs/iamDB/iLogin/index.php.

Obtain the original forms from the IAM dataset and plot the results. Randomly select 4 images for analysis.


## Paragraph segmentation
Given the image of a form in the IAM dataset, predict a bounding box of the handwriten component.

## Image processing
Crop the handwriting component out of the original IAM form.

## Line/word segmentation
Given a form with only handwritten text, predict a bounding box for each word.

## Word to line image processing
Algorithm to sort then group all words within a line together.

## Handwriting recognition
Given each line of text, predict a string of the handwritten text.

## Appendix


##### Results

![](https://cdn-images-1.medium.com/max/800/1*HEb82jJp93I0EFgYlJhfAw.png) 


##### Results

![](https://cdn-images-1.medium.com/max/1000/1*JJGwLXJL-bV7zsfrfw84ew.png)


