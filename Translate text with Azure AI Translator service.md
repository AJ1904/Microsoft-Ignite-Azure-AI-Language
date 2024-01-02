## Translating Text with Azure AI Translator

Azure AI Translator service facilitates intelligent language translation between various languages, offering capabilities like language detection, translation, transliteration, and specific translation options. The service supports over 90 languages.

#### Provisioned Azure AI Translator Resource

- Created an Azure AI Translator resource in our Azure subscription to access the translation APIs.
- Obtained the resource's location and subscription keys for API access through REST or language-specific SDKs.

#### Understood Language Capabilities

##### Language Detection
- We utilized the Detect function via the REST API to identify the language of a given text.
- Example: Detecting Japanese language from text 'こんにちは' using curl commands.

##### Translation
- Used the Translate function to convert text between languages.
- Translated text from Japanese ('ja') to English ('en') and French ('fr') using the API.

##### Transliteration
- Converted text from one script to another using the Transliterate function.
- Example: Transliterating Japanese text 'こんにちは' to Latin script ('Latn').

#### Specify Translation Options

- Customized translation behavior by setting various parameters:
  - Word alignment for better understanding of text relationships.
  - Include sentence length for UI presentation.
  - Handle profanity filtering during translation.

#### Defined Custom Translations

- Developed custom translation models for specific vocabularies or industry terms.
- Created a workspace, uploaded training data, trained a model, tested it, and published the model through the Custom Translator portal.
- Used the category Id of our custom model in translation calls to Azure AI Translator.

#### Calling the API

- Initiated translation requests by sending POST requests to the specified URL.
- Included parameters like api-version, target language ('to'), and category Id.
- Specified required headers: Ocp-Apim-Subscription-Key and Content-Type.
- The request body contained an array with a JSON object specifying the text to translate.

#### API Response

- Successful requests returned a response code of 200 with translated text in the response body.

## Lab
We created an app to translate text using the Azure AI Translator service. It involved provisioning the service, setting up Visual Studio Code, configuring the app, and implementing the translation functionality.

#### Provisioned Azure AI Translator Resource
- Accessed the Azure portal and created an Azure AI Translator resource:
  - Opened Azure portal, searched for "Azure AI services," selected "Translator," and created a resource.
  - Set subscription, resource group, region, name, pricing tier, and agreed to Responsible AI Notice.
  - Reviewed and waited for deployment completion to access resource keys and endpoint.

#### Prepared Development Environment

- Used Visual Studio Code to develop the translation app using provided code files from the GitHub repo:
  - Cloned the repository if not done earlier and open it in Visual Studio Code.
  - Installed necessary files to support C# or Python code projects.

#### Configured Application

- Set up the application to use Azure AI Translator:
  - Installed Azure AI Translator SDK package for C# or Python.
  - Updated configuration values in the appsettings.json (C#) or .env (Python) file with Azure AI Translator resource details.

#### Implemented Translation Functionality

- Integrated Azure AI Translator to translate text:
  - Added required namespaces to import the necessary SDK elements in C# or Python files.
  - Created a client using Azure AI Translator endpoint and key.
  - Enabled user input for selecting the target language.
  - Implemented text translation functionality using Azure AI Translator service.

#### Tested the Application

- Ran and tested the application to verify the translation functionality:
  - Executed the program in the integrated terminal for C# `dotnet run` or Python `python translate.py`.
  - Entered a valid target language and phrases for translation.
  - Reviewed the translated results and verify the language detection and translation to the target language.


## Acknowledgements
- https://learn.microsoft.com/en-us/training/modules/translate-text-with-translator-service

## Badge(s) Earned
- [Translate text with Azure AI Translator service Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/YV56F5ZR?sharingId=966CA24C5AD997DF)![Translate text with Azure AI Translator service Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/70a1e556-d68c-46cb-932e-0d6b78a18e4f)




