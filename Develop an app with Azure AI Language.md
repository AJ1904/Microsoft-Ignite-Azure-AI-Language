## Developing an App with Azure AI Language

Upon creating an Azure AI Language Understanding model, we can publish and integrate it into client applications.


The Azure AI Language Understanding service facilitates the definition and training of language models that predict user intent from natural language input. To incorporate this model into an application, it needs to be published and consumed by a client application.

### Understanding Azure AI Language Service Capabilities

The Azure AI Language service offers several features to understand human language better. Applications can utilize these features individually or together to gain insight into user intentions and inquiries.

#### Preconfigured Features

The Azure AI Language service provides specific features without model labeling or training, offering immediate use within our app. These include:

- Summarization
- Named Entity Recognition
- Personally Identifiable Information (PII) Detection
- Key Phrase Extraction
- Sentiment Analysis
- Language Detection

#### Learned Features

Learned features require labeling data, training, and deployment of models to be utilized in your application. These include:

- Conversational Language Understanding (CLU)
- Custom Named Entity Recognition
- Custom Text Classification
- Question Answering

### Processing Predictions

To integrate our Azure AI Language Understanding model into a client application, we can utilize REST APIs or language-specific SDKs. Requests for predictions are sent to the Azure AI Language service and include specific parameters based on the language feature requested.

#### Prediction Results

The prediction results, delivered in JSON format via REST interfaces or object hierarchy via SDKs, provide details about detected intents, entities, and other pertinent information about user queries.

## Creating a Language Service Client Application

### Understanding Conversational Language Understanding

The Conversational Language Understanding feature within Azure AI Service allows the creation of language models that interpret user intent and identify relevant entities. Client applications can consume these models using REST interfaces or language-specific SDKs.

### Cloning the Repository

1. We cloned existing repository.
     ```
     git clone https://github.com/MicrosoftLearning/mslearn-ai-language ai-language
     ```
   
### Setting Up Language Service Resources

2. **Created Language Service Resources:**
   - In the Azure portal, we created a Language service resource with specific settings:
     - Default features: All
     - Custom features: none
     - Subscription: Azure subscription
     - Resource group: Choose or create a resource group
     - Region: Westus2
     - Pricing tier: S
     - Confirm Responsible AI Notice

3. **Imported, Trained, and Published a Conversational Language Understanding Model:**
   - Opened the Language Studio portal at [Language Studio Portal](https://language.cognitive.azure.com).
   - Signed in and complete the Welcome steps.
   - Imported the Clock.json file.
   - Trained the app and create a deployment named "production."

### Prepared for Language Service SDK Usage

4. **Prepared for Language Service SDK:**
   - We used Python and:
     - Installed the required packages.
     - Accessed and updated the configuration file with the Endpoint URL and Primary Key.

### Implemented the Client Application

5. **Implemented the Application:**
   - Loaded the necessary namespaces or dependencies.
   - Created a client for the Language service model.
   - Used the client to get predictions from the Conversational Language model.
   - Applied appropriate actions based on predicted intents and entities detected in user input.

6. **Tested the Application:**
   - Ran the program in chosen language.
   - Entered different utterances to test the application's functionality, such as inquiries about time, date, or day.
   - Observed the application's responses based on the predicted intents and detected entities.


### What We Learned

In this module, we learned how to publish and use Azure AI Language understanding apps, empowering us to configure, understand features, and deploy this service effectively.
- Understood the capabilities of an Azure AI Language Understanding model
- Implemented predictions from an Azure AI Language within our application
- Configured Azure AI Language Understanding app publishing options
- Deploy the Azure AI Language Understanding Service as a container

## Acknowledgements
- https://learn.microsoft.com/en-us/training/modules/publish-use-language-understand-app/

## Badge(s) Earned
[Create a Language Understanding solution with Azure AI Language Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/K5FREC2B?sharingId=966CA24C5AD997DF) ![Create a Language Understanding solution with Azure AI Language Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/8a3ddc24-fbd1-429a-a292-ce517ff32cdf)

[Develop an app with Azure AI Language Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/DGY74UQJ?sharingId=966CA24C5AD997DF) ![Develop an app with Azure AI Language Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/3833cff9-5a87-4270-a90b-19dadbc124ca)




