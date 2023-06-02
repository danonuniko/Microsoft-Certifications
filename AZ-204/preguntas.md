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
- 10.
- 30. 
- Min Value.
- Max Value.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
  
"The number os fault domains for managed availability sets varies by region - either two or three per region."

<b>7. Your company has an Azure subscription. You need to deploy a number of Azure virtual machines to the subscription by using Azure Resource Manager (ARM) templates. The virtual machines will be included in a single availability set. You need to ensure that the ARM template allows for as many virtual machines as possible to remain accessible in the event of fabric failure or maintenance. Which of the following is the value that you should configure for the platformUpdateDomainCount property?</b>
- <label>10.</label>
- 20.
- 30.
- 40.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

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

<b>13. </b>

