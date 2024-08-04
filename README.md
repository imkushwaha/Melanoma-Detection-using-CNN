# Melanoma Detection using CNN
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution which can evaluate images and alert the dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information

### Background of the Project
The project focuses on developing a convolutional neural network (CNN) model to accurately detect melanoma, a type of skin cancer. Melanoma is one of the deadliest forms of skin cancer, responsible for 75% of skin cancer-related deaths. Early detection is crucial for effective treatment and can significantly improve survival rates. By leveraging deep learning techniques, the project aims to create a tool that can assist dermatologists in identifying melanoma from skin lesion images, reducing the manual effort and potential for human error in diagnosis.

### Business Problem
The primary business problem addressed by this project is the need for efficient and accurate detection of melanoma. Traditional methods of diagnosing skin cancer involve time-consuming and subjective visual inspections by dermatologists. This project seeks to automate the detection process using a CNN-based model, which can quickly and accurately evaluate images for the presence of melanoma. This automation has the potential to:
- Reduce the workload of dermatologists.
- Increase the accuracy and consistency of diagnoses.
- Enable early detection and treatment, potentially saving lives.
- Lower healthcare costs by reducing the need for invasive biopsies and other diagnostic procedures.

### Dataset
The dataset used for this project consists of 2,357 images of various malignant and benign oncological diseases. These images were sourced from the International Skin Imaging Collaboration (ISIC). The images are classified into the following categories:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

The images are distributed relatively evenly across these categories, with a slight dominance of melanoma and nevus images. This diverse dataset enables the model to learn and differentiate between multiple types of skin lesions, improving its ability to detect melanoma accurately.


## Conclusions

1. **Effective Data Augmentation Strategy:**
Initial experiments with a normal CNN resulted in low training and validation accuracy (20.25% and 17.89% respectively). This indicated overfitting and a need for better data handling. Implementing data augmentation significantly improved the model's performance, demonstrating that data augmentation is crucial for enhancing model robustness and preventing overfitting.

2. **Improvement with Augmented CNN Model:**
By applying data augmentation techniques, the CNN model's performance improved, achieving 42.80% training accuracy and 42.28% validation accuracy. While this showed that the model no longer overfitted, the overall accuracy was still not satisfactory, highlighting the importance of further improving the dataset quality and balance.

3. **Impact of Class Balancing:**
Balancing the dataset led to substantial improvements, with the CNN model achieving 89.6% training accuracy and 88.3% validation accuracy. This demonstrates that a balanced dataset is critical for training effective machine learning models, particularly in multi-class classification tasks involving imbalanced data.

4. **Best Model for Detecting Melanoma:**
Among the models tested, the CNN model with the balanced dataset provided the best performance, striking a good balance between high accuracy and generalization. This model proved to be the most effective in detecting melanoma, as it did not overfit or underfit and provided high accuracy on both training and validation datasets.

5. **Potential for Further Improvement:**
While 20 epochs were used for training, increasing the number of epochs might lead to further improvements in model accuracy. Longer training times can allow the model to better learn from the data, potentially enhancing its performance.


## Technologies Used
- Python - version 3.12
- Tensorflow - version 2.13.1
- Augmentor - version 0.2.12
- Pandas - version 2.2.0
- Numpy - version 1.26.4
- Seaborn - version 0.13.2
- Matplotlib - version 3.8.3


## Acknowledgements
- This Melanoma Detection Project is a part of my assignment for Post Graduate Diploma Degree in AI & ML at IIIT-Bangalore

## Contact
Created by [https://github.com/imkushwaha/] - feel free to contact me!
