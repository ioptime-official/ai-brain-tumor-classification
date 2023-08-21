# AI-brain-tumor-classification
# BraTum Scans -- Brain Tumor Classification using MobileNet-v2
## 1 SCOPE
Brain Tumor is one of the deadly diseases prevailing in today's world. It's timely detection is very important to start the treatment process immediately.Brain tumor classification using machine learning is a significant and rapidly evolving field with broad implications for medical diagnosis and treatment planning. As medical imaging technologies continue to advance, the amount of data generated from brain scans has grown exponentially, creating both opportunities and challenges. Machine learning techniques offer a powerful means to process and interpret this data, assisting medical professionals in accurately identifying and classifying different types of brain tumors. The scope of this brain tumor classification project is to classify the brain mri images into four classes yhat are pituitary tumor, meningioma tumor, no tumor or pituitary tumor. MobileNet V2 model is used in this project along with application of explainabled AI at the end to evaluate the model predictions more accurately. The ultimate goal of this project  is to provide clinicians with efficient and reliable tools to aid in early detection, precise diagnosis, and personalized treatment recommendations. With the potential to expedite diagnoses, minimize subjectivity, and improve patient outcomes, brain tumor classification using machine learning holds immense promise in the realm of medical image analysis and healthcare innovation.
## 2 INTRODUCTION:
Brain tumor classification project involves the classification of brain mri images into further classes on basis of feature learning using AI model.Road map of this project includes cpollection of suitable data, selection of applropriate AI for the dataset, training of model and testing it afterwards. All the details of model are provided in sections below.
## 3 PROCESS OF Brain Tumor Classification
Steps and challenges faced during the project include collection of suitable dataset, model selection of basis of it's architecture suitablility with the dataset, preprocessing of data that includes division and augmentation of data , model training, predictions and finally application of exlainable AI to get better understanding of model's working. 
<br />

![flowchart1](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/f126c22b-835f-43e7-be8c-4486ee5d3f96)
### 3.1 DATASET
In my Brain Tumor Classification project, I embarked on a comprehensive journey to construct an advanced neural network model that can effectively distinguish between different types of brain tumors. To begin, I accessed a high-quality dataset from Kaggle, containing a diverse range of brain images representing various tumor categories. Original dataset consist of two divisions testing and training sets. Each testing and training set further contain four classes  glioma_tumor, meningioma_tumor, no_tumor and pituitary_tumor. For my project I divided the data into three sets training, testing and validation in 70, 10 and 20 percent proportion respectively. 
<br />
![dataset](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/c8732fdf-a599-438c-b0b7-008727a313e6)
### 3.2 DATA PREPROCESSING:
Data preprocessing involves the steps the dataset particularly the training set undergoes before starting the training of model. Preprocessing steps done in brain tumor classification project are mentioned below;
#### 3.2.1 COMBINED AND SEGREGATED DATASETS
As in dataset brain mri scans are taken from different angles like top angle images, left angle images and back angle images. For better understanding of images classification I segregated those images for each class and created sub classes like glioma_tumor_top_Angle, mengiona_tumor_Left_Angle and so on. I applied model once on combined dataset and once on each angle dataset. 
#### 3.2.2  DATA AUGMENTATION
For segregated dataset I used data augmentations. As now I divided the already existing classes into different sub classes I faced issue of less data. To enhance data I used data augmentations. To enhance the robustness of the model, I applied data preprocessing techniques such as data augmentation like CLahe, Random Brightness, Random BrightnessandContrast.
##### 3.2.2.1 CLAHE
CLAHE stands for "Contrast Limited Adaptive Histogram Equalization." It is a computer image processing technique used to enhance the contrast and visibility of details in an image. Unlike standard histogram equalization, which spreads out the pixel intensity values across the entire range, CLAHE divides the image into smaller regions and applies histogram equalization separately to each region. This adaptive approach prevents the over-amplification of noise in areas with low contrast, leading to improved image quality. CLAHE is particularly useful for enhancing details in images with uneven lighting conditions or those containing both dark and bright regions. It finds applications in medical imaging, remote sensing, and other fields where enhancing image contrast is crucial for analysis and visualization.
![aug1](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/8eb1081f-6fb6-4da3-a04e-b3fa38437819)
<br />
##### 3.2.2.2 RANDOM BRIGHTNESS
Random brightness augmentation is a data augmentation technique commonly used in image processing and computer vision tasks. It involves adjusting the brightness of an image randomly to create variations of the original image. This technique is often applied to augment training datasets for machine learning models, helping the models become more robust and generalizable by exposing them to a wider range of lighting conditions.
![aug2](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/fd2c7360-db0e-42ed-9f14-332d53230f18)
<br />
##### 3.2.2.3 RANDOM BRIGHTNESS AND CONTRAST
Random brightness and contrast augmentation are two distinct data augmentation techniques commonly employed in image processing and computer vision tasks to enhance the diversity and quality of training data for machine learning models.By applying both random brightness and contrast augmentation, machine learning models become more resilient to changes in lighting conditions and are better equipped to recognize important features regardless of how the image is captured. These techniques contribute to reducing overfitting, enhancing generalization, and improving the model's performance on real-world data. When combined with other augmentation techniques such as rotation, scaling, and flipping, random brightness and contrast augmentation form a comprehensive strategy for creating a diverse and representative training dataset that helps build more robust and accurate models.
![aug3](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/32d8e471-31d2-405c-9806-de78f69d750a)
<br />
### 3.3 MODEL ARCHITECTURE:
MobileNet-V2 has been selected for brain tumor classifciation project because of it's efficiency and less computer sources utility.Mobilenet-V2 model has been used in this project of brain tumor classification. MobileNet v2 is a lightweight convolutional neural network (CNN) architecture that is designed for efficient computation on mobile and embedded devices. It uses depth-wise separable convolutions and residual connections to reduce the number of parameters and improve the performance of the network. MobileNet is used for feature extraction, which means it is responsible for identifying key features in the input image that can be used for object detection.
![model](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/950254ab-4b65-460e-9b22-9afa56f47d5c)
<br />
### 3.4 TRAINING LOOP:
After data augmentation training of model started. This project include four datasets which are combined dataset, top angle data set, left angle data set and back angle dataset which further have their own training, validation and testing sets.. So training has to be done for each dataset's training set  individually. Models are trained on 30 epochs. After training the models comes the step of validation. models are being validated on validation set of respective dataset. After validation models are being tested.
### 3.5 TESTING
After training and validation models are being saved and then reloaded for proper testing. Results got after testing are mentioned in next section. test accuracy should be compared with validation accuracy to interpret the working of models.
#### 3.5.1 RESULTS
##### 3.5.1.1 MODEL ON COMBINED DATASET
I trained Mobilenet-v2 model on combined dataset that contain main classes glioma_tumor, meningioma_tumor, no_tumor and pituitary_tumor. I trained the model at 30 Epoch. After I validated the model on validation set. After this I tested the model on testing set to check accuracy of model. I got the following results;
Train Loss: 0.0781 | Train Acc: 0.9755
Valid Loss: 1.0393 | Valid Acc: 0.8451
Test Accuracy: 92.97%
Test Loss: 0.3987
![cm1](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/a786497e-8835-471a-9542-10e16ceb6d0d)
##### 3.5.1.2 SEGREGATED DATASETS
###### 3.5.1.2.1 TOP_ANGLE_DATASET

