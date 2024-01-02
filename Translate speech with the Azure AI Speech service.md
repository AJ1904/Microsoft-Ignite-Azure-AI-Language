## Translate Speech with Azure AI Speech

Speech translation expands on speech recognition by transcribing spoken input in one language and providing translations in multiple other languages.

### Provisioning Azure Resources

The Azure AI Speech service offers robust speech translation powered by machine learning. To use this service, we provision an Azure AI Speech resource in our subscription. Retrieve location and keys from the resource's Keys and Endpoint page.

### Translating Speech to Text

Utilize the Azure AI Speech SDK to facilitate speech translation. Create a TranslationRecognizer object with a SpeechTranslationConfig, specifying source and target languages. Process the response to access transcriptions and translations.

### Synthesizing Translations

After obtaining translated transcriptions, we can synthesize speech from these translations using event-based synthesis or manual synthesis methods.

## Lab
Azure AI Speech offers a speech translation API enabling language translation for various purposes. For instance, it allows the development of translation applications to assist travelers in communicating across languages.

### Provisioned Azure AI Speech Resource

1. Opened the [Azure portal](https://portal.azure.com) and signed in.
2. Searched for "Azure AI services" and select "Speech service" to create a resource.
3. Configured the resource settings and retrieve the keys and endpoint from the deployed resource's "Keys and Endpoint" page.

### Prepared Application in Visual Studio Code

1. Accessed the provided GitHub repository for the speech app in Visual Studio Code.
2. Installed necessary dependencies and update configuration files with Azure AI Speech resource details.

### Implemented Speech Translation

1. Integrated Azure AI Speech SDK into our application using Python.
2. Configured translation and speech settings using the provided code snippets.
3. Ran the program to translate spoken input into multiple languages supported by the application.

### Synthesize Translated Speech

Added code to synthesize translated text into speech using the Azure AI Speech service.

### Lessons Learned

- **Resource Provisioning**: Understanding the process of setting up Azure AI Speech resources is fundamental.
- **SDK Integration**: Utilizing the SDK and configuring it correctly for speech translation functionality is key.
- **Configuration Handling**: Updating and managing configuration files for language translation settings is crucial.
- **Speech Translation Implementation**: Implementing speech translation from spoken input to multiple languages using Azure AI Speech.
- **Speech Synthesis**: Synthesizing translated text into speech using the Speech service for enhanced communication.
- **SDK Utilization**: Utilizing the SDK to configure speech translation settings is crucial for accurate output.
- **Response Handling**: Efficiently handling response data aids in accessing desired transcriptions and translations.
- **Synthesis Methods**: Understanding both event-based and manual synthesis methods for speech-to-speech translation.

## Acknowledgements
- https://learn.microsoft.com/en-us/training/modules/translate-speech-speech-service/

## Badge(s) Earned
- [Develop natural language processing solutions with Azure AI Services Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/ZPC3AZB2?sharingId=966CA24C5AD997DF)![Develop natural language processing solutions with Azure AI Services Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/4f99c7fd-104c-43b9-b993-3390258ebe88)
- [Translate speech with the Azure AI Speech service Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/HYKJUHR8?sharingId=966CA24C5AD997DF)![Translate speech with the Azure AI Speech service Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/8e197378-d7a5-47dc-a502-1ed2b702f658)

