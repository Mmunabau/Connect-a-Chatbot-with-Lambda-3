<h1>Connects a Chatbot with lambda</h1>

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
 <br />
 Navigate to your lambda console
  <br/>
<img src="images/lx2.png" height="80%" width="80%" alt="key steps"/>
<br />
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
 TestBotAlias is a default version of your bot that's made for testing or
 development.
 To connect Lambda with my BankerBot, I visited my bot's TestBotAlias and the
 custom Checkbalance slot.<br/>
<img src="images/lx3.png" height="80%" width="80%" alt="key steps"/>
<br />

<br />
 Code Hooks:
 A Code hooks is a piece of code that can be connected to my chatbot to perform functions/actions that my chatbot cannot do alone/by default Even though I already connected my Lambda function with my chatbot's alias, I had to use code hooks because the chatbot is not able to calculate/return a bank balance figure on its own I could find code hooks at '.Fulfillment code hook sectio<br/>
<img src="images/lx4.png" height="80%" width="80%" alt="key steps"/>
<br />
<br />
The final result!
 'I've set up my chatbot to trigger Lambda and return a random dollar figure
 when customers request for there account Balance and Credencials asked by
 the chatbot <br/>
<img src="images/lx6.png" height="80%" width="80%" alt="key steps"/>
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

