## Azure AI Language: Question Answering

### Discovering Question Answering Capabilities
We harnessed Azure AI Language's question answering feature, empowering us to establish knowledge bases using question-answer pairs. These bases, accessible via a REST endpoint, served as invaluable resources for client applications, particularly bots. Our sources included:

- Extraction from FAQ web pages.
- Compilation from structured text files like brochures or guides.
- Integration of chit-chat pairs for common conversational exchanges.

### Comparing Question Answering and Language Understanding
By delving into these language models, we uncovered distinctions in usage and response processing:

| Question Answering      | Language Understanding  |
|-------------------------|-------------------------|
| User asks for an answer | User expects a response or action |
| Matches query to answer | Interprets intent, identifies entities |
| Provides a static answer | Indicates likely intent and referenced entities |
| Client showcases the answer | Client takes action based on detected intent |

We realized the complementary nature of these services in creating comprehensive language solutions.

### Crafting a Knowledge Base
Our journey involved creating, training, and deploying knowledge bases using REST APIs, SDKs, or the intuitive Language Studio web interface:

- Sign-in and resource creation in the Azure Portal.
- Configuring an Azure AI Language resource, enabling the question answering feature.
- Selection or creation of an Azure AI Search resource to host the base index.
- Leveraging Language Studio to construct a Custom question answering project.
- Populating our base with data sources like web URLs, files, or predefined chit-chat datasets.

### Implementing Engaging Multi-turn Conversations
We enhanced our knowledge bases by introducing follow-up prompts, enriching user interactions by gathering specific information before providing definitive answers.

### Testing and Publishing Our Knowledge Base
Once our bases were defined and trained, we meticulously tested and deployed them for application and bot usage. Our testing phase within Language Studio involved submitting inquiries and reviewing confidence-scored responses. Finally, deploying these bases to REST endpoints granted seamless access for client applications to query and retrieve answers.

### Elevating Question Answering Performance
To continuously improve our bases, we embraced active learning and synonym definitions:

- **Active Learning:** Explored alternate question suggestions, refining our answers over time.
- **Synonyms:** Defined multiple synonymous words, improving our system's interpretation of queries.


## Hands-On

### Setting Up Azure AI Language Resource
1. **Provisioning the Resource:**
    - Navigated to Azure portal and created an Azure AI Language service resource.
    - Enabled the Question Answering feature within the resource setup.

2. **Configuration and Deployment:**
    - Selected the desired settings such as subscription, resource group, and region.
    - Configured the Azure Search region and pricing tier.
    - Waited for deployment completion and accessed the deployed resource.

### Building a Question Answering Project
1. **Creating a Knowledge Base:**
    - Utilized the Language Studio portal to establish a project focused on Microsoft Learn FAQs.
    - Selected English as the language and specified project details.

2. **Importing Sources:**
    - Imported data from the Microsoft Learn FAQ webpage.
    - Added conversational chit-chat pairs to support common interactions.

3. **Knowledge Base Editing:**
    - Added new question-answer pairs sourced from the Microsoft Learn FAQ.
    - Introduced alternate questions and follow-up prompts to enrich responses.

### Training and Testing the Knowledge Base
1. **Testing in Language Studio:**
    - Submitted various test queries to ensure appropriate responses.

2. **Deployment:**
    - Published the knowledge base to access its REST interface for client applications.

### Preparing for App Development in Visual Studio Code
1. **Cloning the Repository:**
    - Cloned the necessary repository into Visual Studio Code.

2. **Configuring the Application:**
    - Installed the Azure AI Language question answering SDK package.
    - Updated configuration values, incorporating endpoint and key information.

### Integrating Azure AI Language Functionality
1. **Adding SDK Libraries:**
    - Imported necessary namespaces or libraries to establish connections and submit queries.

2. **Implementing Submission and Retrieval:**
    - Integrated code to fetch answers based on user-submitted questions.
    - Displayed retrieved answers along with related details.

### Running the Application
1. **Executing the Code:**
    - Ran the application to interactively submit questions and retrieve corresponding answers.

2. **Reviewing Responses:**
    - Checked and assessed the returned answers for accuracy and relevance.

This immersive journey highlighted the steps from resource provisioning to app integration, enabling us to leverage Azure AI Language's question answering prowess effectively.


## Lessons Learned

- Distinguishing features between question answering and language understanding.
- A step-by-step process from creation to deployment and consumption of knowledge bases.
- Implementation of engaging multi-turn conversations and continuous improvement through active learning and synonyms.

## Acknowledgements
- https://learn.microsoft.com/en-us/training/modules/create-question-answer-solution-ai-language/

## Badge(s) Earned
[Build a Question Answering Solution Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/YV5MMSKR?sharingId=966CA24C5AD997DF) ![Build a Question Answering Solution Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/f1db1208-7b56-4d9c-ab3c-f10e43b04565)
