# Create Speech-Enabled Apps with Azure AI Services
The module focused on utilizing Azure AI Speech service capabilities, emphasizing speech recognition and speech synthesis functionalities. It covered using APIs for speech-to-text and text-to-speech, enabling the creation of speech-enabled applications.

#### Provisioned Azure AI Speech Resource

- Created an Azure AI Speech resource in your Azure subscription:
  - Accessed the Azure portal and create a dedicated or multi-service Azure AI Speech resource.
  - Collected location and keys for client application access from the Keys and Endpoint page.

#### Used Azure AI Speech to Text API

- Utilized the Speech to text and Speech to text Short Audio REST APIs:
  - Performed speech recognition for spoken input or batch transcription.
  - Preferred language-specific SDKs for interactive speech-enabled applications.

#### Implemented Speech to Text using SDK

- Followed a consistent pattern for speech recognition:
  - Configured SpeechConfig and AudioConfig objects.
  - Created a SpeechRecognizer object.
  - Invoked SpeechRecognizer methods for transcription and process response.

#### Utilized Azure AI Text to Speech API

- Used REST APIs for speech synthesis:
  - Employed Text to speech and Batch synthesis APIs.
  - Preferred language-specific SDKs for interactive speech-enabled applications.

#### Implemented Text to Speech using SDK

- Structured for implementing speech synthesis:
  - Set up SpeechConfig and AudioConfig objects.
  - Created a SpeechSynthesizer object.
  - Employed SpeechSynthesizer methods for converting text to speech and handle the result.

#### Configure Audio Format and Voices

- Customized audio output and select voices:
  - Set desired output audio format using SpeechConfig.
  - Specified voices for personalized speech synthesis through SpeechSynthesisVoiceName property.

#### Employed Speech Synthesis Markup Language (SSML)

- Leveraged SSML for detailed speech synthesis control:
  - Employed XML-based SSML syntax for speech characteristics control.
  - Controlled speaking styles, insert pauses, adjust prosody, specify phonemes, and utilize "say-as" rules.
  - Used SpeakSsmlAsync() method to submit SSML description to the Speech service.

## Lab
Azure AI Speech provides speech-to-text and text-to-speech APIs to implement speech recognition and speech synthesis functionalities. The exercise demonstrates using both APIs to create a speaking clock application.

#### Provisioned Azure AI Speech Resource

- Accessed the Azure portal, created an Azure AI Speech resource with specific settings (subscription, resource group, region, name, pricing tier), and noted down the keys and endpoint information.

#### Prepared Development Environment

- Used Visual Studio Code and clone the provided GitHub repository for the speech app.
- Installed necessary packages for Python app.

#### Configured Application for Azure AI Speech

- Updated the configuration files (.env for Python) with Azure AI Speech resource information (region and key).

#### Integrated Azure AI Speech SDK

- Imported required namespaces in the code files (Program.cs for C# or speaking-clock.py for Python).
- Configureed the SpeechConfig for speech service in the Main function.

#### Implemented Speech Recognition

- Configured speech recognition for microphone or audio file input.
- Processed spoken input using SpeechRecognizer in the application.

#### Synthesized Speech Output

- Configured speech synthesis to generate spoken output using SpeechSynthesizer.
- Added code to create spoken output in the application based on user input.

#### Used Different Voices or SSML

- Changed voices for synthesis by modifying the voice in the code.
- Alternatively, utilized SSML for customized speech output, specifying voice and additional characteristics.

#### Ran the Program

- Executed the program in the integrated terminal for the speaking-clock folder to test speech recognition and synthesis functionalities.

### Final Steps

- Verified speech recognition by speaking into the microphone or using an audio file, prompting the app for the current time.
- Ensured the application synthesizes spoken output correctly, responding with the time based on the input.


## Lessons Learned
- **Resource Configuration**: Accurate setup of Azure AI Speech resources (keys, region) is critical for seamless integration.
- **Development Setup**: Cloning repositories and installing required packages streamlines development.
- **SDK Integration**: Importing namespaces and updating config files enables efficient use of Azure AI Speech SDK.
- **Speech Recognition**: Handling microphone input and errors aids in recognizing varied user commands.
- **Speech Synthesis**: Configuring voices and SSML enhances speech output personalization.
- **Testing & Improvement**: Validating inputs, troubleshooting errors, and exploring features lead to refinement.
- **Resource Understanding**: Grasping service capabilities optimizes application usage.
- **Continuous Learning**: Exploring documentation and community insights fosters ongoing improvement.


## Acknowledgements
- https://learn.microsoft.com/en-us/training/modules/create-speech-enabled-apps/
## Badge(s) Earned
- [Create speech-enabled apps with Azure AI services Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/4SNYEZ9K?sharingId=966CA24C5AD997DF)![Create speech-enabled apps with Azure AI services Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/c496c9c1-9e90-4bd2-9b79-1ef22986e363)

