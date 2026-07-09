## Welcome to my Portfolio

# Hi, I’m Rukayat Amzat 👋

### Machine Learning Engineer | Data Analyst | AI Engineer | Sustainability Engineer

MSc Advanced Chemical Engineering (Distinction)

University of Manchester

Building machine learning systems, data analytics solutions, and AI applications for sustainability & carbon capture research.

📬 Let's Connect:

🔗 [LinkedIn](https://www.linkedin.com/in/rukayat-amzat-889839173/) 

💻 [GitHub](https://github.com/orbitnook) 


# Featured Project

## [Physics-Informed Feature Engineering and ML Prediction for CO2 Adsorption in Metal-Organic Frameworks (MOFs)](https://github.com/orbitnook/Engineering-ML-Features-for-MOF-CO2-Adsorption)

Problem Statement: Traditional ML models for CO₂ adsorption in MOFs rely on geometric descriptors, which fail to capture complex adsorption behaviour at intermediate pressures.

This work introduces energy-based features derived from CO₂ probe simulations, significantly improving predictive performance, especially in the 0.1–0.5 bar range.

Approach:
- Simulated CO₂ and O₂ probe interactions with MOF surfaces to model adsorption behaviour at the molecular level.
- Computed interaction energies by evaluating probe–surface configurations across different orientations.
- Transformed raw energy interaction data into structured energy distributions using histogram-based feature engineering.
- Developed energy-based descriptors and compared them with conventional geometric features (e.g., surface area, pore size, density).
- Combined geometric and energy-derived features to train machine learning models for CO₂ uptake prediction across multiple pressure points.

Tools: Python, PowerBI, Auto-sklearn, CRAFTED MOF Database, CIF (crystallographic file), ASE atom package

Key Highlights:
- 900+ engineered descriptors
- CO₂ vs O₂ probe comparison
- Feature engineering impact analysis
- R² up to ~0.95

![](/images/Pg1.png)


![](/images/Pg2.png)


![](/images/Pg3.png)


![](/images/Pg4.png)


# ML/AI Projects

## [AI chatbot LLM QA evaluator](https://github.com/orbitnook/AI_Chatbot_Testing_LLM_evaluator)

Problem: LLM outputs are often inconsistent and difficult to evaluate manually at scale. This project demonstrates a simplified QA evaluation pipeline that mimics how AI-generated content can be systematically assessed using predefined rubrics, similar to early-stage RLHF evaluation workflows.

Approach:
- Built a lightweight LLM evaluation framework for assessing AI-generated responses using structured, rule-based rubrics.
- Designed a deterministic scoring system that evaluates outputs across multiple dimensions including clarity, completeness, structure, and relevance.
- Simulated an LLM evaluation pipeline commonly used in QA and GenAI testing workflows, without relying on external APIs.
- Developed an interactive Streamlit interface that allows users to compare high-quality and low-quality responses and observe how evaluation scores change.

Stack: Python, Streamlit, OpenAI API

Example Usage:
Users can select between:
- High-quality structured response (expected PASS)

![](/images/llm-evaluator-1.png)


![](/images/llm-evaluator-2.png)


![](/images/llm-evaluator-3.png)

- Low-quality / nonsensical response (expected FAIL)

![](/images/llm-evaluator-4.png)


![](/images/llm-evaluator-5.png)


The system evaluates and returns:
- Score breakdown
- Final decision (PASS / FAIL)

Possible Improvements:
- Replace rule-based scoring with LLM-as-a-judge evaluation
- Add embedding-based semantic similarity scoring
- Introduce multi-model evaluation comparison
- Expand into dataset benchmarking tool for LLM outputs


## [Querying and reading Multiple PDF files using OpenAI and Langchain](https://github.com/orbitnook/OpenAI_ex/blob/main/Quering_Multiple_PDF_from_Vector_Store_using_Langchain.ipynb)

Problem: With LLM prevalent and trained on various human data, it poses the question of hallucination. What if we want to leverage the benefit of large language models but have our own specific knowledge base, e.g. PDF files.

Solution: Integrate the data sources into the OpenAI querying pipeline.

Approach: 
- Built a Retrieval-Augmented Generation (RAG) pipeline for querying multiple PDF documents.
- Used LangChain to orchestrate the LLM workflow and manage document processing.
- Converted PDFs into structured document objects using UnstructuredPDFLoader.
- Generated vector embeddings for document chunks and stored them in a vector database for semantic search.
- Enabled context-aware querying by retrieving the most relevant document chunks and passing them to the LLM for response generation.

Stack: Python, LangChain

![](/images/query.png)



## [Smart Conversation Reply](https://github.com/orbitnook/Smart-Reply-suggest)
Problem: Responding to large volumes of messages can be time-consuming and lead to missed communications.

Solution: Developed a smart reply recommendation system that suggests relevant responses based on conversation context.

Approach: 
- Building Similarity indexes with the ANNOY library.
- Employing Hdbscan clustering to cluster similar replies.
- Trained an LSTM model to generate context-aware response suggestions.
- Used the Amazon Topical Chat dataset (8,000+ conversations, 184,000+ messages).

Result:
- Achieved 97% accuracy with a loss of 0.1177.
- Generated multiple relevant reply suggestions for a given message.

Example usage:
   Input - bye

Suggested replies: 
    Response 1 -> bye  
    Response 2 -> have a good one  
    Response 3 -> same to you  
    Response 4 -> have a good weekend  

Future Improvements:
- Improve clustering performance.
- Restore punctuation in generated responses.
- Deploy as a user-facing application



# 👁 Computer Vision Projects

## [Face Recognition with Siamese Network](https://github.com/orbitnook/Face-Verification-with-Siamese-Network-and-Kivy-App)
Problem: Develop a face verification system capable of determining whether two images belong to the same person.

Approach: 
- Built a Siamese Convolutional Neural Network (CNN) for face verification.
- Combined a public face dataset ([Labelled Faces](http://vis-www.cs.umass.edu/lfw/)) with self-collected images captured using OpenCV.
- Applied image augmentation and preprocessing to create over 6,000 labelled image pairs.
- Used shared embedding networks and an L1 distance layer to compare facial representations.
- Trained the model using Binary Cross-Entropy loss and the Adam optimizer.

Results:
- Achieved precision and recall of 1.0 on the test dataset.
- Developed a simple Kivy-based interface for real-time interaction with the model.

Technologies: Python, TensorFlow, OpenCV, Kivy, Computer Vision, Deep Learning


![](/images/verified.jpg)


![](/images/kivy.png)


# 📊 Predictive ML Projects

## [Detecting Hate Speech in Tweets](https://github.com/orbitnook/NLP-notebooks/blob/main/Detecting%20Hate%20speech%20in%20tweet.ipynb)

Problem: Classify tweets as hate speech or normal speech.

Approach: 
- Text preprocessing (stopword removal, cleaning)
- Feature extraction using Count Vectorizer
- Trained Naive Bayes models for classification. 

Dataset: 5,232 tweets (3,000 non-hateful, 2,242 hateful).

![image](https://github.com/orbitnook/orbitnook/assets/74497446/3d469d62-5828-48a7-906f-f69384b179b2)

Result:
- Gaussian Naive Bayes: 60% accuracy
- Multinomial Naive Bayes (with feature engineering): 86% accuracy.
  
![image](https://github.com/orbitnook/orbitnook.github.io/assets/74497446/75c2deb1-8c7d-488a-a9c0-f2671e01ebb2)



## [Heart Disease Prediction](https://github.com/orbitnook/Tensorflow-practice/blob/main/Dp_Classification%2C_heart_disease.ipynb)
Problem: Predict whether a patient has heart disease based on medical features.

Dataset: 14 clinical variables, ~300 samples.

Approach: 
- Built baseline neural network model
- Applied Recursive Feature Elimination (RFE) for feature selection
- Compared performance before and after feature selection

Results:
- Baseline model: 82% accuracy
- Feature-selected model: 84% validation accuracy

![](/images/loss_without.png)

![](/images/feature_selected.png)

![](/images/loss_with.png)



## [Credit Card Lead Prediction](https://github.com/orbitnook/Project-/blob/main/Credit_card_interest_classification.ipynb)

Problem: Predict customer interest in credit card offers for a retail bank.

Dataset: 245,725 records with significant class imbalance.

Approach:
- Encoding (Label + One-Hot Encoding)
- SMOTE for class balancing
- Feature scaling
- Tested multiple models (Logistic Regression, Random Forest, XGBoost, Voting Classifier, Neural Network)

Results:
- Best model (Neural Network): ~85.8% accuracy
- Strong F1-score performance after handling imbalance
  
![image](https://github.com/orbitnook/orbitnook/assets/74497446/46454917-682a-4d91-a7b3-ae8096d20c6f)

     
![image](https://github.com/orbitnook/orbitnook/assets/74497446/21d7a2bf-be91-4abf-81f8-7754bdb6bc59)



# 📈 Data Analysis Projects

## [Wrangle and Analyze Data: We Rate Dogs](https://github.com/orbitnook/Project-/blob/main/WeRateDogs/wrangle_act.ipynb)

Problem: Clean and analyse messy real-world social media data. 

Approach:
- Collected data from multiple sources (CSV archive, API via Tweepy, image predictions via Requests)
- Cleaned and merged datasets into a single analysis-ready dataset
- Performed exploratory data analysis on dog ratings and trends

Key Insights:
- Labrador Retriever was the most common breed
- Retweets peaked in 2016
- Popular dog names included Charlie, Cooper, Lucy, and Oliver

![image](https://github.com/orbitnook/orbitnook/assets/74497446/9f20079b-ea18-4dd2-873d-c30509e85d32)



## [Investigate a Dataset: No Show Appointment](https://github.com/orbitnook/Project-/blob/main/Investigate_a_Dataset.ipynb)

Problem: Understand factors influencing missed medical appointments.

Dataset: 100,000+ medical appointments in Brazil.

Approach:
- Cleaned and explored patient demographic and health data
- Analysed relationships between health conditions and appointment attendance

Key Insights:
- Diabetes patients showed slightly higher attendance rates (82%) than non-diabetic patients (80%)
- Females were overrepresented in the dataset
- Teenagers with hypertension showed lower attendance rates (<70%).

![image](https://github.com/orbitnook/orbitnook/assets/74497446/c5add26d-8aa8-4134-9d36-9f692b5e20af)


<!--
## [Segmentation and Classification of fishes using Images](https://www.kaggle.com/rukayaamzat/91-accuracy-cnn-for-fish-classification)
- Project: Augmentation and Classification of the fishes based on images to their correct class using the Sequential model.

Approach:
  - Trained a Convolutional Neural Network (CNN) on a dataset of 9 seafood classes and 9,000 images.
  - Applied image augmentation and preprocessing using Keras ImageDataGenerator.
  - Used convolution, max-pooling, and dropout layers to improve generalisation and reduce overfitting.

Results:
- Achieved 92% accuracy and 98% recall on the classification task.

Technologies: Python, TensorFlow/Keras, Computer Vision, Deep Learning

![](/images/fish_loss.png)

![](images/fish_class.png)
-->
