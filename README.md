&nbsp;
# Project 1: Alphanumeric CAPTCHA Solver
[Article Link](https://github.com/Ceudan/Alphanumeric-CAPTCHA-Solver)
 [Video Link](https://drive.google.com/file/d/1td802b0Awh8pfEoDKK6pBHAdh1UC6BsB/view?usp=sharing)

Led a team of 4 to independantly design from scratch a multi-staged software that decodes alphanumeric CAPTCHA images. Motivation was a course final project. Input consists 5 character CAPTCHAs disguised with various levels of rotational, distance, colour and overlapping distortions along with image noise. Output is a 5 character prediction of the sequence.
![Image of a CAPTCHA and the software's predicted output](images/output.png) 
\
The program consists of 3 main steps: preprocessing using computer vision libraries to eliminate noise, character segmentation using object recognition to localize individual characters, and character classification using a convolutional neural network followed by several fully connected layers. We succesfully achieved an accuracy of 71% per entire CAPTCHA image and 91% per individual character. These accuracies are high given that CAPTCHAs are designed not to be bypassed by computer software. 
\
\
Skills Learned: computer vision libraries, image processing, deep-learning, generating custom train data

# Project 2: Matching Road Sections between Databases
[Article Link](https://github.com/Ceudan/Match-Roads-Between-Databases)

I independantly created a program without guidance to match sections across databases using geospatial information. This was one of the many tasks I recieved at the University of Toronto Transportation Research Institute. Hurdles included:
- over 100,000 road sections per database (strong time complexity requirements)
- close proximity does not gaurentee correct match
- geographic coordinates carry up to 10 metres of uncertainty



![Visualization of road sections in Database 1](images/ex1_HERE.png) ![Visualization of road sections in Database 2](images/ex1_aimsun.png) ![Visualization of road sections in Database 2](images/ex1_match_background.png) 


Achieved an accuracy of 94% when excluding abnormal sections. Accuracy is highly dynamic since adjustable thresholds can tradeoff quantity with quality. It was succesfully used to match sections from an Aimsun traffic simulation covering the GTHA, with HERE Technologies' observed traffic information.
\
\
Skills Learned: GeoPandas, GIS, shapefiles, shapely visualizations, matrix/array operational time dependancies
