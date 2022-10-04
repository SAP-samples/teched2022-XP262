# Exercise 4 - How does SAP Cloud Connector and SAP Private Link service help?

Now that you have seen how the extension application is notified about new or changed business partners and where the data subsequently comes from via SAP Cloud Connector or SAP Private Link service, let's take a look at the data storage of the extension application. In some cases, it may either make sense or even be necessary to provide the extension application with its own data storage. It could make sense if you want to work independently of the SAP S/4HANA system, for example if the SAP S/4HANA system is not available and users should still be able to use the applications. It is necessary in general if additional content (such as the "verification status" field in our case) is to be stored. 


Applications developed with the SAP Cloud Application Programming Model benefit from automatically generated database artefacts. These can then be deployed in a so-called HDI container in the SAP HANA Cloud. We will not go into the details of an HDI container here; more information is available at [help.sap.com](https://help.sap.com/docs/SAP_HANA_PLATFORM/3823b0f33420468ba5f1cf7f59bd6bd9/e28abca91a004683845805efc2bf967c.html?version=2.0.04&locale=en-US): 


## Exercise 4.1 SAP Cloud Connector
## Exercise 4.2 SAP Private Link service

## Summary

You should now have a good overview of how the extension application is notified about new or changed business partners using SAP Event Mesh and where the data is stored. 

Next, you are going to have a look at the logs that your application produces and set some of the outputs in context. 

