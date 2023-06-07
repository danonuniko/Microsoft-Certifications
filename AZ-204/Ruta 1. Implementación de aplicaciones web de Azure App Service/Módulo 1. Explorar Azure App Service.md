<h1 align="center"><ins>RUTA 1: IMPLEMENTACIÓN DE APLICACIONES WEB DE AZURE APP SERVICE</ins></h1>
<h2 align="center">MÓDULO 1 - EXPLORAR AZURE APP SERVICE</h2>  

### Examen de Azure App Service

Azure App Service es un servicio basado en HTTP para hospedar aplicaciones web, API de REST y back-ends para dispositivos móviles. Puede desarrollar en su lenguaje o marco de programación favorito. Las aplicaciones se ejecutan y escalan fácilmente en los entornos Windows y Linux.

#### Compatibilidad integrada con el escalado automático

En Azure App Service se integra la capacidad de escalar o reducir verticalmente, o bien escalar o reducir horizontalmente. En función del uso de la aplicación web, puede escalar o reducir verticalmente los recursos de la máquina subyacente en la que se hospeda la aplicación web. Los recursos incluyen el número de núcleos o la cantidad de memoria RAM disponible. El escalado o la reducción horizontal es la capacidad de aumentar o disminuir el número de instancias de máquina que ejecutan la aplicación web.

#### Compatibilidad con la integración e implementación continuas

Azure Portal proporciona integración e implementación continuas integradas con Azure DevOps Services, GitHub, Bitbucket, FTP o un repositorio de Git local en la máquina de desarrollo. Conecte su aplicación web con cualquiera de los orígenes anteriores y App Service se encargará del resto mediante la sincronización automática del código y los futuros cambios en el código en la aplicación web.

#### Ranuras de implementación

Cuando implemente la aplicación web, puede usar una ranura de implementación distinta en lugar del espacio de producción predeterminado si su nivel de servicio del plan de App Service es estándar o mejor. Las ranuras de implementación son aplicaciones activas con sus propios nombres de host. Los elementos de contenido y configuraciones de aplicaciones se pueden intercambiar entre dos ranuras de implementación, incluida la ranura de producción.

#### App Service en Linux

App Service también puede hospedar las aplicaciones Web de forma nativa en Linux para las pilas de aplicaciones admitidas. Además, puede ejecutar contenedores de Linux personalizados (también conocidos como Web App for Containers). App Service en Linux admite muchas imágenes integradas específicas del lenguaje. Solo implemente el código. Entre los lenguajes y marcos compatibles se incluyen: Node.js, Java (JRE 8 y JRE 11), PHP, Python, .NET y Ruby. Si el tiempo de ejecución que requiere la aplicación no se admite en las imágenes integradas, puede implementarlo con un contenedor personalizado.

Los lenguajes y sus versiones admitidas se actualizan de forma periódica. Puede recuperar la lista actual mediante el comando siguiente en Cloud Shell.

az webapp list-runtimes --os-type linux

##### Limitaciones
App Service en Linux tiene algunas limitaciones:

- App Service en Linux no se admite en el plan de tarifa Compartido.
- Azure Portal solo muestra las características que funcionan actualmente para las aplicaciones Linux. A medida que se habiliten las características, se activarán en el portal.
- Cuando se implementen en imágenes integradas, el código y el contenido se asignarán a un volumen de almacenamiento para el contenido web, respaldado por Azure Storage. La latencia de disco de este volumen es mayor y más variable que la del sistema de archivos del contenedor. Las aplicaciones que requieran muchos accesos de solo lectura a archivos de contenido pueden beneficiarse de la implementación de contenedores personalizados, que permite colocar los archivos en el sistema de archivos de contenedor en lugar de en el volumen de contenido.

### Examen de los planes de Azure App Service

En App Service, cada aplicación se ejecuta siempre en un plan de App Service. Un plan de App Service define un conjunto de recursos de proceso para que una aplicación web se ejecute. Pueden configurarse una o varias aplicaciones para que se ejecuten en los mismos recursos informáticos (o en el mismo plan de App Service).

Cuando se crea un plan de App Service en una región determinada (por ejemplo, Oeste de Europa), se crea un conjunto de recursos de proceso para ese plan en dicha región. Todas las aplicaciones que coloque en este plan de App Service se ejecutan en estos recursos de proceso según lo definido por el plan de App Service. Cada plan de App Service define:

- Sistema operativo (Windows, Linux)
- Región (oeste de EE. UU., este de EE. UU., etc.)
- Número de instancias de VM
- Tamaño de las instancias de VM (pequeño, mediano, grande)
- Plan de tarifa (Gratis, Compartido, Básico, Estándar, Premium, PremiumV2, PremiumV3, Aislado y AisladoV2)
  
El plan de tarifa de un plan de App Service determina qué características de App Service obtendrá y cuánto paga por el plan. Existen algunas categorías de planes de tarifa:

- Proceso de compartido: Gratis y Compartido, los dos planes básicos, ejecutan una aplicación en la misma VM de Azure que otras aplicaciones de App Service, incluidas las aplicaciones de otros clientes. Estos planes asignan cuotas de CPU a cada aplicación que se ejecuta en los recursos compartidos, y los recursos no se pueden escalar horizontalmente.
- Dedicated compute (Proceso dedicado): Los planes Básico, Estándar,Premium, PremiumV2 y PremiumV3 ejecutan aplicaciones en VM de Azure dedicadas. Solo las aplicaciones del mismo plan de App Service comparten los mismos recursos de proceso. Cuanto mayor sea el plan, más instancias de VM estarán disponibles para la escalabilidad horizontal.
- Aislado: los niveles Aislado y AisladoV2 ejecutan máquinas virtuales de Azure dedicadas en instancias de redes virtuales de Azure dedicadas. Proporciona aislamiento de red, además de aislamiento de proceso a sus aplicaciones. Proporciona las máximas posibilidades de escalabilidad horizontal.

Nota: Los planes de hospedaje Gratis y Compartido de App Service (versión preliminar) corresponden a niveles básicos que se ejecutan en la misma máquina virtual de Azure que otras aplicaciones de App Service. Es posible que algunas aplicaciones pertenezcan a otros clientes. Estos niveles están pensados para su uso exclusivo con fines de desarrollo y pruebas.

#### ¿Cómo se ejecuta y escala mi aplicación?

En los planes Gratis y Compartido, una aplicación recibe minutos de CPU en una instancia de máquina virtual compartida y no se puede escalar horizontalmente. En otros planes, una aplicación se ejecuta y escala de la siguiente manera:

- Una aplicación se ejecuta en todas las instancias de máquina virtual configuradas en el plan de App Service.
- Si hay varias aplicaciones en el mismo plan de App Service, comparten las mismas instancias de VM.
- Si tiene varias ranuras de implementación para una aplicación, todas las ranuras de implementación se ejecutan también en las mismas instancias de VM.
- Si habilita los registros de diagnóstico, realiza copias de seguridad o ejecuta WebJobs, también usan ciclos de CPU y memoria en estas instancias de VM.
  
De esta manera, el plan de App Service es la unidad de escalado de las aplicaciones de App Service. Si el plan está configurado para ejecutar cinco instancias de VM, todas las aplicaciones del plan se ejecutan en las cinco instancias. Si el plan está configurado para el escalado automático, todas las aplicaciones del plan se escalan horizontalmente juntas según la configuración de escalado automático.

#### ¿Qué ocurre si mi aplicación necesita más funcionalidades o características?

El plan de App Service se puede escalar o reducir verticalmente en cualquier momento. Basta con cambiar el plan de tarifa del plan. Si la aplicación está en el mismo plan de App Service con otras aplicaciones, puede que desee mejorar el rendimiento de la aplicación aislando los recursos de proceso. Para hacerlo, puede mover la aplicación a otro plan de App Service.

Puede ahorrar dinero incluyendo varias aplicaciones en un plan de App Service. Sin embargo, dado que todas las aplicaciones del mismo plan de App Service comparten los mismos recursos de proceso, debe conocer la capacidad del plan de App Service existente y la carga prevista para la nueva aplicación.

Aísle la aplicación en un nuevo plan de App Service en los siguientes casos:

- La aplicación consume muchos recursos.
- Quiere escalar la aplicación independientemente de las demás aplicaciones del plan existente.
- La aplicación necesita recursos de una región geográfica diferente.

### Implementación en App Service

Cada equipo de desarrollo tiene requisitos únicos que pueden dificultar la implementación de una canalización de implementación eficaz en cualquier servicio en la nube. App Service admite la implementación automatizada y manual.

#### Implementación automatizada

La implementación automatizada, o la implementación continua, es un proceso que se usa para insertar nuevas características y correcciones de errores en un patrón repetitivo y rápido con un efecto mínimo en los usuarios finales.

Azure admite la implementación automatizada directamente desde varios orígenes. Están disponibles las opciones siguientes:

- Azure DevOps Services: puede insertar el código en Azure DevOps Services, compilarlo en la nube, ejecutar las pruebas, generar una versión a partir del código y, por último, insertar el código en una aplicación web de Azure.
- GitHub: Azure admite la implementación automatizada directamente desde GitHub. Al conectar el repositorio de GitHub a Azure para la implementación automatizada, los cambios que se insertan en la rama de producción en GitHub se implementan automáticamente.
- Bitbucket: con sus similitudes con GitHub, puede configurar una implementación automatizada con Bitbucket.

#### Implementación manual

Hay algunas opciones que puede usar para insertar el código en Azure de forma manual:

- Git: App Service Web Apps incluyen una dirección URL de Git que se puede agregar como repositorio remoto. Al insertar en el repositorio remoto, se implementa la aplicación.
- CLI: webapp up es una característica de la interfaz de la línea de comandos az que empaqueta la aplicación y la implementa. A diferencia de otros métodos de implementación, az webapp up puede crear una aplicación web de App Service de forma automática si todavía no ha creado una.
- Implementación desde un archivo Zip: use curl o una utilidad HTTP similar para enviar un archivo ZIP de los archivos de la aplicación a App Service.
- FTP/S: FTP o FTPS es una manera tradicional de insertar el código en muchos entornos de hospedaje, incluido App Service.

#### Uso de ranuras de implementación

Siempre que sea posible, use ranuras de implementación al implementar una nueva compilación de producción. Cuando se usa un nivel de plan de App Service Estándar o superior, puede implementar la aplicación en un entorno de ensayo y, a continuación, intercambiar los espacios de ensayo y producción. La operación de intercambio prepara las instancias de trabajo necesarias para que coincidan con la escala de producción, lo que elimina el tiempo de inactividad.

### Exploración de la autenticación y autorización en App Service

Azure App Service incluye compatibilidad con la autenticación y la autorización, así que puede iniciar la sesión de los usuarios y acceder a los datos escribiendo una cantidad mínima de código o directamente sin código en la aplicación web, la API RESTful, el back-end móvil y Azure Functions.

#### ¿Por qué usar la autenticación integrada?

No es necesario usar App Service para la autenticación y autorización. Muchos marcos web están incluidos en las características de seguridad y puede usarlos si lo desea. Si necesita más flexibilidad de la que App Service proporciona, también puede escribir sus propias utilidades.

La característica de autenticación integrada para App Service y Azure Functions puede ahorrar tiempo y esfuerzo, ya que proporciona autenticación integrada con proveedores de identidades federados, lo que le permite centrarse en el resto de la aplicación.

- Azure App Service permite integrar diversas funcionalidades de autenticación en la aplicación web o la API sin implementarlas usted mismo.
- Está integrada directamente en la plataforma y no requiere ningún lenguaje, SDK, conocimientos de seguridad o código en particular.
- Puede integrar con varios proveedores de inicio de sesión. Por ejemplo, Azure AD, Facebook, Google y Twitter.

#### Proveedores de identidades

App Service usa la identidad federada, en la cual un proveedor de identidades de terceros almacena las identidades de usuario y el flujo de autenticación para usted. De forma predeterminada, están disponibles los siguientes proveedores de identidades:

<b>Proveedor --- Punto de conexión de inicio de sesión	--- Guía de procedimientos</b>

Plataforma de identidad de Microsoft --- /.auth/login/aad --- Inicio de sesión con la Plataforma de identidad de Microsoft para App Service  
Facebook --- /.auth/login/facebook --- Inicio de sesión con Facebook para App Service  
Google --- /.auth/login/google --- Inicio de sesión con Google para App Service  
Twitter --- /.auth/login/twitter --- Inicio de sesión con Twitter para App Service  
Nuevo proveedor de OpenID Connect --- /.auth/login/<providerName> --- Inicio de sesión con OpenID Connect para App Service  
GitHub --- /.auth/login/github --- Inicio de sesión de GitHub de App Service

Cuando habilita la autenticación y autorización con uno de estos proveedores, su punto de conexión de inicio de sesión está disponible para la autenticación de usuarios y para la validación de tokens de autenticación del proveedor. Se puede proporcionar a los usuarios cualquier número de estas opciones de inicio de sesión.

#### Funcionamiento

El módulo de autenticación y autorización se ejecuta en el mismo espacio aislado que el código de aplicación. Cuando está habilitado, cada solicitud HTTP entrante pasa a través de él antes de que el código de aplicación lo controle. Este módulo controla varios aspectos de la aplicación:

- Autentica usuarios y clientes con los proveedores de identidades especificados.
- Valida, almacena y actualiza los tokens de OAuth emitidos por los proveedores de identidades configurados.
- Administra la sesión autenticada
- Inserta información de identidad en encabezados de solicitud HTTP.
  
El módulo se ejecuta por separado del código de la aplicación y se puede configurar mediante Azure Resource Manager o mediante un archivo de configuración. No se necesitan SDK, lenguajes de programación específicos ni cambios en el código de la aplicación.

Nota: En Linux y los contenedores, el módulo de autenticación y autorización se ejecuta en un contenedor independiente, aislado del código de la aplicación. Puesto que no se ejecuta en proceso, no es posible la integración directa con plataformas de lenguaje específicas.

##### Flujo de autenticación
El flujo de autenticación es el mismo para todos los proveedores, pero varía en función de si desea iniciar sesión con el SDK del proveedor.

- Sin el SDK del proveedor: la aplicación delega el inicio de sesión federado a App Service. Por lo general, suele ser el caso de las aplicaciones de explorador, que pueden presentar la página de inicio de sesión del proveedor al usuario. El código de servidor administra el proceso de inicio de sesión, por lo que también se conoce como flujo dirigido por el servidor o flujo de servidor.

- Con el SDK del proveedor: la aplicación inicia manualmente la sesión del usuario con el proveedor y luego envía el token de autenticación a App Service para su validación. Por lo general, suele ser el caso de las aplicaciones sin explorador, que no pueden presentar la página de inicio de sesión del proveedor al usuario. El código de aplicación administra el proceso de inicio de sesión, por lo que también se conoce como flujo dirigido por el cliente o flujo de cliente. Esto se aplica a las API de REST, Azure Functions, los clientes del explorador JavaScript y las aplicaciones móviles nativas que inician la sesión de los usuarios mediante el SDK del proveedor.

En la tabla siguiente se muestran los pasos del flujo de autenticación.

<b>Paso --- Sin el SDK del proveedor --- Con el SDK del proveedor</b>

Inicio de sesión del usuario --- Redirige el cliente a /.auth/login/<provider>. --- El código de cliente proporciona inicio de sesión al usuario directamente con el SDK del proveedor y recibe un token de autenticación. Para información, consulte la documentación del proveedor.  
Autenticación posterior --- El proveedor redirige el cliente a /.auth/login/<provider>/callback. --- El código de cliente publica el token del proveedor en /.auth/login/<provider> para la validación.  
Establecer la sesión autenticada --- App Service agrega una cookie autenticada a la respuesta. --- App Service devuelve su propio token de autenticación al código de cliente.  
Servir contenido autenticado --- El cliente incluye la cookie de autenticación en las solicitudes posteriores (controladas automáticamente por explorador). --- El código de cliente presenta el token de autenticación en el encabezado X-ZUMO-AUTH (controlado automáticamente por SDK de cliente de Mobile Apps).

Para los exploradores del cliente, App Service puede dirigir automáticamente todos los usuarios no autenticados a /.auth/login/<provider>. También se pueden presentar a los usuarios uno o varios vínculos /.auth/login/<provider> para iniciar sesión en la aplicación con sus proveedores preferidos.

##### Comportamiento de la autorización
En Azure Portal, puede configurar App Service con varios comportamientos cuando una solicitud entrante no esté autenticada.

- Permitir solicitudes no autenticadas: Esta opción aplaza la autorización del tráfico no autenticado al código de la aplicación. Para las solicitudes autenticadas, App Service también transfiere información de autenticación en los encabezados HTTP. Esta opción proporciona más flexibilidad a la hora de controlar las solicitudes anónimas. Le permite presentar varios proveedores de inicio de sesión a los usuarios.

- Requerir autenticación: esta opción rechaza todo tráfico no autenticado que se dirige a la aplicación. Este rechazo puede ser una acción de redireccionamiento a uno de los proveedores de identidades configurados. En estos casos, un cliente del explorador se redirige a /.auth/login/<provider> para el proveedor que elija. Si la solicitud anónima procede de una aplicación móvil nativa, la respuesta devuelta es HTTP 401 Unauthorized. También puede configurar el rechazo para que sea HTTP 401 Unauthorized o HTTP 403 Forbidden para todas las solicitudes.

Precaución: Este método de restricción del acceso se aplica a todas las llamadas a la aplicación, lo que puede no ser deseable para las aplicaciones que necesitan una página de inicio disponible públicamente, como muchas aplicaciones de una sola página.

##### Almacén de tokens
App Service proporciona un almacén de tokens integrado, que es un repositorio de tokens que están asociados a los usuarios de las aplicaciones web, API o aplicaciones móviles nativas. Al habilitar la autenticación con cualquier proveedor, este almacén de tokens pasa a estar inmediatamente disponible para la aplicación.

##### Registro y seguimiento
Si habilita el registro de aplicaciones, los seguimientos de autenticación y autorización se recopilan directamente en los archivos de registro. Si ve un error de autenticación que no esperaba, puede encontrar cómodamente todos los detalles examinando los registros de aplicaciones existentes.

### Detección de características de redes de App Service

De manera predeterminada, puede acceder a las aplicaciones hospedadas en App Service directamente a través de Internet, y éstas sólo pueden acceder a los puntos de conexión hospedados en Internet. No obstante, en el caso de muchas aplicaciones, debe controlar el tráfico de red entrante y saliente.

Hay dos tipos de implementación principales para Azure App Service. El servicio público multiinquilino hospeda planes de App Service en las SKU de precios Gratis, Compartido, Básico, Estándar, Premium, PremiumV2 y PremiumV3. También se encuentra disponible App Service Environment (ASE) de un único inquilino, que hospeda planes de App Service de SKU aislada directamente en su red virtual de Azure.

#### Características de redes de App Service multiinquilino

Azure App Service es un sistema distribuido. Los roles que controlan las solicitudes HTTP o HTTPS entrantes se denominan servidores front-end. Los roles que hospedan la carga de trabajo del cliente se denominan roles de trabajo. Todos los roles de una implementación de App Service existen en una red de varios inquilinos. Puesto que hay muchos clientes diferentes en la misma unidad de escalado de App Service, no puede conectar la red de App Service directamente a su red.

En lugar de conectarse a redes, necesita características para administrar los diversos aspectos de la comunicación de aplicaciones. Las características que controlan las solicitudes a la aplicación no se pueden usar para solucionar problemas al realizar llamadas desde la aplicación. Del mismo modo, las características que resuelven problemas para las llamadas desde la aplicación no se pueden usar para solucionar problemas de llamadas a la aplicación.

**Características de entrada** ------------------ **Características de salida**

Dirección asignada a las aplicaciones  ------------------  conexiones híbridas  
Restricciones de acceso	 ------------------  Integración de red virtual con requisito de puerta de enlace  
Puntos de conexión del servicio	 ------------------  Integración de la red virtual  
Puntos de conexión privados	

Puede combinar las características para solucionar los problemas con algunas excepciones. Los siguientes casos de uso de entrada son ejemplos de cómo usar características de redes de App Service para controlar el tráfico de entrada a la aplicación.

**Caso de uso de entrada** ------------------ **Característica**  

Compatibilidad con las necesidades de SSL basado en IP de la aplicación	------------------ Dirección asignada a las aplicaciones  
Compatibilidad con la dirección entrante dedicada no compartida para la aplicación	------------------ Dirección asignada a las aplicaciones  
Restricción del acceso a la aplicación desde un conjunto de direcciones bien definidas ------------------ Restricciones de acceso  

#### Comportamiento predeterminado de la redes

Las unidades de escalado de Azure App Service admiten muchos clientes en cada implementación. Los planes de SKU Gratis y Compartido hospedan cargas de trabajo de clientes en roles de trabajo multiinquilino. El plan Básico y los planes superiores hospedan cargas de trabajo dedicadas a un único plan de App Service. Si tiene un plan de App Service Estándar, todas las aplicaciones de ese plan se ejecutan en el mismo rol de trabajo. Si escala horizontalmente el rol de trabajo, todas las aplicaciones de ese plan de App Service se replican en un rol de trabajo nuevo para cada instancia del plan de App Service.

##### Direcciones de salida
Las máquinas virtuales de trabajo se desglosan en gran medida a través de los planes de App Service. Los planes Gratis, Compartido, Básico, Estándar y Premium usan el mismo tipo de máquina virtual de trabajo. El plan PremiumV2 usa otro tipo de máquina virtual. PremiumV3 también usa otro tipo de máquina virtual. Cuando se cambia la familia de máquinas virtuales, obtiene un conjunto diferente de direcciones de salida.

Hay muchas direcciones que se usan para las llamadas salientes. Las direcciones de salida que usa la aplicación para realizar llamadas salientes se muestran en las propiedades de la aplicación. Todas las aplicaciones que se ejecutan en la misma familia de máquinas virtuales de trabajo de la implementación de App Service comparten estas direcciones. Si quiere ver todas las direcciones que puede usar la aplicación en una unidad de escalado, existe una propiedad denominada possibleOutboundIpAddresses que las enumera.

##### Búsqueda de las direcciones IP de salida
Para buscar las direcciones IP de salida que usa actualmente su aplicación en Azure Portal, seleccione Propiedades en el panel de navegación izquierdo de la aplicación.

Puede encontrar la misma información si ejecuta el comando siguiente de la CLI de Azure en Cloud Shell. Se enumeran en el campo Direcciones IP salientes adicionales.

az webapp show \
    --resource-group <group_name> \
    --name <app_name> \ 
    --query outboundIpAddresses \
    --output tsv

Para buscar todas las posibles direcciones IP de salida para la aplicación, con independencia de los planes de tarifa, ejecute el siguiente comando en Cloud Shell.

az webapp show \
    --resource-group <group_name> \ 
    --name <app_name> \ 
    --query possibleOutboundIpAddresses \
    --output tsv

### Ejercicio: Creación de una aplicación web HTML estática mediante Azure Cloud Shell

En este ejercicio, implementará un sitio de HTML y CSS básico en Azure App Service mediante el comando az webapp up de la CLI de Azure. Después, actualizará el código y lo volverá a implementar con el mismo comando.

El comando az webapp up facilita la creación y actualización de aplicaciones web. Cuando se ejecuta, realiza las siguientes acciones:

- Crea un grupo de recursos predeterminado si no se especifica uno.
- Crear un plan de App Service predeterminado.
- Crear una aplicación con el nombre especificado.
- Implementar con ZIP archivos desde el directorio de trabajo actual a la aplicación web.

#### Descarga de la aplicación de ejemplo

En esta sección, usará el espacio aislado para descargar la aplicación de ejemplo y establecer variables para que algunos de los comandos sean más fáciles de escribir.

En el espacio aislado, cree un directorio y, después, navegue hasta él.

mkdir htmlapp  
cd htmlapp

Ejecute el siguiente comando git para clonar el repositorio de aplicaciones de ejemplo en el directorio htmlapp.

git clone https://github.com/Azure-Samples/html-docs-hello-world.git

Establezca variables para contener el grupo de recursos y los nombres de la aplicación mediante la ejecución de los comandos siguientes.

resourceGroup=$(az group list --query "[].{id:name}" -o tsv)  
appName=az204app$RANDOM

#### Creación de la aplicación web

Cambie al directorio que contiene el código de ejemplo y ejecute el comando az webapp up.

cd html-docs-hello-world  
az webapp up -g $resourceGroup -n $appName --html

Este comando puede tardar varios minutos en ejecutarse. Durante la ejecución, muestra información similar a la del ejemplo siguiente.

JSON

{  
"app_url": "https://<myAppName>.azurewebsites.net",  
"location": "westeurope",  
"name": "<app_name>",  
"os": "Windows",  
"resourcegroup": "<resource_group_name>",  
"serverfarm": "appsvc_asp_Windows_westeurope",  
"sku": "FREE",  
"src_path": "/home/<username>/demoHTML/html-docs-hello-world ",  
< JSON data removed for brevity. >  
}

Abra una pestaña nueva en el explorador, vaya a la dirección URL de la aplicación (https://<myAppName>.azurewebsites.net) y compruebe que la aplicación está en ejecución; anote el título de la parte superior de la página. Deje el explorador abierto en la aplicación para la sección siguiente.

Nota: Puede copiar <myAppName>.azurewebsites.net desde la salida del comando anterior, o bien seleccionar la dirección URL de la salida para abrir el sitio en una pestaña nueva.

#### Actualización de la aplicación y nueva implementación

En Cloud Shell, escriba code index.html para abrir el editor. En la etiqueta de encabezado <h1>, cambie Azure App Service - Sample Static HTML Site a Azure App Service Updated - o a cualquier otra cosa que desee. Use los comandos ctrl-s para guardar y ctrl-q para salir. Vuelva a implementar la aplicación con el mismo comando az webapp up que ha usado antes.

az webapp up -g $resourceGroup -n $appName --html 
 
Sugerencia: Puede usar la flecha arriba del teclado para desplazarse por los comandos anteriores.

Una vez completada la implementación, vuelva al explorador del paso 2 de la sección "Creación de la aplicación web" anterior y actualice la página.