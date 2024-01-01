## Creating a Custom Text Classification Solution

In our exploration of Azure's AI capabilities, we delved into the realm of Natural Language Processing (NLP), where the goal was to decipher human language through software. Within Azure's toolkit, text classification—covering sentiments, languages, and user-defined categories—became our focal point.

### The Azure AI Language Service

Our learning journey led us to comprehend the nuances of classifying text using Azure's AI Language service. This service enables us to categorize text into custom groups, empowering us to assign specific labels (or classes) to various text files. For instance, a video game summary could be classified into genres like "Adventure," "Strategy," "Action," or "Sports."

### Project Types in Custom Text Classification

We traversed two fundamental types of projects:

1. **Single Label Classification:**
   - Here, each file is assigned just one class. For example, a game summary could only be labeled as "Adventure" or "Strategy."

2. **Multiple Label Classification:**
   - This project type permits assigning multiple classes to each file, allowing flexibility in labeling like "Adventure" or "Adventure and Strategy."

### Key Aspects Explored:

#### 1. Labeling Data:
- For single label projects, one class per file is assigned during labeling. However, in multiple label projects, multiple classes can be assigned per file. Quality, clarity, and variety of data influence model accuracy.

#### 2. Evaluating and Improving the Model:
- Measures like Recall, Precision, and F1 Score became our tools to assess model performance, identifying false positives and negatives. Improving the model involved seeking more high-quality data.

#### 3. API Payload and Project Lifecycle:
- The REST API facilitated model building and interaction, guiding us through defining labels, tagging data, training, viewing, improving, deploying models, and finally, text classification.

#### 4. Dataset Splitting for Training:
- The importance of splitting datasets into training and testing phases was emphasized, with options for automatic or manual splits.

#### 5. Deployment Options and REST API Usage:
- Azure's flexibility in deploying multiple models and versions allowed for thorough testing and comparison. The REST API, functioning asynchronously, enabled seamless development and interaction with language projects.

## Lab
Diving into Azure's suite of NLP capabilities, we explored features like key phrase identification, text summarization, and sentiment analysis. Among these, the Azure AI Language service stood out for its unique offerings, including custom question answering and custom text classification.

### Configuring and Testing the Custom Text Classification

To test the Azure AI Language service's custom text classification capabilities, we embarked on a journey that involved configuring the model using Language Studio and employing a Cloud Shell-based command-line application. This process mirrors real-world application development, offering practical insights.

### Setting up Azure AI Language Resources

The initial step involved provisioning an Azure AI Language service resource. If not already available, we outlined the steps to create this resource within the Azure portal, emphasizing the importance of enabling the Custom text classification & extraction feature.

### Uploading Sample Articles for Training

Following the resource setup, we covered the process of uploading example articles to train the model. This step involved configuring a storage account, enabling blob anonymous access, creating and populating a container named "articles" with the sample articles downloaded earlier.

### Creation of a Custom Text Classification Project

Moving forward, we delved into creating a custom text classification project using Language Studio. This involved guiding users through the project setup, including defining project details, choosing the article container, and specifying labeling options.

### Labeling Data for Model Training

Once the project was set up, the focus shifted to labeling the data for training the model. Detailed instructions were provided on how to categorize and assign datasets (training/testing) to individual articles, ensuring clarity and accuracy during labeling.

### Training, Evaluation, and Deployment

With the labeled data in place, we proceeded to train the model, evaluating its performance, and making improvements where necessary. The process included monitoring model performance metrics, identifying errors, and deploying the trained model for practical usage.

### Preparing an App in Visual Studio Code

To test the custom text classification capabilities practically, users were guided through developing a simple console application in Visual Studio Code. Detailed steps were provided for configuring the application and integrating Azure AI Language functionality.

### Code Integration and Testing

Finally, we integrated Azure AI Language services into the application code, enabling document classification. Instructions for running the application and observing classification outcomes were provided, facilitating practical testing.

## Lessons Learned

Our journey through this module offered insights into text classification, encompassing project types, data tagging, model training, and using the REST API for text classification tasks.
Post-module completion, we've gained the ability to:
- Recognize classification project types.
- Develop custom text classification projects.
- Tag data, train models, and deploy them.
- Perform classification tasks via our applications, leveraging the Azure AI Language service.


## Acknowledgements
- https://learn.microsoft.com/en-us/training/modules/custom-text-classification/

## Badges Earned
- [Create A Custom Text Classification Solution Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/BLXA4TCD?sharingId=966CA24C5AD997DF)![Create A Custom Text Classification Solution Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/0863e5d5-aad3-4a7f-aa8a-9af89c930f8b)

