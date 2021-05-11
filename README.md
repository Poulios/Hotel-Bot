## Microsoft Bot Framework Implementation
### for the case of a hotel business

**Scope**: A chatbot that serves hotel's needs (_JavaScript SDK v4_).

**Goals**: 
1. Functionality to answer QnA related to the hotel (_for example What time can i check in?, Which is the charging policy for limousine service?, Can I use any fitness equipment during my accomondation?_).
1. Functionality to answer QnA related to general staff (_for example How are you?, What are you?, What can you do? etc._).
1. Functionality to querie for available room at the hotel's management system having firstly collected the necessary details with one of the following ways
	1. By collecting the necessarry details through a dialog (_What date do you desire check in?, What date do you desire check out?, What room category do you desire?, How many rooms do you want?_)
	1. By extracting all the necessary details from a customer prompt statement (_for example Can i book two Deluxe Single rooms check in date 10 August and check out date 15 August, I want ten Junior Suite Unter den Linden from 8 August to 28 August_) 

In order to create a chatbot that achieves the above functionality goals we started with adjustments of official [BotBuilder Samples](https://github.com/microsoft/BotBuilder-Samples/tree/main/samples/javascript_nodejs) for the [Bot Framework](https://docs.microsoft.com/en-us/azure/bot-service/index-bf-sdk?view=azure-bot-service-4.0):

**NLP Bot** 
- [repo](https://github.com/microsoft/BotBuilder-Samples/tree/main/samples/javascript_nodejs/14.nlp-with-orchestrator)
- [Code documentation](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-tutorial-dispatch?view=azure-bot-service-4.0&tabs=js)

The NLP Bot distingues 3 intents (q_sample-qna Goals #1 & #2_, RoomAvailability ability _Goal #3a_, Bookdetails _Goal #3b_)
code dispatchBot

**Prompt for user input**
- [repo](https://github.com/microsoft/BotBuilder-Samples/tree/main/samples/javascript_nodejs/44.prompt-for-user-input)
- [Code documentation](https://docs.microsoft.com/en-us/azure/bot-service/bot-builder-primitive-prompts?view=azure-bot-service-4.0&tabs=javascript)


customPromptBot Prompts customer for input and validate booking details (Ability 3.a)
Extract details from customer statement and validate details
Hotel management system tables that are necessary for bot's operation 

safdsf   

