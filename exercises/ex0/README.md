# Getting Started

Before you start work on the existing extension application, let's make sure you have all of the tools you need to complete this session successfully. This exercise will give you a few login credentials that you will need to remember throughout the session. **Please do not use any other user than the one assigned to you.**

There are only two accounts that you need in the entire session. Both of them are provided by SAP, please do not use your personal users for the subsequent exercises.

## Test SAP S/4HANA access

The _source system_ so to speak for our extension application is an SAP S/4HANA on-premise system. You will mostly work in the transaction **BP** to create/modify business partners which will trigger events for SAP Event Mesh or to check changes to business partners that have been made using the SAP BTP extension application. This user is used for tasks that are usually done by a functional end user.

1. Log on to the SAP S/4HANA on-premise system using the SAPGUI on your Desktop. Therefore, open **SAP Logon** on your Desktop. 

2. Select (TODO: Enter correct system name, systems not yet available) from the list of systems. 

3. Enter the following credentials: 

* Client: 100
* User: S4H_0XX
* Password: Welcome1

**IMPORTANT:** XX is the UserID on your desk. In case 01 is your UserID, please use S4H_001 as the user for the SAP S/4HANA sytem.

4. Enter **bp** as the transaction code and hit **Enter** to open the transaction. Alternatively you can also you use double-click the entry in your user menu. 

![How to enter the Business Partner transaction](./images/bp_transaction_code.png)

## Test SAP BTP access

Of course, you will also receive a user for the SAP BTP in order to be able to access your very own existing extension application and the corresponding services of this scenario. 

1. There are a few tool options that we have in order to walk you through this session and the takeways that we want to tackle. It could either be the Cloud Foundry CLI/SAPBTP CLI(either on the machines commandline/terminal or SAP Business Application Studio) or the SAP BTP Cockpit. We try to keep tools/and the potential hurdles at a minimum level in order to focus on the key aspects - understanding and getting in touch with the architecture - of the extension application. That's why we are going to use the SAP BTP Cockpit throughout this session.

👉 Open the SAP BTP Cockpit: https://cockpit.eu10.hana.ondemand.com/cockpit/#/globalaccount/fb7dfea1-5d8c-431d-bd16-1ebbe842f62f/subaccount/145b0547-19d3-4d89-9b81-e55ed8d5f1db

Enter your SAP BTP account credentials: 

* User: XP262-0XX
* Password: (TODO, noch nicht bekannt)

2. Let's have a look at a few menu items to proof that you have all the required RoleCollections. 

👉 Go to **Services > Instances & Subscriptions**. You should see a list with service instances and subscriptions that your SAP TechEd instructors have been created before. If you have issues seing this list, please reach out to one of the instructors. 

(TODO: Screenshot hinzufügen)

3. Go back to the **Overview** menu where you'll find lots of information about the subaccount itself. Among other things, there is a list of Cloud Foundry spaces inside, you should see a **dev** space there. 

![Go to Cloud Foundry space by clicking on the dev space name](./images/go_to_cfspace.png)

👉 Navigate directly to the Cloud Foundry space by clicking on **dev**. 

Here, for example, you get an overview of the applications that have been deployed in this Cloud Foundry space. There is an application for each participant that is only intended for the respective participant. Each app has its own front end with its own URL, its own backend and its own HDI container in the SAP HANA Cloud.The only thing you share with all participants is the SAP S/4HANA system, even if you have been given your very own user for it. But more about that later. 

## Summary

Now that you have tested both required accounts, you should be well equipped to see the extension application in action. In the next step, you'll see how SAP Event Mesh connects SAP S/4HANA and SAP BTP. 
Continue to - [Exercise 1 - Exercise 1 Description](../ex1/README.md)
