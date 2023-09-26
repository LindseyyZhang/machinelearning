# Introduction for the proejct 
This project serves as a group assignment for one of my master's modules in machine learning. The journey has been enlightening, providing a comprehensive insight into the application of machine learning in the business realm. I am particularly grateful for the suggestions and guidance received from our professor, Linus, and of course my teammates(Cheng and Ella). Through this project, I have gained a deeper understanding of the critical aspects of data science, recognizing its limitations and the importance of adopting a critical perspective.

## Dataset 
This study comprises 119,390 booking instances from both a City Hotel and a Resort Hotel in Portugal, recorded between July 1, 2015, and August 31, 2017. Each instance represents an individual booking. The dataset is from Kaggle. Here is the link to access it. https://www.kaggle.com/datasets/mojtaba142/hotel-booking

# Methodology
## Data Preprocessing
The initial step involved a visual inspection of the predominantly categorical dataset. A rigorous data preprocessing stage followed, including cleaning, partitioning, and refining the data. This stage concluded with a correlation analysis to enable a more profound exploration of the dataset, ensuring it met the prerequisites for the subsequent application of machine learning algorithms.

## Model Selection
Informed by existing literature, the study employed five models known for their efficacy in similar research: Logistic Regression, Decision Tree, Random Forest, Support Vector Machine, and Neural Networks. The choice of models was critical for accurate predictions. These models underwent thorough testing using cross-validation to evaluate their fit to the test data and were assessed based on accuracy scores, with a threshold of 0.8 indicating high confidence. The highest-scoring model, in this case is the Randomn Forest, was then selected for further optimization and testing.

## Model Optimization
A series of optimization steps were carried out to fine-tune the parameters of the Random Forest model. This optimisation was carried out by completing a grid search on 50% of the dataset, involved systematically working through multiple combinations of parameters to identify the optimal settings. The search was conducted using two sets of parameters, with cross-validation performed three times in the first search and five times in the second search to ensure robust evaluation.

## Model Assessment
To address concerns of overfitting, the study compared the Random Forest model’s performance on both the training and test datasets. The comparable accuracy scores on both datasets suggest a consistency in performance, indicating the model is not merely memorizing the training data but is also capable of making reliable predictions on unseen data.
