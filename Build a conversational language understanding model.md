# Build a conversational language understanding model

Building a conversational language understanding (CLU) model involves several steps, from defining intents and entities to training, testing, and deploying the model.

### 1. **Define Intents and Entities:**
   - **Intents:** These represent the tasks or actions a user wants to perform, defining the meaning of user utterances. For example, "GetTime," "GetWeather," or "TurnOnDevice."
   - **Entities:** These add specific context to intents, like location, time, or device. Entities can be learned, listed, or prebuilt.

### 2. **Collect Utterances for Each Intent:**
   - Capture a diverse range of example utterances for each intent.
   - Include variations in length, grammar, word placement, and different ways of expressing the same intent.
   - Label data precisely, consistently, and completely to train the model effectively.

### 3. **Use Patterns to Differentiate Similar Utterances:**
   - When similar utterances represent different intents, create patterns to disambiguate them.
   - Provide examples that cover various formats of similar utterances to train the model effectively.

### 4. **Utilize Prebuilt Entity Components:**
   - Incorporate prebuilt components to detect common entities like numbers, URLs, or emails.
   - Leverage prebuilt components to automatically identify specified entity types without specific training examples.

### 5. **Train, Test, and Review:**
   - Train the model with the collected data to learn intents and entities from sample utterances.
   - Test the model interactively or with a testing dataset to evaluate its performance.
   - Review predictions, refine the model based on feedback, and iterate on utterances to improve the model's accuracy.

### 6. **Deploy the Model:**
   - Once trained and tested, deploy the trained model to a public endpoint for client applications to use.

### 7. **Iterate and Improve:**
   - Continuously review user interactions and feedback to refine the model iteratively.
   - Update and retrain the model to adapt to changing user intents and language patterns over time.

## Hands-On

**1. Provisioning Azure AI Language Resource:**
   - **Action:** Created an Azure AI Language service resource within the Azure subscription.
   - **Outcome:** Obtained necessary keys and endpoints for model access and deployment.

**2. Creating a Conversational Language Understanding Project:**
   - **Action:** Initialized a project named "Clock" for language understanding in English.
   - **Outcome:** Defined intents like GetTime, GetDay, GetDate, and associated sample utterances for each intent.

**3. Training and Testing the Model:**
   - **Action:** Trained the model using defined intents and utterances, evaluating its performance metrics.
   - **Outcome:** Tested the model with various utterances to ascertain its accuracy in predicting intents.

**4. Adding Entities to Enhance Context:**
   - **Action:** Added entities like Location, Weekday, and Date to refine the model's understanding by mapping entities to specific terms in utterances.
   - **Outcome:** Retrained the model to incorporate the new entities, improving its ability to extract relevant information.

**5. Integration into Client Application:**
   - **Action:** Configured and integrated the Azure AI Language resource into a client application (either C# or Python).
   - **Outcome:** Developed functionalities to interact with the deployed model, receive user input, predict intents, and perform actions based on identified intents and entities.

**6. Testing the Client Application:**
   - **Action:** Ran the client application in the integrated development environment (Visual Studio Code).
   - **Outcome:** Tested the application's functionality by entering various utterances to see how accurately the model predicts intents and extracts entities, performing the appropriate action based on the prediction.

Throughout the process, adjustments were made to refine the model's understanding by adding entities, training it with more data, and finally integrating it into a client application for real-time use. The focus was on continuously improving the model's accuracy in interpreting user intents and entities from natural language input.

Absolutely, here's a simple "What We Learned" section in Markdown format:

### What We Learned
- **Azure AI Language Service Provisioning:**
  - Creating an Azure AI Language service resource within Azure subscription.
- **Conversational Language Understanding Project:**
  - Defining intents and sample utterances for a language understanding project.
- **Model Training and Evaluation:**
  - Training the language model, evaluating its performance metrics, and adjusting based on results.
- **Entity Integration for Context Enhancement:**
  - Adding entities to improve the model's understanding by associating specific terms in utterances.
- **Client Application Integration:**
  - Configuring and integrating Azure AI Language resource into a client application (C# or Python).
- **Testing and Refinement:**
  - Iteratively testing the client application, refining the model's accuracy, and improving functionality based on user input.
 

## Acknowledgements
- https://learn.microsoft.com/en-us/training/modules/build-language-understanding-model


## Badge(s) Earned
[Build a Conversational Language Understanding Model Badge](https://learn.microsoft.com/api/achievements/share/en-us/JainAyushri-0042/AQGE4YV7?sharingId=966CA24C5AD997DF) ![Build a Conversational Language Understanding Model Badge](https://github.com/AJ1904/Microsoft-Ignite-Azure-AI-Language/assets/49027490/34f9e90d-ba3a-47d5-9f86-61fffab7aef0)
