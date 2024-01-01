## Custom Named Entity Extraction with Azure AI Language

### Understanding Custom Named Entity Recognition (NER)

Custom NER, a feature within Azure AI Language, allows extracting predefined entities from unstructured text documents. These entities could span people, places, events, skills, or values. The goal here was to extract these entities from texts not in a known format, like legal agreements or online ads.

### Built-in vs. Custom NER

Azure AI Language offers built-in entity recognition for common categories like person, location, organization, or URL. However, custom NER steps in when specific entities require extraction. For instance, extracting specific legal or banking data, improving catalog searches, or identifying text for audit policies.

### The Project Lifecycle

Our journey mirrored the Azure AI Language project lifecycle, encompassing steps to define, tag, train, view, improve, deploy, and extract entities.

### Considerations for Success

For optimal performance, the quality and diversity of training data play a crucial role. High-quality, diverse datasets aid in teaching the model accurately. Defining entities clearly and distinctly avoids ambiguity and improves model performance.

### Labeling Data

Precision, consistency, and completeness in labeling data are key aspects. These ensure accurate training for the model to recognize and extract entities effectively.

### Training and Evaluation

Training and evaluating the model involve iterative processes, adding and refining data to enhance the model's accuracy. Metrics like precision, recall, and F1 score guide the improvements needed.

### The Confusion Matrix

The confusion matrix visually illustrates entity performance, aiding in identifying areas for model enhancement.

## Lab
Azure AI Language Service allows defining and extracting custom entities from text documents. The workflow involves provisioning the service, uploading sample ads, creating a custom entity recognition project, labeling data, training the model, evaluation, deployment, and application integration.

#### Provisioned Azure AI Language Resource
- We created an Azure AI Language Service resource enabling Custom text classification & extraction.
- Uploaded sample ads to the storage account.

#### Created Custom Named Entity Recognition Project
- Accessed Azure AI Language Studio portal, selected the language resource, and created a new custom entity recognition project.
- Configured project settings and labeled the uploaded data by identifying entities like ItemForSale, Price, and Location.

#### Trained and Evaluated Model
- Started a training job to train the model, splitted the testing set from training data, and evaluated the model's performance through scoring metrics.

#### Deployed Model
- Deployed the trained model to allow entity extraction via the API.

#### Application Development in Visual Studio Code
- Configured and set up a console application in Visual Studio Code using the Azure AI Language resource.
- Added code to extract entities from text using the Text Analytics SDK.

#### Test Application
- Ran the application to analyze and extract entities from the provided classified ads.

### Lessons Learned
- Understood labeled entities and their significance.
- Developed a custom entity extraction project.
- Labeled data, trained models, and deployed entity extraction solutions.
- Integrated entity extraction tasks into custom applications.

## Acknowledgements
- https://learn.microsoft.com/en-us/training/modules/custom-name-entity-extraction

## Badges Earned
- [Create A Custom Named Entity Extraction Solution Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/PTWXQG54?sharingId=966CA24C5AD997DF) ![Create A Custom Named Entity Extraction Solution Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/0d016556-bbb1-4a51-bb26-cc96cca65b11)

