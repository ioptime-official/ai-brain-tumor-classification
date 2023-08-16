# AI-brain-tumor-classification
# BraTum Scans -- Brain Tumor Classification using MobileNet-v2
## SCOPE--INTRODUCTION
Brain Tumor is one of the deadly diseases prevailing in today's world. It's timely detection is very important to start the treatment process immediately.Brain tumor classification using machine learning is a significant and rapidly evolving field with broad implications for medical diagnosis and treatment planning. As medical imaging technologies continue to advance, the amount of data generated from brain scans has grown exponentially, creating both opportunities and challenges. Machine learning techniques offer a powerful means to process and interpret this data, assisting medical professionals in accurately identifying and classifying different types of brain tumors. The scope of brain tumor classification encompasses various modalities, including MRI, CT scans, and PET scans, each providing unique insights into the tumor's characteristics. By training models on large datasets containing labeled tumor images, machine learning algorithms can learn intricate patterns and features indicative of different tumor types, grades, and locations. The ultimate goal is to provide clinicians with efficient and reliable tools to aid in early detection, precise diagnosis, and personalized treatment recommendations. With the potential to expedite diagnoses, minimize subjectivity, and improve patient outcomes, brain tumor classification using machine learning holds immense promise in the realm of medical image analysis and healthcare innovation.
## PROCESS OF Brain Tumor Classification
<br />
![flowchart1](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/b84f2654-5d7e-4db0-ab83-bb0ec2490824)
<br />
In my Brain Tumor Classification project(BraTum Scans), I embarked on a comprehensive journey to construct an advanced neural network model that can effectively distinguish between different types of brain tumors. To begin, I accessed a high-quality dataset from Kaggle, containing a diverse range of brain images representing various tumor categories. To enhance the robustness of the model, I applied data preprocessing techniques such as data augmentation like CLahe, Random Brightness, Random BrightnessandContrast. As example is shown below;
<br />

![CLAHE](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/8f25b81e-f4ac-4f53-a4ce-84035e237657)
<br />
I opted for the MobileNetV2 architecture, known for its efficiency and accuracy in image classification tasks. After constructing the model architecture, I undertook a rigorous training phase using the preprocessed dataset.Following training, I  evaluated the model's performance using dedicated validation datasets. By analyzing metrics such as accuracy, precision, recall, and F1-score, I gained insights into the model's strengths and weaknesses. Notably, the model showcased impressive accuracy in classifying different types of brain tumors, showcasing its potential clinical significance.To delve further into the inner workings of the model and its decision-making process, I integrated Grad-CAM (Gradient-weighted Class Activation Mapping). This cutting-edge technique allowed me to visualize which areas of the brain images were crucial in influencing the model's predictions. The overlay of these activation maps on the original images provided a form of "explainable AI," giving valuable insights into the model's decision rationale and aiding medical practitioners in understanding its decisions.Example image is shown below;
<br />

![eai2](https://github.com/ioptime-official/ai-brain-tumor-classification/assets/138657622/960dd473-81d8-4f2c-b1d7-639cf3408019)

<br />
