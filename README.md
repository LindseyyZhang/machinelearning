# Introduction for the proejct 
This project serves as a group assignment for one of my master's modules in machine learning. The journey has been enlightening, providing a comprehensive insight into the application of machine learning in the business realm. I am particularly grateful for the suggestions and guidance received from our professor, Linus, and of course my teammates(Cheng and Ella). Through this project, I have gained a deeper understanding of the critical aspects of data science, recognizing its limitations and the importance of adopting a critical perspective. Below, I provide a simple description of the analysis process and share my reflections on this project. If you have any questions regarding to this project, I would be happy to answer it. 

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

# Implication
For dynamic pricing and inventory allocation to be genuinely responsive, the model needs to be deeply embedded within the hotel's central reservation system (CRS) and the Hotel Property Management System (PMS). Such integration can facilitate the swift reallocation of rooms, especially in instances of booking classification changes.

Moreover, it is paramount to understand the constantly evolving nature of the hospitality industry. With shifts in marketing strategies, a surge in online platform bookings, or even changing guest preferences, predictor variables like “MarketSegment,” “DistributionChannel,” and “LeadTime” undergo significant transformations. Thus, while crafting tailored offers to guests based on insights from the model, managers must recognize that the underlying data is subject to change with shifts in guest behaviours and market dynamics. This consideration necessitates ongoing monitoring and refinement of the model to ensure that offers continue to resonate with guests' unique needs and preferences, truly maximising revenue, occupancy, and satisfaction.

# Reflection
Building the model to predict cancellations was a careful process that needed a lot of attention. The data had to be just right, as any mistakes or missing information could make the model work poorly. In essence, the predictive model is not just a static tool but an evolving strategy that needs both integration and periodic re-evaluation to remain effective in the ever-changing hospitality industry.

This study provides a comprehensive insight into the complex dynamics of hotel booking cancellations and devises a predictive model capable of assessing the likelihood of cancellations with an accuracy score of 86.33%.

The extensive exploratory analysis identified key factors influencing cancellations, in alignment with previous studies.Utilising Random Forest as the chosen modelling tool aligns with contemporary trends in the domain.

The business implications of the study extend beyond mere cancellation prediction, translating into actionable insights for real-time pricing adjustments, distribution channel management, intelligent room allocation, and enhanced customer engagement. Moreover, it offers strategic recommendations on model integration, recognizing the evolving nature of the industry. 

## Limitations and Future Researches
In evaluating the proposed model's performance, significant effectiveness was observed in predicting cancellation patterns. However, this study has several limitations. 

Firstly, the data is exclusively drawn from hotels in Portugal, which raises questions about the applicability of the findings to hotels in other countries or datasets with more diverse variables. Moreover, the inclusion of only two hotels in the study may limit the ability to generalise the model's performance across different settings or scales.

Secondly, the absence of a specific pricing strategy stands as a limitation. While the study identifies seasonal trends in bookings and cancellations, it falls short of establishing a robust pricing strategy. This would necessitate a more intricate set of data, encompassing elements such as historical pricing, competitor pricing, variable costs, and information on local economic indicators. Without this detailed information, the model's capability to simulate different pricing scenarios and analyse price elasticity is substantially restricted.

Thirdly, the reliance on historical data may present a limitation in projecting future trends, particularly in the face of unprecedented events or rapidly changing market dynamics. The model may not account for sudden shifts in consumer behaviour, changes in regulatory policies, or unforeseen economic challenges. The exclusive focus on quantitative data might also overlook qualitative aspects, such as customer satisfaction, brand perception, or unique cultural factors that might significantly influence booking and cancellation behaviours.

The challenge of extending the model's applicability to various global contexts and incorporating more intricate data to shape specific strategies emerges as a critical frontier in evolving the predictive capabilities further.

