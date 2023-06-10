<h2 align="center"><ins>PREGUNTAS AZ-204 RUTAS MICROSOFT LEARN</ins></h2><br>

<b>1. ¿Cuál de las siguientes categorías de plan de App Service proporciona las capacidades máximas de escalabilidad horizontal?</b>
- Proceso dedicado.
- Aislado.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Proceso compartido.

"La categoría Aislado proporciona aislamiento de red y proceso, y tiene la capacidad máxima de escalabilidad horizontal."

<b>2. ¿Cuál de las siguientes características de red de App Service puede usarse para controlar el tráfico de red saliente?</b>
- Dirección asignada a las aplicaciones.
- Conexiones híbridas.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Puntos de conexión del servicio.

"Las conexiones híbridas son una característica de red saliente."

<b>3. ¿En cuál de las siguientes categorías de configuración de la aplicación establecería el idioma y la versión del SDK?</b>
- Configuración de la aplicación. **ERROR AL CONTESTAR:** Esta categoría se una para configurar opciones que pasan a la aplicación en el entorno de ejecución.
- Asignaciones de ruta de acceso.
- Configuración general.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"La categoría de configuración general se usa para configurar las opciones de pila, la plataforma, la depuración y el certificado de cliente entrante."

<b>4. ¿Cuál de los siguientes tipos de registro de aplicaciones se admite en la plataforma Linux?</b>
- Registro del servidor web.
- Seguimiento de solicitudes con error.
- Registro de implementación.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

<b>5. ¿Cuál de estas afirmaciones describe mejor el escalado automático?</b>
- El escalado automático requiere la supervisión activa de la carga de trabajo de un sistema por parte de un administrador.
- El escalado automático es una solución para escalar y reducir horizontalmente.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- El escalado vertical y la reducción vertical proporcionan una mejor disponibilidad que el escalado automático.

"El sistema puede escalar horizontalmente cuando las métricas de recursos especificadas indican un aumento del uso y reducir horizontalmente cuando estas métricas disminuyan."

<b>6. ¿Cuál de estos escenarios sería adecuado para el escalado automático?</b>
- El número de usuarios que requieren acceso a una aplicación varía según una programación periódica. Por ejemplo, más usuarios usan el sistema los viernes que otros días de la semana.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- El sistema está sujeto a un flujo repentino de solicitudes que hace que el sistema se detenga.
- Su organización ofrece una promoción y espera ver un aumento del tráfico en el sitio web durante las próximas dos semanas.

"Los cambios en la carga de la aplicación que son predecibles son buenos candidatos para el escalado automático."

<b>7. De forma predeterminada todas las solicitudes que realiza el cliente a la direción URL de producción de la aplicación (http://<app_name>.azurewebsites.net) se enrutan al espacio de producción. Se puede enrutar automáticamente parte del tráfico a otra ranura. ¿Cuál es la regla de enrutamiento predeterminada que se aplica a las nuevas ranuras de implementación?</b>
- 0%.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- 10%.
- 20%.

"De forma predeterminada, a las ranuras nuevas se les da una regla de enrutamiento de 0%."

<b>8. Algunos elementos de configuración siguen al contenido en los intercambios (no son específicos de la ranura), mientras que otros permanecen en la misma ranura después de este (específicos). ¿Cuáles de los siguientes valores se intercambian?</b>
- Extremos de publicación.
- Contenido de WebJobs.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Programadores de WebJobs.

<b>9. ¿Cuál de las siguients opciones de hospedaje de Azure Functions es mejor cuando se requiere poder predecir el escalado y los costos?</b>
- Plan Premium de Functions.
- Plan dedicado.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Plan de consumo.

"Los planes dedicados se ejecutan en App Service, que admite la configuración de reglas de escalado automático en función del uso predictivo."

<b>10. Una organización quiere implementar un flujo de trabajo sin servidor para resolver un problema empresarial. Uno de los requisitos e que la solución debe usar un modelo de desarrollo orientado al diseñador (declarativo). ¿Cuál de las opciones siguientes cumple los requisitos?</b>
- Azure Functions.
- Azure Logic Apps.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Trabajos Web.

"Azure Logic Apps permite cargas de trabajo sin servidor y usa un modelo de desarrollo orientado al diseñador (declarativo)."

<b>11. ¿Cuál de las siguientes opciones es necesaria para que se ejecute una función?</b>
- Enlace.
- Desencadenador.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Desencadenadores y enlaces.

"Un desencadenador define cómo se invoca una función y cada función debe tener exactamente un desencadenador."

<b>12. ¿Cuál de las siguientes opciones admite las configuraciones de dirección in y out?</b>
- Enlaces.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Desencadenador.
- Valor de conexión.

<b>13. ¿Cuál de los siguientes tipos de blobs se usa para almacenar archivos de disco duro virtual?</b>
- Blobs en bloques.
- Blobs en anexos.
- Blobs en páginas.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"Los blobs en páginas almacenan archivos de acceso aleatorio de hasta 8 TB de tamaño y se usan para almacenar archivos de unidad de disco duro virtual (VHD). También sirven como discos para máquinas virtuales de Azure."

<b>14. ¿Cuál de los siguientes tipos de cuentas de almacenamiento se recomienda para la mayoría de los escenarios que usan Azure Storage?</b>
- Uso general v2.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Uso general v1.
- FileStorage.

"Este tipo admite blobs, archivos, colas y tablas. Se recomienda para la mayoría de los escenarios que usan Azure Storage."

<b>15. ¿Qué nivel de acceso se considera sin conexión y no se puede leer ni modificar?</b>
- Acceso esporádico.
- Archivo.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Acceso frecuente.

"Los blobs de nivel de archivo deben rehidratarse a los niveles esporádico o frecuente para poder leerse o modificarse."

<b>16. ¿Cuál de los siguientes tipos de cuenta de almacenamiento admite directivas de ciclo de vida?</b>
- General Purpose v1.
- General Purpose v2.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- FileStorage.

"La administración del ciclo de vida de Azure Blob Storage ofrece una directiva enriquecida basada en reglas para cuentas de almacenamiento de blobs y de uso general v2."

<b>17. ¿Cuál de los siguientes encabezados HTTP estándar se admite para contenedores y blobs al establecer propiedades mediante REST?</b>
- Last-Modified.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Content-Length.
- Origen.

"Last-Modified se admite tanto para contenedores como para blobs."

<b>18. ¿Cuál de las siguientes clases de la biblioteca cliente de Azure Storage para .NET permite manipular los contenedores de Azure Storage y sus blobs?</b>
- BlobCient.
- BlobContainerClient.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- BlobUriBuilder.

"BlobContainerClient se puede usar para manipular contenedores y blobs."

<b>19. ¿Cuál de los siguientes niveles de coherencia ofrece el mayor rendimiento?</b>
- Alta.
- Sesión.
- Ocasional.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"El nivel de coherencia Ocasional ofrece el mayor rendimiento a costa de una coherencia más débil."

<b>20. ¿Qué son las unidades de solicitud (RU) en Azure Cosmos DB?</b>
- Una unidad de medida que se usa para expresar el costo de todas las operaciones de base de datos en Azure Cosmos DB.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Unidad de tiempo utilizada para medir la duración de las operaciones de base de datos.
- Unidad de almacenamiento que se usa para medir la cantidad de datos almacenados en Azure Cosmos DB.

"Las RU representan el costo normalizado de todas las operaciones de base de datos en Azure Cosmos DB, incluidas las escrituras, las lecturas puntuales y las consultas."

<b>21. Al definir un procedimiento almacenado en Azure Portal, ¿los parámetros de entrada siempre se envían como tipo al procedimiento almacenado?</b>
- String.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Entero.
- Boolean.

"Al definir un procedimiento almacenado mediante Azure Portal, los parámetros de entrada siempre se envían como una cadena para el procedimiento almacenado."
  
<b>22. ¿Cuál de las siguientes opciones usaría para validar las propiedades de un elemento que se está creando?</b>
- Desencadenador previo.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Desencadenador posterior.
- Función definida por el usuario.

"Los desencadenadores previos se pueden usar para ajustar los datos antes de agregarlos al contenedor."

<br><h2 align="center"><ins>PREGUNTAS AZ-204 FREE EXAMS</ins></h2><br>

<b>1. You manage an Azure App Service web app named app1. App1 is registered as an application in Azure Active Directory (Azure AD). You need to ensure that Azure AD signed-in user information can be retrieved by app1 by using Microsoft Graph. What should you configure?</b>
- appRoles.
- Application permissions.
- GroupMembershipClaims.
- Delegated permissions.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"This item test the candidate's knowlegde of accessing user data from Microsoft Graph, which is part of implementing user authentication and authorization. Delegated permissions are used by apps that have a signed-in user present. For these apps, either the user or an administrator consents to the permissions that the app requests and the app can be assigned to users, groups or service principals. Application permissions are used by apps that run without a signed-in user present. For example, apps that run as background services or daemons. An administrator can only permit application permissions. GroupMembershipClaims is an attribute in the application manifest of the registered application that configures the groups claim issued in a user or OAuth 2.0 access token that the app expects. AppRoles, application permissions and GroupMembershipClaims will not allow signed-in user information to be retrieved in the code."

<b>2. You manage an Azure App Service web app named app1. App1 is registered as a multi-tenant application in an Azure Active Directory (Azure AD) tenant named tenant1. You need to grant app1 the permission to access the Microsoft Graph API in tenant1. Which service principal should you use?</b>
- Legacy.
- System-assigned managed identity.
- Application.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- User-assigned managed identity.

"This item test the candidate's knowlegde of accessing user data from Microsoft Graph, which is part of implementing user authentication and authorization. An Azure AD application is defined by its one and only application object, which resides in the Azure AD tenant where the application was registered (known as the application's home tenant). The application service principal is a legacy app, which is an app created before app registrations were introduced or an app created through legacy experiences. Managed identities eliminate the need to manage credentials in code. A system-assigned managed identity is restricted to one per resource and is tied to the lifecycle of the resource. Managed identities for Azure resources eliminate the need to manage credentials in code. A user-assigned managed identity can be created and assigned to one or more instances of an Azure service. The legacy, system-assigned managed identity, and user-assigned managed identity cannot be used to assign permission for app1 in tenant1 to access the Microsoft Graph API."

<b>3. You develop a multitenant web application named App1. You plan to register App1 with multiple Azure Active Directory (Azure AD) tenants. You need to identify the relationship between the application objects and security principals associated with App1. Which relationship should you identify?</b>
- App1 will have multiple application objects and multiple service principals.
- App1 will have multiple application objects and a single service principal.
- App1 will have a single application object and multiple service principals.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- App1 will have a single application object and a single service principal.

"This item tests the candidate's knowledge of configuring authentication of multitenant applications, which is a common scenario when implementing authentication. App1 will have a single application object and multiple service principals."

<b>4. You plan to generate a shared access signature (SAS) token for read access to a blob in a storage account. You need to secure the token from being compromised. What should you use?</b>
- Primary account key.
- Secondary account key.
- Azure AD credentials assigned the Contributor role.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Azure AD credentials assigned the Reader role.

"This item test the candidate's knowledge of Azure Storage shared access signatures (SAS). Azure AD credentials are required to generate the SAS token. The account used must have the Microsoft.Storage/storageAccounts/blobServices/generateUserDelegationKey permission, which is present in the following built-in roles: Contributor, Storage Account Contributor, Storage Blob Data Contributor, Storage Blob Data Owner, Storage Blob Data Reader and Storage Blob Delegator. The account key can be used to generate the SAS token, but it can be more easily compromised."

<b>5. You have 10 applications running in Azure App Service. You need to ensure the applications have access to items stored in Azure App Configuration by using a common configuration. Passwords or keys must not be used. Which solution should you use?</b>
- System-assigned managed identities.
- User-assigned managed identity.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Service principal with permissions to Azure App Configuration.
- Developer's credentials in code.

"This item test the candidate's knowlegde of managed identities. User-assigned managed identities are a way to reuse the permissions across applications. User-assigned managed identities associate the managed identity to the new applications, with no keys or passwords. System-assigned managed identities use a new identity for each application, which does not meet the common configuration requirement. A service principal has keys that no need to be rotated. The developer does not run the application, so the developer's identity cannot be assumed."

<b>6. You need to group keys in Azure App Configuration. What are two possible ways to achieve this goal?</b>
- Use Azure role-based access control. Grant the Read permission to read keys that belong to the application.
- Organize keys by using key prefixes.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Use managed identity. Grant the Read permission to read keys that belong to the application.
- Organize keys by using labels.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"This item test the candidate's knowledge of best practices when working with keys in Azure App Configuration. Key prefixes are the beginning parts of keys. A set of keys can be grouped by using the same prefix in names. Labels are an attribute on keys. Labels are used to create variants of a key. For example, labels can be assigned to multiple versions of a key. Authorizing role-based access control to read Azure App Configuration is not a valid way to group keys. Authorizing a managed identity to read Azure App Configuration is not a valid way to group keys."

<b>7. You plan to create a key namespace hierarchy in Azure App Configuration. You need to separate individual key names. Which character should you use?</b>
- :  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- \*
- ,
- \

"This item tests the candidate's knowledge of configuring key namespace hierarchy of App Configuration, which is part of implementing secure cloud solutions. The colon character (:) is used to separate names of individual keys when creating a namespace hierarchy in Azure App Configuration. The asterisk character (*) is one of reserved characters in Azure App Configuration, so it cannot be used to separate names of individual keys when creating a namespace hierarchy in Azure App Configuration. The comma character (,) is one of reserved characters in Azure App Configuration, so it cannot be used to separate names of individual keys when creating a namespace hierarchy in Azure App Configuration. The backslash character (\\) is one of reserved characters in Azure App Configuration, so it cannot be used to separate names of individual keys when creating a namespace hierarchy in Azure App Configuration."

<b>8. You need to generate a new version of a key stored in Azure Key Vault. Which code segment should you use?</b>
- az keyvault key rotation-policy update -n mykey --vault-name mykeyvault --value path/to/policy.json
- az keyvault key purge --name mykey -vault-name mykeyvault
- az keyvault key rotate --vault-name mykeyvault --name mykey  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- az keyvault key set-attributes --vault-name mykeyvault --name mykey -policy path/to/policy.json

"This item tests the candidate's knowledge of setting key rotation by using Azure CLI. The **Rotate** operation will generate a new version of the key based on the key policy. The **Rotation Policy** operation updates the rotation policy of a key vault key. The **Purge Deleted Key** operation is applicable for soft-delete enabled vaults or HSMs. The **Set Attributes** operation changes specified attributes of a stored key."

<b>9. You have an Azure App Configuration instance named AppConfig1 and an Azure key vault named KeyVault1. You plan to encrypt data stored in AppConfig1 by using your own key stored in KeyVault1. You need to grant permissions in KeyVault1 to the identity assigned to AppConfig1. Which three key-specific permissions should you use?</b>
- DECRYPT.
- ENCRYPT.
- GET.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- UNWRAP.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- WRAP.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"This item tests the candidate's knowledge of implementing bring your own key encryption scenarios, which is an essential part of implementing secure cloud solutions. To use the custom key stored in KeyVault1, the identity assigned to AppConfig1 needs to have GET, WRAP and UNWRAP permissions to the custom key. The DECRYPT and ENCRYPT permissions are not required to use the custom key stored in KeyVault1 in this scenario."

<b>10. You have an Azure Storage account container named container1. You need to configure access to the container to meet the following requirements:
- The shared access signature (SAS) token should be secured with Azure Active Directory (Azure AD) credentials.
- Role-based access control (RBAC) should be used.
- The SAS token should support granting access to containers.
Which type of SAS should you use?</b>
- Account.
- User delegation.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Service.
- Stored access policy.

"This item tests the candidate's knowledge of securing an Azure Storage account, which is part of developing solutions that use blob storage. User delegation SAS fulfills all the requirements, including securing the SAS token with Azure AD credentials, RBAC support and granting access to containers. Azure Storage supports creating a new type of SAS at the level of the storage account. A service SAS delegates access to a resource in just one of the storage services (i.e. Blob Queue, Table or File). A stored access policy serves to group shared access signatures and to provide additional restrictions for signatures that are bound by the policy. The account, service and stored access policy SAS types do not fulfill the requirement of securing the SAS token with Azure AD credentials and RBAC support to manage permissions."

<b>11. You are developing a solution that stores secrets in an Azure Key Vault named myvault. You need to retrieve the value for a secret named mysecret that is stored in myvault. Which CLI command should you use?</b>
- az keyvault secret recover --name mysecret --vault-name myvault
- az keyvault secret recover --id myvault/mysecret
- az keyvault secret show --id myvault/mysecret
- az keyvault secret show --name mysecret --vault-name myvault  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"This item tests the candidate's knowlegde of developing code that uses keys, secrets and certificates stored in Azure Key Vault. The CLI comand **az keyvault** offers several commands to work with secrets. The most commonly used commands are **set** for storing a secret and **show** to get the secret's value. When using these commands,either an id specifying the full secret identification (in the format **https://<keyvaultname>.vault.azure.net/secrets/<secret-name>/<secret-version>**) or the secret and the vault name must be specified."

<b>12. You need to create a container in a container group and mount an Azure file share as volume. Which code segment should you use?</b>
- az container create -g MyResourceGroup --name myapp --image myimage:latest --command-line "cat /mnt/azfile/myfile" --azure-file-volume-share-name myshare --azure file-volume-account-name mystorageaccount --azure-file-volume-account-key mystoragekey --azure-file-volume-mount-path /mnt/azfile  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- az container create -g MyResourceGroup --name myapp --image myimage:latest --command-line "cat /mnt/azfile/myfile" --azure-file-volume-share-name myshare --azure file-volume-account-name mystorageaccount --azure-file-volume-account-key mystoragekey --secrets-mount-path /mnt/azfile
- az container create -g MyResourceGroup --name myapp --image myimage:latest --command-line "cat /mnt/azfile/myfile" --azure file-volume-account-name mystorageaccount --azure-file-volume-account-key mystoragekey --azure-file-volume-mount-path /mnt/azfile
- az container create -g MyResourceGroup --name myapp --image myimage:latest --command-line "cat /mnt/azfile/myfile" --azure file-volume-account-name mystorageaccount --azure-file-volume-account-key mystoragekey --secrets-mount-path /mnt/azfile

"This item tests the candidate's knowlegde of running containers by using Azure Container Instances. The code segment that includes the **--azure-file-volume-mont-path** parameter and the **--azure-file-volume-share-name** parameter creates a container in a conteiner group and mounts an Azure file share as volume. The code segment that include the **--secrets-mount-path** parameter will not mount an Azure file share as volume. The code segment that does not include the **--azure-file-volume-share-name** is invalid."

<b>13. You manage an Azure App Service web app named app1. App1 uses a service plan based on the Basic pricing tier. You need to create a deployment slot for app1. What should you do first?</b>
- Scale out app1.
- Scale up app1.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Configure automated deployment of app1 with Azure DevOps.
- Configure automated deployment of app1 with GitHub.

"This item tests the candidate's knowledge of creating deployment slots, which ties directly to the pricing tier used by Azure App Service web apps. This is configured as part of the Azure Service web app creation. Deployment slots require at a minimum the Standard pricing tier, so to supply support for app1, it is necessary to scale it up. Scaling out app1 provisions more instances of app1, but it does not provide the ability to create its deployment slot. Automated deployment of app1 with Azure DevOps or GitHub is not a prerequisite of support for deployment slots, but it commonly is the reason for implementing them."

<b>14. You manage the staging and production deployment slots of an Azure App Service web app named app1. You need to ensure a connection string is not swapped when swapping is performed. Which configuration should you use?</b>
- Deployment Center.
- Deployment slot setting.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Managed identity.
- Scale up.

"This item tests the candidate's knowledge of deploying code to Azure App Service, which is part of creating Azure App Service Web Apps. Marking a setting as a deployment slot setting keeps it sticky to that deployment slot. For example, an app setting marked as a deployment slot setting on app1 will always stick with app1 and will never move to app1/staging during a swap. The Deployment Center setting is used to configure continuous deployment and manual deployment. Managed identity provides an identity for applications to use when connecting to resources that support Azure Active Directory authentication. Scale up will ensure the web app is entitled to get CPU, memory, disk space and extra features such as dedicated virtual machines, custom domains and certificates, staging slots and autoscaling. Deployment Center, Managed Identity and Scale up cannot be used to ensure a connecting string is not swapped when swapping is performed."

<b>15. You need to configure a web app to allow external requests from https://myapps.com. Which Azure CLI command should you use?</b>
- az webapp cors add -g MyResourceGroup -n MyWebApp --allowed-origins https://myapps.com  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- az webapp identity add -g MyResourceGroup -n MyWebApp --allowed-origins https://myapps.com
- az webapp traffic-routing set --distribution myapps=100 --name MyWebApp --resource-group MyResourceGroup
- az webapp config access-restriction add -g MyResourceGroup -n MyWebApp --rule-name external --action Allow -ids myapps --priority 200

"This item tests the candidate's knowledge of configuring web app settings. The code segment that includes the **cors add** will configure CORS to allow requests from https://myapps.com. The code segment that includes **identity** add will add a managed identity to a web app. The code segment that includes **traffic-routing-set** will configure a traffic routing to a deployment slot named myapps. The code segment that includes **access-restriction add** will add an access restriction on a web app."

<b>16. You manage a multi-instance deployment of an Azure App Service web app named app1. You need to ensure a client application is routed to the same instance for the life of the session. Which platform setting should you use?</b>
- WebSocket.
- Always on.
- HTTP version.
- ARR Affinity.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"This item tests the candidate's knowledge of configuring web app settings, which is part of creating Azure App Service Web Apps. In a multi-instance deployment, the ARR Affinity setting ensures a client application is routed to the same instance for the life of the session. WebSocket is a standardized protocol that provides full-duplex communication. Always on keeps the app loaded even when there is no traffic. In HTTP/2, a persistent connection can be used to service multiple simultaneous requests. WebSocket, Always on and HTTP version are not used to ensure a client application is routed to the same instance for the life of the session."

<b>17. A company plans to implement a Microsoft Defender for Cloud solution. The company has the following requirements:
- Notifies when DNS domains are not deleted when a new function app is deleted.
- Use native alerting.
- Minimize costs.

You need to select a hosting plan. Which hosting plan should you use?</b>
- Consumption.
- Basic.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Premium.
- Free.

"This item tests the candidate's knowlegde about securing Azure Functions. The Basic plan supports both custom domains and Microsoft Defenter for Cloud, which can automatically alert on dangling DNS domains. The Consumption plan is incorrect because it does not support Microsoft Defender for Cloud. This can automatically alert on dangling DNS domains. The Premium plan supports custom domains and Microsoft Defender for Cloud, which can automatically alert on dangling DNS domains. This, however is not the lowest cost option. The Free plan does not support custom domains, although it does support Microsfot Defender for Cloud, which can automatically alert on dangling DNS domains."

<b>18. You have an Azure Key Vault named MyVault. You need to use a key vault reference to access a secret named MyConnection from MyVault. Which code segment should you use?</b>
- @Microsoft.KeyVault(Secret=MyConnection;VaultName=MyVault)
- @Microsoft.KeyVault(SecretName=MyConnection;VaultName=MyVault)  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- @Microsoft.KeyVault(Secret=MyConnection;Vault=MyVault)
- @Microsoft.KeyVault(SecretName=MyConnection;Vault=MyVault)

"This item tests the candidate's knowledge of retrieving secrets from Key Vault in Azure Functions. The code segment **@Microsoft.KeyVault(SecretName=MyConnection;VaultName=MyVault)** reads the secret from Key Vault. The code segment that includes **Secret** or **Vault** uses invalid parameters."

<b>19. You plan to create a C# script-based Azure function app. You need to configure the trigger and bindings for the functions of the function app. What should you do?</b>
- Create a function.json file for each function.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Create a host.json file for the function app.
- Decorate methods of each function with C# attributes.
- Decorate parameters of each function with C# attributes.

"This item tests the candidate's knowledge of configuring triggers and bindings. When using scripting languages, such as C# script, the function.json file for each function contains its triggers and bindings, and it needs to be explicitly created. The file host.json has runtime-specific configurations, not definitions of triggers and bindings. Decorating methods and Decorating parameters are used to define triggers and bindings when using compiled languages, not scripted ones."

<b>20. A container group in Azure Container Instances has multiple containers. The containers must restart when the process executed in the container group terminates due to an error. You need to define the restart policy for the container group. Which Azure CLI command should you use?</b>
- az container restart \ --name mycontainer \ --resource-group myResourceGroup \ --no-wait
- az container create \ --resource-group myResourceGroup \ --name mycontainer \ --image mycontainerimage \ --restart-policy Always
- az container create \ --resource-group myResourceGroup \ --name mycontainer \ --image mycontainerimage \ --restart-policy Never
- az conteiner create \ --resource-group myResourceGroup\ --name mycontainer \ --image mycontainerimage \ --restart-policy OnFailure  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>

"This item tests the candidate's knowledge of running containers by using Azure Container Instances (ACI). Configurable restart policies can be specified for a container group in ACI. A configurable restart policy allows you to specify that containers are stopped when their processes have completed. When you create a container group in ACI, you can specify one of three restart policy settings: Always, Never and OnFailure. If the --restart-policy is mentioned as OnFailure, the containers in the container group are restarted only when the process executed in the container fails (when it terminates with a nonzero exit code). If the --restart-policy is mentioned as Always, the containers in the container group are always restarted irrespective of the success or failure of process execution in a container. If the --restart-policy is mentioned as Never, the containers in the container group will only run at most once. The az container restart command is used to restart all the containers in a container group, not to define a restart policy for a container group."

<b>21. You are developing a Linyx web app on Azure App Service. You need to deploy the web app to the production environment based on the following requirements:
- App changes must be validated in an environment identical to the production environment before moving the app to the production environment.
- Downtime must be eliminated when the app is deployed to the production environment.  

What should you use?</b>
- Deployment slots.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- Auto-scaling.
- Hybrid connection.
- App cloning.

"This item tests the candidate's knowledge of when to use deployment slots. Deployment slots are live apps with unique host names, which allow swapping configuration and content between them. Auto-scaling is a feature that allows adding more capacity to a function app hosting environment. This capacity can be added to an individual hosting environment (for example, scaling up or adding memory or CPU), or adding more hosts (scaling out). The scaling can be trigerred based on a schedule or when breaching thresholds defined for certain metrics. Hybrid connections are available for consuming on-premises apps without needing to expose them to the internet. App cloning is a process to obtain an existing app and copy it to another destination, which can be a new app or a deployment slot, for example. However, this is not supported on Linyx apps."

<b>22. You develop an App Service app hosted on Windows Platform. Users report that the app is failing. You need to begin troubleshoosting the app by inspecting a copy of the page that is returned when the HTTP return code is greater than 400. Which type of log should you review?</b>
- application.
- web server.
- detailed error.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- deployment.

"This item tests the candidate's knowledge of using logs to troubleshoot web apps. The detailed error log contains copies of the error pages, produced in reponse to HTTP codes greater than 400, that would have been sent to clients. These pages are not sent due to security reasons. The web server log shows information about the raw HTTP requet, such as method, bytes and client user agent. The application log is application specific, logging information that your application code or components that are used by your application writes. The deployment log stores information to diagnose the reasons for a failed deployment."

<br><h2 align="center"><ins>PREGUNTAS AZ-204 EXAMTOPICS</ins></h2><br>
<h3 align="center"><ins>QUESTION SET 1</h3><br>

<b>1. You have two Hyper-V hosts named Host1 and Host2. Host1 has an Azure virtual machine named VM1 that was deployed by using a custom Azure Resource Manager template. You need to move VM1 to Host2. What should you do?</b>
- From the Update management blade, click Enable.
- From the Overwiew blade, move VM1 to a different subscription.
- From the Redeploy blade, click Redeploy.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b>
- From the Profile blade, modify the usage location.

"When you redeploy a VM, it moves the VM to a new node within the Azure infrastructure and the powers it back on, retaining all your configuration options and associated resources."SET 1

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

<b>28. You are developing a .NET Core MVC application that allows customers to research independent holiday accommodation providers. You want to implement Azure Search to allow the application to search the index by using various criteria to locate documents related to accommodation venues. You want the application to list holiday accommodation venues that fall within a specific price range and are within a specified distance to an airport. What should you do?</b>
- Configure the SearchMode property of the SearchParameters class.
- Configure the QueryType property of the SearchParameters class.
- Configure the Facets property of the SearchParameters class.
- Configure the Filter property of the SearchParameters class.  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b></b>

"The Filter property gets or sets the OData $filter expression to apply to the search query."

<b>29. You are a developer at your company. You need to edit the workflows for an existing Logic App. What should you use?</b>
- The Enterprise Integration Pack (EIP).  &emsp; &emsp; &emsp; &emsp; <b>CORRECTO</b></b>
- The Logic App Code View.
- The API Connections.
- The Logic Apps Designer.

"For business-to-business (B2B) solutions and seamless communication between organizations, you can build automated scalable enterprise integration workflows by using the Enterprise Integration Pack (EIP) with Azure Logic App."

<b>30. You are a developer for a company that provides a bookings management service in the tourism industry. You are implementing Azure Search for the tour agencies listed in your company's solution. You create the index in Azure Search. You now need to use the Azure Search .NET SDK to import the relevant data into the Azure Search service. Which three actions should you perform in sequence?</b>
- Create a DataSource instance and set its Container property to the DataContainer.
- Create an IndexBatch that contains the documents which must be added.  &emsp; &emsp; &emsp; &emsp; <b>STEP 2</b></b>
- Set the DataSources property of the SearchServiceClient.
- Create a SearchIndexClient object to connect to the search index. &emsp; &emsp; &emsp; &emsp; <b>STEP 1</b></b>
- Call the Documents.Index method of the SearchIndexClient and pass the IndexBatch. &emsp; &emsp; &emsp; &emsp; <b>STEP 3</b></b>
- Call the Documents.Seggest method of the SearchIndexClient and pass the DataSource.

"1. The index needs to be populated. To do this, we will need a SearchIndexClient. Thre are to ways to obtain one: by constructing it, or by calling Indexex.GetClient on the SearchServiceClient. Here we will use the first method.  
2. Create the indexBatch with the documents.  
Something like:  
var hotels = new Hotel[];  
{  
new Hotel()  
{  
HotelId = "3",  
BaseRate = 129.99,  
Description = "Close to town hall and the river"  
}  
};  
var batch = IndexBatch.Upload(hotels);  
3. The next step is to populate the newly-created index  
Example:  
var batch = IndexBatch.Upload(hotels);  
try  
{  
indexClient.Documents.Index(batch);  
}  

<b>31. You are developing an application that applies a set of governance policies for internal and external services, as well as for applications. You develop a stateful ASP.NET Core 2.1 web application named PolicyApp and deploy it to an Azure App Service Web App. The PolicyApp reacts to events from Azure Event Grid and performs policy actions based on those events. You have the following requirements:
- Authentication events must be used to monitor users when they sign in and sign out.
- All authentication events must be processed by PolicyApp.
- Sign outs must be processed as fast as possible.  
What should you do?</b>
- Create a new Azure Event Grid subscription for all authentication events. Use the subscription to process sign-out events.
- Create a separate Azure Event Grid handler for sign-in and sign-out events.
- Create separate Azure Event Grid topics and subscriptions for sign-in and sign-out events.
- Add a subject prefix to sign-out events. Create an Azure Event Grid subscription. Configure the subscription to use the subjectBeginsWith filter.

<b>32. You are developing a C++ application that compiles to a native application named process.exe. The application accepts images as input and returns images in one of the following image formats: GIF, PNG, or JPEG. You must deploy the application as an Azure Function. You need to configure the function and host json files. How should you complete the json files?</b>

![question 32](images/question-32.jpg)
![question 32 solution](images/question-32-solution.jpg)

<b>33. You are developing an Azure Static Web app that contains training materials for a tool company. Each tool’s training material is contained in a static web page that is linked from the tool’s publicly available description page. A user must be authenticated using Azure AD prior to viewing training. You need to ensure that the user can view training material pages after authentication. How should you complete the configuration file?</b>

![question 33](images/question-33.jpg)
![question 33 solution](images/question-33-solution.jpg)

<b>34. You are authoring a set of nested Azure Resource Manager templates to deploy Azure resources. You author an Azure Resource Manager template named mainTemplate.json that contains the following linked templates: linkedTemplate1.json, linkedTemplate2.json. You add parameters to a parameters template file named mainTemplate.parameters.json. You save all templates on a local device in the C:\templates\ folder.  
You have the following requirements:
- Store the templates in Azure for later deployment.
- Enable versioning of the templates.
- Manage access to the templates by using Azure RBAC.
- Ensure that users have read-only access to the templates.
- Allow users to deploy the templates.  
You need to store the templates in Azure. How should you complete the command? </b>

![question 34](images/question-34.jpg)
![question 34 solution](images/question-34-solution.jpg)

<b>35. You are developing a service where customers can report news events from a browser using Azure Web PubSub. The service is implemented as an Azure Function App that uses the JSON WebSocket subprotocol to receive news events. You need to implement the bindings for the Azure Function App. How should you configure the binding?</b>

![question 35](images/question-35.jpg)
![question 35 solution](images/question-35-solution.jpg)

<b>36. You are building a software-as-a-service (SaaS) application that analyzes DNA data that will run on Azure virtual machines (VMs) in an availability zone. The data is stored on managed disks attached to the VM. The performance of the analysis is determined by the speed of the disk attached to the VM. You have the following requirements:
- The application must be able to quickly revert to the previous day’s data if a systemic error is detected.
- The application must minimize downtime in the case of an Azure datacenter outage.  
You need to provision the managed disk for the VM to maximize performance while meeting the requirements. Which type of Azure Managed Disk should you use?</b>

![question 36](images/question-36.jpg)
![question 36 solution](images/question-36-solution.jpg)

<b>37. You are developing an application that includes two Docker containers. The application must meet the following requirements:
- The containers must not run as root.
- The containers must be deployed to Azure Container Instances by using a YAML file.
- The containers must share a lifecycle, resources, local network, and storage volume.
- The storage volume must persist through container crashes.
- The storage volume must be deployed on stop or restart of the containers.  
You need to configure Azure Container Instances for the application. Which configuration values should you use?</b>

![question 37](images/question-37.jpg)
![question 37 solution](images/question-37-solution.jpg)

<h3 align="center"><ins>QUESTION SET 2</h3>

<b>1. You are implementing a software as a service (SaaS) ASP.NET Core web service that will run as an Azure Web App. The web service will use an on-premises SQL Server database for storage. The web service also includes a WebJob that processes data updates. Four customers will use the web service.
- Each instance of the WebJob processes data for a single customer and must run as a singleton instance.
- Each deployment must be tested by using deployment slots prior to serving production data.
- Azure costs must be minimized.
- Azure resources must be located in an isolated network.  
You need to configure the App Service plan for the Web App. How should you configure the App Service plan? </b>

![question 2-1](images/question-2-1.jpg)
![question 2-1 solution](images/question-2-1-solution.jpg)

"Number of VM instances: 4 - You are not charged extra for deployment slots.  
Pricing tier: Isolated - The App Service Environment (ASE) is a powerful feature offering of the Azure App Service that gives network isolation and improved scale capabilities. Ti is essentially a deployment of the Azure App Service into a subnet of a customer's Azure Virtual Network (VNet)."

<b>2. You are a developer for a software as a service (SaaS) company that uses an Azure Function to process orders. The Azure Function currently runs on an Azure Function app that is triggered by an Azure Storage queue. You are preparing to migrate the Azure Function to Kubernetes using Kubernetes-based Event Driven Autoscaling (KEDA). You need to configure Kubernetes Custom Resource Definitions (CRD) for the Azure Function.
Which CRDs should you configure? To answer, drag the appropriate CRD types to the correct locations. Each CRD type may be used once, more
than once, or not at all.</b>

![question 2-2](images/question-2-2.jpg)
![question 2-2 solution](images/question-2-2-solution.jpg)

<b>3. You are creating a CLI script that creates an Azure web app and related services in Azure App Service. The web app uses the following variables:
- $gitrpo = https://github.com/Contos/webapp
- $webappname = Webapp1103  
You need to automatically deploy code from GitHub to the newly created web app. How should you complete the script?</b>

![question 2-3](images/question-2-3.jpg)
![question 2-3 solution](images/question-2-3-solution.jpg)

"Box 1: az appservice plan create - The azure group creates command successfully returns JSON result. Now we can use resource group to create app service plan.  
Box 2: az webapp create.  
Box 3: --plan $webappname - with the serviceplan we created in step 1.  
Box 4: az webapp deployment - Continuous delivery with GitHub."