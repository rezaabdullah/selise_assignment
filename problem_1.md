# **Question**
Let's say you are a Data Scientist working in a company that analyzes social media contents. Business team approached you and told you to build an Agent that will understand the context of a social media post that they will use to segment the content, find popularity, trends etc.
## **Approach**
**Assumptions:** Based on the scenario, it is assumed that there is already ***data warehouse*** for the social media post.

**Scope:** The scope of the project will center around creating a roadmap and data pipeline to extract and analyze informations that are relevant for:  
**i. User growth**  
**ii. Monetizing users**  
**iii. Sentiment analysis**

**Methodology:** The main objective of the task would be to create an intelligent agent or a machine learning model that can be trained periodically and deployed in the production to generate insights on-demand. The following steps are necessary to build such model:
* **ETL pipeline:** Since social media context along with user segmentation will be analyzed, it is required to extract the dataset and develop an ETL (extract, transformation and load) pipeline. At this stage, depending on the types of data we may need to perform data deduplication, data normalizing and exploratory statistical analysis. 
* **Selecting training dataset:** Once the ETL pipeline is developed for different types of data such as audios, text, user logs, user information and videos etc., dataset can be randomly split into training dataset and test dataset. After the selection of the dataset, we may require to annotate the dataset depending on the language and other criterias. Data annotation process should be automated where data annotators can extract the data, label them and upload in the database. For different types of datasets and analysis, different machine learning pipeline are needed to be developed:  
    **i. Text analysis:** Text data needs to be tokenized and NLP libraries such as NLTK can be used to analyze the sentiments and other requirements. The steps for developing text analysis are: i. tokenization ii. stop word filtering iii. negation handling iv. stemming v. classification vi. sentiment class  
    **ii. Audio analysis:** There could be two approach for audio analysis. Audios can be converted into text by speech-to-text libraries or the sentiment can be analyzed directly using other libraries such as _**Librosa**_ or deep learning frameworks such as _**Tensorflow.**_  
    **iii. Image/video analysis:** From images and videos it is more relevant to detect and classify objects. There are different tools, frameworks and libraries are available for object detection and classification.  
    **iv. Analyzing user information:** 

