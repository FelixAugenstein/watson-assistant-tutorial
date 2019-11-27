<h1 align="center" style="border-bottom: none;">:de: IBM Digital Tech Tutorial: Watson Assistant</h1>
<h3 align="center">In this hands-on tutorial you will create a new IBM Watson Assistant Service on the IBM Cloud and deploy your service with a Node.js app</h3>

You can view a demo of this app <a href="https://watson-assistant-demo-dach.eu-de.mybluemix.net/" target="_blank">here</a>.


## Prerequisites

1. Sign up for an [IBM Cloud account](https://console.bluemix.net/registration/).
2. Fill in the required information and press the „Create Account“ button.
3. After you submit your registration, you will receive an e-mail from the IBM Cloud team with details about your account. In this e-mail, you will need to click the link provided to confirm your registration.
4. Now you should be able to login to your new IBM Cloud account ;-)

## Configuring the Watson Assistant on the IBM Cloud

<h4>1) Create a Watson Assistant Service</h4>
In the Catalogue section, click on the AI category, then select Watson Assistant. On the next page select the Lite Plan and you can also choose a region, where you would like to deploy your service as well as a service name. 

![Catalog Watson Assistant](readme_images/catalog-watson-assistant.png)

<br>
<h4>2) Access your Watson Assistant Service</h4>
Go back to your IBM Cloud Dashboard by clicking the IBM Cloud Logo. Under services you will find the Watson Assistant Service in the corresponding region. Access your service by launching it. Afterwards click on skills and create a new skill.

![Create a new Skill](readme_images/create-skill.png)

<br>
<h4>3) Create Intents, Entities and the Dialog</h4>
The next step is to build your conversation. You can choose to build a customer service assistant, for instance. The three elements to consider are Intents, Entities and the Dialog.
Intents define a user's goal or purpose. Per intent you can configure various user examples. An example of an intent could be #Price and user examples could be “How much does it cost?” and “What is the price?”
Entities handle significant parts of an input that should be used to alter the way the assistant responds to the intent. An example of an entity could be @products with the entity values “juice” and “water”.
Dialog consists of dialog nodes. Each node is made up of a trigger (condition) and a response. If the assistant recognizes the intent #Price, it could then respond: Would you like to know the price of juice or water? Otherwise, if the assistant recognizes the intent #price and the entity value @products is juice, it could then respond: The price of juice is 2€ per bottle.

<br>
4) Deploy your configured Watson Assistant
To deploy your assistant click on Assistants, then click on create assistant and give your integration a name. Then click on add a dialog skill to select your previously configured dialog skill. Afterwards go to the Preview Link and visit the provided URL. You can now talk to your Assistant :-)

![Create a new Skill](readme_images/deploy-assistant.png)

