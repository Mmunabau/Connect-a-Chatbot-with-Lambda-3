<h1>Build a Chatbot with Amazon lex</h1>

<h2>Description</h2>
 Amazon Lex is a fully managed service by AWS for building conversational interfaces into applications using voice and text. It uses automatic speech recognition (ASR) to convert speech to text and natural language understanding (NLU)
<br />

<h2>  How I used Amazon Lex in this project </h2>
 we used Amazon lex with lambda functions to generate random account balance for customers when they request it from a specific account Type. AWS Lambda is a service that lets you run code in the cloud without needing to manage any computers/servers - Lambda will manage them for you.Lambda runs your code only when needed and scales automatically
<h2>Skills Demostrated:</h2>

- <b>Cloud Computing Proficiency: Configuring AWS services like IAM, Lambda, and Amazon Lex to build and manage conversational interfaces</b> 
- <b>Natural Language Understanding (NLU): Designing intents, utterances, and slot types to enable the chatbot to comprehend and respond effectively to user queries.</b>
- <b>Problem-Solving with Lambda: Developing and deploying AWS Lambda functions for custom business logic and advanced intent fulfillment..</b>

<h2>Utilities used</h2>
<ul>
  <li>AWS console</li>
   <li>Amazon Lex</li>
</ul>
<h2>Program walk-through:</h2>

<p align="center">
 AWS Lambda Functions: I created a Lambda function to' Generate random Account balance for customers base on the account provided however in the real world the Lambda Function can be used to extract the user's bank balance from a database <br/>
 <img src="images/lx1.png" height="80%" width="80%" alt="key steps"/>
<br />
 
<br />
Chatbot Alias:An alias in Amazon Lex is a pointer for a specific version of your bot. So when you're connecting Lex with other AWS services or your custom applications,those 
 external resources will connect to an alias, which will point to the specific version
  <br/>
<img src="images/lx2.png" height="80%" width="80%" alt="key steps"/>
<br />

<br />
 configure bot setting: While creating my chatbot, I also created a role with basic permissions because' it will creat permissions to other AWS services if needed.
 In terms of the intent classification confidence score, I kept the default value of 0.40. This means'for my chatbot is it should at least be 40% confident about the intent goal of the chatbot user to respond in more technical terms.<br/>
<img src="images/lx3.png" height="80%" width="80%" alt="key steps"/>
<br />

<br />
Creat an Intents:  Intents are what the user is trying to achieve in their conversation with the chatbot.I created my first intent, WelcomeIntent, to' respond back to me base on my request<br/>
<img src="images/lx4.png" height="80%" width="80%" alt="key steps"/>
<br />
<br />
FallbackIntent: I launched and tested my chatbot, which could respond successfully if I enter' Hello ,Hi,I need help and Can you help me? My chatbot returned the error message 'Intent FallbackIntent is fulfilled' when I entered... This error message occurred because'Amazon Lex doesn't quite recognize your utterance <br/>
<img src="images/lx6.png" height="80%" width="80%" alt="key steps"/>
<br />
<br />
 Configuring FallbackIntent:FallbackIntent is a default intent in every chatbot that gets triggered when your chatbot has a confidence score below 40% for all the intents you've defined I wanted to configure FallbackIntent because' The default closing response to the user is not easily understandab <br/>
<img src="images/lx7.png" height="80%" width="80%" alt="key steps"/>
<br />
<br />
  Variation:  I also added variations! What this means for an end user is' they get to see different forms of the my chatbot's closing response <br/>
<img src="images/lx8.png" height="80%" width="80%" alt="key steps"/>
<br />
<br />
 Test chatbot and Deploy: chatbot sucessful. <br/>
<img src="images/lx9.png" height="80%" width="80%" alt="key steps"/>
<br />


</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
