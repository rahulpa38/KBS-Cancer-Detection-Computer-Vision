# FinalProject
Final Project

1)  Research question:   Skin cancer is the most common human malignancy, is primarily diagnosed visually, beginning with an initial clinical screening and followed potentially by dermoscopic analysis, a biopsy and histopathological examination. Automated classification of skin lesions using images is a challenging task owing to the fine-grained variability in the appearance of skin lesions. This the HAM10000 ("Human Against Machine with 10000 training images") dataset.It consists of 10015 dermatoscopicimages which are released as a training set for academic machine learning purposes and are publiclyavailable through the ISIC archive. This benchmark dataset can be used for machine learning and for comparisons with human experts.

2)  Domain and Data: 
    Source of Data - https://www.kaggle.com/kmader/skin-cancer-mnist-ham10000
    Domain - Health, Image Data
    Size of Data : HAM10000_matadata.csv - This file has 7 columns with 10015 rows. This has information about patient details.
          In addition to this file we have 10015 images of various skin cancer patients. We also have hmnist*.csv files which has pixel           information.

    Preprocessing: We have removed nulls from the age column and replaced it with the mean.
                   We added 3 new columns in the table for better understanding of the data.
                   1) With dx - Cancer Type
                   2) With dx-  Cancer Id
                   3) Age Range - Age - For Plotting age Data

         
       ![image](https://github.com/Group13-KBS/FinalProject/blob/master/Tablesummary.JPG)
       
    User Dashboard:
    
    The below dashboard represents count of each age range
    ![image](https://github.com/Group13-KBS/FinalProject/blob/master/EDA%20images/Image1.JPG)
    
    The below dashboard represents body part affected based on gender
    ![image](https://github.com/Group13-KBS/FinalProject/blob/master/EDA%20images/image2.JPG)
    
    The below dashboard represents pie chart of diagnostics type
    ![image](https://github.com/Group13-KBS/FinalProject/blob/master/EDA%20images/image3.JPG)
    
    The below dashboard represents cancer type and the their counts
    ![image](https://github.com/Group13-KBS/FinalProject/blob/master/EDA%20images/image4.png)
    
    Internal Dashboard:
    
    Data Scientist or Data Engineer? Please download the jupyter notebook [here](https://github.com/Group13-KBS/FinalProject/blob/master/Notebooks/Untitled.ipynb) to access a more sophisticated dashboard on the dataset.
    
    
    
    
    
       
      

      c)  tentative plan for analysis on GCP

           1)  EDA and Preprocessing:
               a. We will plot graphs based on the skin lesion type.
               b. Plotting of Technical Validation field (ground truth) which is dx_type to see the distribution of its 4 categories
               c. Plotting the distribution of localization field.
               d. Also analyze patient informationd details.
               We can work on the preprocessed data and implement the recommendation algorithm.

           2)  Dashboard for User group, Dashboard for Data Engineers:
               We will plan to represent graphically the different types of skin lesions based on images. Also dashboards for the skin images occured based on various factors.
           3)  GCP further processing :
               We will use classiffication algorithms(CNN) to predict the skin lesion.

           4)  Evaluation of results :
               We will be evaluating our result by categorical cross entropy. The smaller the value more accurate result will be. We will try to implement and tune the algorithm to get the least categorical cross entropy.          

           5)  Steps for production model :
               We will load our data in Classification model and train our model with partial data and check categorical cross entropy. After training , we will be testing our model and prepare the model for Production data.

           6)  Final Dashboard for User Group :
               Finally, we can recommend users the chances of skin cancer based on the images . Our model can be used for machine learning and for comparisons with human experts.
      
      Research Citation:
      
      1. Advanced Deep Learning Methodologies for Skin Cancer Classification in Prodromal Stages
         By Muhammad Ali Farooq, Asma Khatoon, Viktor Varkarakis , Peter Corcoran
         
         In this paper, the researchers have designed a Computer-Aided Diagnosis (CAD) system which is a type of digitized platform              based on advanced computer vision, deep learning, and pattern recognition techniques for skin cancer classification. For the            proposed study we have designed a CAD system for skin cancer classification by utilizing advanced deep neural networks. this            system was created because performing dermoscopy using conventional methods may lower down the diagnostic accuracy which can            lead to more chances of errors. These errors are generally caused by the complexity of lesion structures and the subjectivity            of visual interpretations 
      
      2. Automatic Melanoma Detection Using Multi-Stage Neural Networks
         By Nikhil Cheerla, Debbie Frazier
         
         This paper discusses about a system that uses enhanced image processing to segment the images without manual intervention. From          the segmented image, it extracts a comprehensive set of features using new and improved techniques. The features were fed                automatically to a multistage neural network classifier which achieved greater than 97% sensitivity and greater than 93%                specificity. The trained system was tested with lesion images found online and it was able to achieve similar sensitivity.              Finally, a new approach that will simplify the entire diagnosis process is discussed. This approach uses Dermlite® DL1                  dermatoscope that can be attached to the iPhone. After taking the lesion image with a dermatoscope attached iPhone, the                  physician gets the diagnosis with a few simple clicks. This system could have widespread ramifications on melanoma diagnosis.            It achieves higher sensitivity than previous research and provides an easy to use iPhone based app to detect melanoma in early          stages without the need for biopsy.
         
      3. Decision Support System for Skin Cancer Diagnosis
         By Karol Przystalski ,Leszek Nowak ,Maciej Ogorzałek ,Grzegorz Surówka
         
         This paper proposes decision support system based on semantic analysis method for dermatoscopic images of malignant melanoma            cases. Further the system uses automatic classification using two approaches, namely the radial basis function kernels in                artificial neural networks and four kernels (linear, polynomial, radial and sigmoid based) for support vector machines. In the          analysis process all images are segmented into semantic objects containing various textures, shapes and colors.


