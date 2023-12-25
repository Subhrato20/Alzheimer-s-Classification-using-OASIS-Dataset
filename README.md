# Alzheimer-s-Classification-using-OASIS-Dataset

**Project Title: Alzheimer's Disease Classification**

**Abstract:**
This project focuses on developing and evaluating classification models for detecting Alzheimer's disease through Brain Magnetic Resonance Image (MRI) scans. Both multiclass and binary classifications are performed using various machine learning models, including Logistic Regression, Linear Discriminant Analysis (LDA), K-Nearest Neighbors (KNN), and ensemble techniques which were implemented from scratch(without the use of any library), and also is green coded. The dataset utilized is the OASIS Alzheimer's Dataset obtained from Kaggle, containing multiple brain MRI images across different classes. The project explores downsampling techniques, image modifications (blur and edge detection), and ensemble methods to enhance classification accuracy.

**Introduction:**
Alzheimer's disease is a progressive neurodegenerative disorder affecting memory and cognitive abilities. This project aims to classify Alzheimer's using Brain MRI scans from the OASIS dataset. Traditional machine learning models, such as Logistic Regression and LDA, are initially employed for binary classification. The transition to multiclass classification involves exploring various models, including KNN and Naive Bayes, along with preprocessing techniques like image blurring and edge detection.


**Method:**
- **Dataset Description:** Utilizes the OASIS-1 Alzheimer's Dataset from Kaggle, downsampled and categorized into classes.
- **Data Preprocessing:** Addresses class imbalance, downsamples images and applies modifications such as blur and edge detection.
- **Binary Classification:** Implements Logistic Regression and LDA for classifying Alzheimer's and non-Alzheimer's cases.
- **Multiclass Classification:** Utilizes Multi-Class LDA, KNN, Naive Bayes, and 1vs1 techniques for classifying into non-demented, very mild dementia, mild dementia, and moderate dementia.
- **Ensembling:** Combines the three best-performing models (1vs1 LDA, 1vs1 Logistic Regression, and KNN with Canny Edge) using mean ensemble techniques.
- **Green Coding:** All the models were implemented and improved by keeping in mind the factor of efficiency.

**Evaluation:**
Binary classification models achieve satisfactory accuracy. Multiclass LDA struggles, prompting exploration of alternative models like KNN and Naive Bayes. Ensembling these models improves accuracy significantly, with the mean ensemble achieving 83.17% accuracy in higher dimensions. Below are the outcomes of our ensembled models.


<div align="center">
<div style="text-align: center;">
    <table>
        <thead>
            <tr>
                <th>Ensemble Evaluation</th>
                <th colspan="2">Image Size</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td></td>
                <td>64x32</td>
                <td>128x64</td>
            </tr>
            <tr>
                <td>Accuracy</td>
                <td>0.8271</td>
                <td>0.8318</td>
            </tr>
            <tr>
                <td>Precision</td>
                <td>0.8357</td>
                <td>0.8377</td>
            </tr>
            <tr>
                <td>Recall</td>
                <td>0.8271</td>
                <td>0.8318</td>
            </tr>
            <tr>
                <td>F1</td>
                <td>0.8314</td>
                <td>0.8347</td>
            </tr>
        </tbody>
    </table>
</div>
</div>

**Conclusion:**
Ensembling the top-performing models enhances Alzheimer's classification accuracy, emphasizing the effectiveness of combining diverse models. The results demonstrate the significance of ensemble modeling in achieving optimal performance across various configurations.


**Refer to Paper for Full Explanation**
