<h2 align="center"><ins>PREGUNTAS AZ-204 RUTAS MICROSOFT LEARN</ins></h2><br>b

<b>1. ¿Cuál de las siguientes categorías de plan de App Service proporciona las capacidades máximas de escalabilidad horizontal?</b>
- Proceso dedicado.
- Aislado.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Proceso compartido.

"La categoría Aislado proporciona aislamiento de red y proceso, y tiene la capacidad máxima de escalabilidad horizontal."

<b>¿Cuál de las siguientes características de red de App Service puede usarse para controlar el tráfico de red saliente?</b>
- Dirección asignada a las aplicaciones.
- Conexiones híbridas.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Puntos de conexión del servicio.

"Las conexiones híbridas son una característica de red saliente."

<br><h2 align="center"><ins>PREGUNTAS AZ-204 EXAMTOPICS</ins></h2><br>

<b>1. You have two Hyper-V hosts named Host1 and Host2. Host1 has an Azure virtual machine named VM1 that was deployed by using a custom Azure Resource Manager template. You need to move VM1 to Host2. What should you do?</b>
- From the Update management blade, click Enable.
- From the Overwiew blade, move VM1 to a different subscription.
- From the Redeploy blade, click Redeploy.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- From the Profile blade, modify the usage location.

"When you redeploy a VM, it moves the VM to a new node within the Azure infrastructure and the powers it back on, retaining all your configuration options and associated resources."

<b>2. You have downloaded an Azure Resource Manager template to deploy numerous virtual machines. The template is based on a current virtual machine, but must be adapted to reference an administrative password. You need to make sure that the password is not stored in plain text. You are preparing to create the necessary components to achieve your goal. Which of the following should you create to achieve you goal?</b>
- An Azure Key Vault.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- An Azure Storage account.
- Azure Active Directory (AD) Identity Protection.
- An access policy.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- An Azure policy.
- A backup policy.

<b>3.Your company has an Azure Kubernetes Service (AKS) cluster that you manage from an Azure AD-joined device. The cluster is located in a resource group. Developers have created an application named MyApp. MyApp was packaged into a container image. You need to deploy the YAML manifest file for the application. Solution: You install the Azure CLI on the device and run the "kubectl apply f myapp.yaml" command. Does this meet the goal?</b>
- Yes.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- No.

"kubectl apply -f myapp.yaml applies a configuration change to a resource from a file or stdin"


<b>4. Your company has an Azure Kubernetes Service (AKS) cluster that you manage from an Azure AD-joined device. The cluster is located in a resource group. Developers have created an application named MyApp. MyApp was packaged into a container image. You need to deploy the YAML manifest file for the application. Solution: You install the docker client on the device and run the "docker run -it microsoft/azure-cli:0.10.17" command. Does this meet the goal?</b>
- Yes.
- No.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

<b>5. Your company has a web app named WebApp1. You use the WebJobs SDK to design a triggered App Service background task that automatically invokes a function in the code every time new data is received in a queue. You are preparing to configure the service processes a queue data item. Which of the following is the service you should use?</b>
- Logic Apps.
- WebJobs.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Flow.
- Functions.

<b>6. Your company has an Azure subscription. You need to deploy a number of Azure virtual machines to the subscription by using Azure Resource Manager (ARM) templates. The virtual machines will be included in a single availability set. You need to ensure that the ARM template allows for as many virtual machines as possible to remain accessible in the event of fabric failure or maintenance. Which of the following is the value that you should configure for the platformFaultDomainCount property?</b>
- <label>10.</label>
- <label>30.</label>
- Min Value.
- Max Value.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
  
"The number os fault domains for managed availability sets varies by region - either two or three per region."

<b>7. Your company has an Azure subscription. You need to deploy a number of Azure virtual machines to the subscription by using Azure Resource Manager (ARM) templates. The virtual machines will be included in a single availability set. You need to ensure that the ARM template allows for as many virtual machines as possible to remain accessible in the event of fabric failure or maintenance. Which of the following is the value that you should configure for the platformUpdateDomainCount property?</b>
- <label>10.</label>
- <label>20.</label>
- <label>30.</label>
- <label>40.</label>  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"Each virtual machine in your availability set is assigned an update domain and a fault domain by the underlying Azure platform. For a given availability set, five non-user-configurable update domains are assigned by default (Resource Manager deployments can then be increased to provide up to 20 update domains) to indicate groups of virtual machines and underlying physical hardware that can be rebooted at the same time."

<b>8. You are creating an Azure Cosmos DB account that makes use of the SQL API. Data will be added to the account every day by a web application. You need to ensure that an email notification is sent when information is received from IoT devices, and that compute cost is reduced. You decide to deploy a function app. Which of the following should you configure the function app to use?</b>
- Azure Cosmos DB connector.
- SendGrid action.
- Consumption plan.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Azure Event Hubs binding.
- SendGrid binding.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

<b>9. This question requires that you evaluate the underlined text to determine if it is correct.
You company has an on-premises deployment of MongoDB, and an Azure Cosmos DB account that makes use of the MongoDB API.
You need to devise a strategy to migrate MongoDB to the Azure Cosmos DB account.
You include the Data Management Gateway tool in your migration strategy.
Instructions: Review the underlined text. If it makes the statement correct, select `No change required.` If the statement is incorrect, select the answer choice that makes the statement correct.</b>
- No change required.
- Mongorestore.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Azure Storage Explorer.
- AzCopy.

<b>10. You are developing an e-Commerce Web App. You want to use Azure Key Vault to ensure that sign-ins to the e-Commerce Web App are secured by using Azure App Service authentication and Azure Active Directory (AAD). What should you do on the e-Commerce Web App</b>
- Run the az keyvault secret command.
- Enable Azure AD Connect.
- Enable Managed Service Identity (MSI).  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Create an Azure AD service principal.

"A managed identity from Azure Active Directory allows your app to easily access other AAD-protected resources such as Azure Key Vault."

<b>11. This question requires that you evaluate the underlined text to determine if it is correct.
Your Azure Active Directory Azure (Azure AD) tenant has an Azure subscription linked to it.
Your developer has created a mobile application that obtains Azure AD access tokens using the OAuth 2 implicit grant type.
The mobile application must be registered in Azure AD.
You require a redirect URI from the developer for registration purposes.
Instructions: Review the underlined text. If it makes the statement correct, select `No change is needed.` If the statement is incorrect, select the answer choice that makes the statement correct.</b>
- No change required.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- A secret.
- A login hint.
- A client ID.

"For Native Applications you need to provide a Redirect URI, which Azure AD will use to return token responses."

<b>12. You are creating an Azure key vault using PowerShell. Objects deleted from the key vault must be kept for a set period of 90 days.
Which two of the following parameters must be used in conjunction to meet the requirement? (Choose two)</b>
- EnabledForDeployment.
- EnablePurgeProtection.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- EnabledForTemplateDeployment.
- EnableSoftDelete.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

<b>13. You have an Azure Active Directory (Azure AD) tenant. You want to implement multi-factor authentication by making use of a conditional access policy. The conditional access policy must be applied to all users when they access the Azure portal. Which three settings should you configure?</b>

![question 13](./images/question-13.jpg)
![question 13 solution](./images/question-13-solution.jpg)

"The conditional access policy must be applied or assigned to Users and Groups.  
The conditional access policy must be applied when users access the Azure portal, which is a cloud app. That is: Microsoft Azure Management.  
Access control must require multi-factor authentication when granting access."

<b>14. You manage an Azure SQL database that allows for Azure AD authentication. You need to make sure that database developers can connect to the SQL database via Microsoft SQL Server Management Studio (SSMS). You also need to make sure the developers use their on-premises Active Directory account for authentication. Your strategy should allow for authentication prompts to be kept to a minimum. Which of the following should you implement?</b>
- Azure AD token.
- Azure Multi-Factor authentication.
- Active Directory integrated authentication.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- OATH software tokens.

"Azure AD can be the initial Azure AD managed domain. Azure AD can also be an on-premises Active Directory Domain Services that is federated with the Azure AD. Using an Azure AD identity to connect using SSMS or SSDT. The following procedures show you how to connect to a SQL database with an Azure AD identity using SQL Server Management Studio or SQL Server Database. Use this method if you are logged in to Windows using your Azure Active Directory credentials from a federated domain. 
1. Start Management Studio or Data Tools and in the Connect to Server (or Connect to Database Engine) dialog box, in the Authentication box, select Active.  

<span style="display:block;text-align:center;">![question 14](images/question-14.jpg)</span>

2. Select the Options button, and on the Connection Properties page, in the Connect to database box, type the name of the user database you want to connect to (The AD domain name or tenant ID option is only supported for Universal with MFA connection options, otherwise it is greyed out)."

<b>15. You are developing an application to transfer data between on-premises file servers and Azure Blob storage. The application stores keys, secrets, and certificates in Azure Key Vault and makes use of the Azure Key Vault APIs. You want to configure the application to allow recovery of an accidental deletion of the key vault or key vault objects for 90 days after deletion. What should you do?</b>
- Run the Add-AzKeyVaultKey cmdlet.
- Run the az keyvault update --enable-soft-delete true --enable-purge-protection true CLI.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Implement virtual network service endpoints for Azure Key Vault.
- Run the az keyvault update --enable-soft-delete false CLI.

"When soft-delete is enabled, resources marked as deleted resources are retained for a specified period (90 days by default). The service further provides a mechanism for recovering the deleted object, essentially undoing the deletion. Purge protection is an optional Key Vault behavior and is not enabled by default. Purge protection can only be enabled once soft-delete is enabled. When purge protection is on, a vault or an object in the deleted state cannot be purged until the retention period has passed. Soft-deleted vaults and objects can still be recovered, ensuring that the retention policy will be followed. The default retention period is 90 days, but it is possible to set the retention policy interval to a value from 7 to 90 days through the Azure portal. Once the retention policy interval is set and saved it cannot be changed for that vault."

<b>16. You have developed a Web App for your company. The Web App provides services and must run in multiple regions. You want to be notified whenever the Web App uses more than 85 percent of the available CPU cores over a 5 minute perior. Your solution must minimize costs. Which command should you use?</b>

![question 16](./images/question-16.jpg)
![question 16 solution](./images/question-16-solution.jpg)

<b>17. The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements:  
You are configuring a web app that delivers streaming video to users. The application makes use of continuous integration and deployment. You need to ensure that the application is highly available and that the users streaming experience is constant. You also want to configure the application to store data in a geographic location that is nearest to the user.  
Solution: You include the use of Azure Redis Cache in your design. Does the solution meet the goal?</b>
- Yes.
- No.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

<b>18. The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements:  
You are configuring a web app that delivers streaming video to users. The application makes use of continuous integration and deployment. You need to ensure that the application is highly available and that the users streaming experience is constant. You also want to configure the application to store data in a geographic location that is nearest to the user.  
Solution: You include the use of an Azure Content Delivery Network (CDN) in your design. Does the solution meet the goal?</b>
- Yes.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- No.

<b>19. The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements:  
You are configuring a web app that delivers streaming video to users. The application makes use of continuous integration and deployment. You need to ensure that the application is highly available and that the users streaming experience is constant. You also want to configure the application to store data in a geographic location that is nearest to the user.  
Solution: You include the use of a Storage Area Network (SAN) in your design. Does the solution meet the goal?</b>
- Yes.
- No.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

<b>20. You develop a Web App on a tier D1 app service plan. You notice that page load times increase during periods of peak traffic. You want to implement automatic scaling when CPU load is above 80 percent. Your solution must minimize costs. What should you do first?</b>
- Enable autoscaling on the Web App.
- Switch to the Premium App Service tier plan.
- Switch to the Standard App Service tier plan.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Switch to the Azure App Services consumption plan.

"Configure the web App to the Standard App Service Tier. The Standard tier supports auto-scaling, and we should minimize the costs. We can then enable autoscaling on the web app, add a scale rule and add a Scale condition."

<b>21. Your company's Azure subscription includes an Azure Log Analytics workspace. Your company has a hundred on-premises servers that run either Windows Server 2012 R2 or Windows Server 2016, and is linked to the Azure Log Analytics workspace. The Azure Log Analytics workspace is set uo to gather performance counters associated with security from these linked servers. You must configure alerts based on the information gathered by the Azure Log Analytics workspace. You have to make sure that alert rules allow for dimensions, and that alert creation time should be kept to a minimum. Furthermore, a single alert notification must be created when the alert is created and when the alert is resolved. You need to make use of the necessary signal type when creating the alert rules. Which of the following is the option you should use?</b>
- The Activity log signal type.
- The Application Log signal type.
- The Metric signal type.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- The Audit Log signal type.

"Metric alerts in Azure Monitor provide a way to get notified when one of your metrics cross a threshold. Metric alerts work on a range of multidimensional platform metrics, Application Insights standard and custom metrics. Note: Signals are emitted by the target resource and can be of several types. Metric, Activity log, Application Insights and Log."

<b>22. Your are developing a .NET Core MVC application that allows customers to research independent holiday accommodation providers. You want to implement Azure Search to allow the application to search the index by using various criteria to locate documents related to accommodation. You want the application to allow customers to search the index by using regular expressions. What should you do?</b>
- Configure the SearchMode property of the SeachParameters class.
- Configure the QueryType property of the SearchParameters class.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Configure the Facets property of the SearchParameters class.
- Configure the Filter property of the SearchParamenters class.

"The SearchParameters QueryType Property gets or sets a value that specifies the syntax of the search query. The default is 'simple'. Use 'full' if your query uses the Lucene query syntax. You can write queries against Azure Search based on the rich Lucene Query Parser syntax for specialized query forms: wildcard, fuzzy search, proximity search, regular expressions are a few examples."

<b>23. You are a developer at your company. You need to update the definitions for an existing Logic App. What should you use?</b>
- The Enterprise Integration Pack (EIP).
- The Logic App Code View.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- The API Connections.
- The Logic Apps Designer.

"Edit JSON Azure Portal:  
1. Sign in to the Azure Portal.  
2. From the left menu, choose All services. In the search box, find "logic apps", and then from the results, select you logic app.  
3. On your logic app's menu, under Development Tools, select Logic App Code View.  
4. The Code View editor opens and shows your logic app definition in JSON format."

<b>24. The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements:  
You are developing a solution for a public facing API. The API back end is hosted in an Azure App Service instance. You have implemented a RESTful service for the API back end. You must configure back-end authentication for the API Management service instance.  
Solution: You configure Basic gateway credentials for the Azure resource. Does the solution meet the goal?</b>
- Yes.
- No.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"API Management allows to secure access to the back-end service of an API using client certificates."

<b>25. The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements:  
You are developing a solution for a public facing API. The API back end is hosted in an Azure App Service instance. You have implemented a RESTful service for the API back end. You must configure back-end authentication for the API Management service instance.  
Solution: You configure Client cert gateway credentials for the HTTP(s) endpoint. Does the solution meet the goal?</b>
- Yes.
- No.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b></b>

"The API back end is hosted in an Azure App Service instance. It is an Azure resource and not an HTTP(s) endpoint."

<b>26. The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements:  
You are developing a solution for a public facing API. The API back end is hosted in an Azure App Service instance. You have implemented a RESTful service for the API back end. You must configure back-end authentication for the API Management service instance.  
Solution: You configure Basic gateway credentials for the HTTP(s) endpoint. Does the solution meet the goal?</b>
- Yes.
- No.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b></b>

"API Management allows to secure access to the back-end service of an API using client certificates. Furthermore, the API back end is hosted in an Azure App Service instance. It is an Azure resource and not an HTTP(s) endpoint."

<b>27. The question is included in a number of questions that depicts the identical set-up. However, every question has a distinctive result. Establish if the solution satisfies the requirements:  
You are developing a solution for a public facing API. The API back end is hosted in an Azure App Service instance. You have implemented a RESTful service for the API back end. You must configure back-end authentication for the API Management service instance.  
Solution: You configure Client cert gateway credentials for the Azure resource. Does the solution meet the goal?</b>
- Yes.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b></b>
- No.

"API Management allows to secure access to the back-end service of an API using client certificates."

<b>28. </b>
<b></b>
<b></b>
<b></b>
