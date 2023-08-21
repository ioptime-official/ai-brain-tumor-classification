# AI-brain-tumor-classification
# BraTum Scans -- Brain Tumor Classification using MobileNet-v2
## SCOPE
Brain Tumor is one of the deadly diseases prevailing in today's world. It's timely detection is very important to start the treatment process immediately.Brain tumor classification using machine learning is a significant and rapidly evolving field with broad implications for medical diagnosis and treatment planning. As medical imaging technologies continue to advance, the amount of data generated from brain scans has grown exponentially, creating both opportunities and challenges. Machine learning techniques offer a powerful means to process and interpret this data, assisting medical professionals in accurately identifying and classifying different types of brain tumors. The scope of this brain tumor classification project is to classify the brain mri images into four classes yhat are pituitary tumor, meningioma tumor, no tumor or pituitary tumor. MobileNet V2 model is used in this project along with application of explainabled AI at the end to evaluate the model predictions more accurately. The ultimate goal of this project  is to provide clinicians with efficient and reliable tools to aid in early detection, precise diagnosis, and personalized treatment recommendations. With the potential to expedite diagnoses, minimize subjectivity, and improve patient outcomes, brain tumor classification using machine learning holds immense promise in the realm of medical image analysis and healthcare innovation.
## INTRODUCTION:
Brain tumor classification project involves the classification of brain mri images into further classes on basis of feature learning using AI model.Road map of this project includes cpollection of suitable data, selection of applropriate AI for the dataset, training of model and testing it afterwards. All the details of model are provided in sections below.
## PROCESS OF Brain Tumor Classification
Steps and challenges faced during the project include collection of suitable dataset, model selection of basis of it's architecture suitablility with the dataset, preprocessing of data that includes division and augmentation of data , model training, predictions and finally application of exlainable AI to get better understanding of model's working. 
<br />

![flowchart1](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/f126c22b-835f-43e7-be8c-4486ee5d3f96)


In my Brain Tumor Classification project(BraTum Scans), I embarked on a comprehensive journey to construct an advanced neural network model that can effectively distinguish between different types of brain tumors. To begin, I accessed a high-quality dataset from Kaggle, containing a diverse range of brain images representing various tumor categories. To enhance the robustness of the model, I applied data preprocessing techniques such as data augmentation like CLahe, Random Brightness, Random BrightnessandContrast. As example is shown below;
<br />

![Rb](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/338274db-f6e6-48e8-82bc-69d1aa037552)

<br />
I opted for the MobileNetV2 architecture, known for its efficiency and accuracy in image classification tasks. After constructing the model architecture, I undertook a rigorous training phase using the preprocessed dataset.Following training, I  evaluated the model's performance using dedicated validation datasets. By analyzing metrics such as accuracy, precision, recall, and F1-score, I gained insights into the model's strengths and weaknesses. Notably, the model showcased impressive accuracy in classifying different types of brain tumors, showcasing its potential clinical significance.To delve further into the inner workings of the model and its decision-making process, I integrated Grad-CAM (Gradient-weighted Class Activation Mapping). This cutting-edge technique allowed me to visualize which areas of the brain images were crucial in influencing the model's predictions. The overlay of these activation maps on the original images provided a form of "explainable AI," giving valuable insights into the model's decision rationale and aiding medical practitioners in understanding its decisions.Example image is shown below;
<br />

![eai2](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/960dd473-81d8-4f2c-b1d7-639cf3408019)

<br />
