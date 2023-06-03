<b><ins>Área de dominio AZ-900</ins> &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; &nbsp; <ins>Peso</ins></b>

Descripción de los conceptos de la nube &emsp; &emsp; &emsp; &emsp; &emsp; &emsp; 25-30 % <br>
Descripción de la arquitectura y los servicios de Azure &emsp; &nbsp; 35-40 % <br>
Descripción de la administración y la gobernanza &emsp; &emsp; &emsp; 30-35 %

<h1 align="center"><ins>RUTA 1: DESCRIPCIÓN DE LOS CONCEPTOS DE LA NUBE</ins></h1>
<h2 align="center">MÓDULO 1 - DESCRIPCIÓN DE LA INFORMÁTICA EN LA NUBE</h2>  
  
¿Qué es la informática en la nube? Es la prestación de servicios informáticos a través de Internet.<br>
Cada proveedor de nube tiene sus propios servicios, pero los servicios básicos que todos ellos proporcionan son la <ins><b>potencia de proceso</b></ins> y el <ins><b>almacenamiento</b></ins>.

<ins><b>MODELO DE RESPONSABILIDAD COMPARTIDA:</b></ins> Las responsabilidades se comparten entre el proveedor de servicios en la nube y el consumidor. La seguridad física, la alimentación, la refrigeración y la conectividad de red son responsabilidad del proveedor de servicios en la nube. El consumidor es el responsable de los datos y la información almacenados en la nube, así como de la seguridad de acceso, dando acceso solo a aquellos que lo necesitan.

El modelo de responsabilidad compartida está muy vinculado a los tipos de servicio en la nube: infraestructura como servicio (IaaS), plataforma como servicio (PaaS) y software como servicio (SaaS).  
IaaS sitúa la mayor responsabilidad en el consumidor y el proveedor de servicios en la nube es el responsable de los conceptos básicos de seguridad física, energía y conectividad. En el extremo opuesto, SaaS sitúa la mayor parte de la responsabilidad en el proveedor de servicios en la nube.
<br><br>
![texto](./../../images/Azure-Shared-Responsibility-Model.png)

Siempre será responsabilidad suya lo siguiente:

1. La información y los datos almacenados en la nube.
2. Los dispositivos que pueden conectarse a la nube (teléfonos móviles, equipos, etc.).
3. Las cuentas e identidades de las personas, servicios y dispositivos de la organización

El proveedor de nube siempre es el responsable de lo siguiente:

1. El centro de datos físico
2. La red física
3. Los hosts físicos

El modelo de servicio determinará la responsabilidad de cosas como lo siguiente:

1. Sistemas operativos
2. Controles de red
3. Aplicaciones
4. Identidad e infraestructura

<ins><b>MODELOS EN LA NUBE:</b></ins> Definen el tipo de implementación de recursos en la nube. Los tres principales modelos en la nube son: privados, públicos e híbridos.  
  
<b>Nube privada:</b> Evolución natural de un centro de datos corporativo. Brinda servicios de TI a través de Internet y es utilizada por una sola entidad. Proporciona un control mucho mayor para la empresa y su departamento de TI, aunque también incluye un mayor costo.

<b>Nube pública:</b> Un proveedor de nube de terceros crea, controla y mantiene una nube pública. Con una nube pública, cualquier persona que quiera comprar servicios en la nube puede acceder a los recursos y usarlos. La disponibilidad pública general es una diferencia clave entre las nubes públicas y privadas.

<b>Nube híbrida:</b> Entorno informático que usa nubes públicas y privadas en un entorno interconectado. Se puede usar un entorno de nube híbrida para permitir el incremento de una nube privada y acomodarse al aumento de la demanda temporal mediante la implementación de recursos de nube pública. Asi, también se puede usar la nube híbrida para proporcionar una capa adicional de seguridad. Por ejemplo, los usuarios pueden elegir de forma flexible qué servicios mantener en la nube pública y qué implementar en su infraestructura de nube privada.

Nube pública:

1. No hay gastos de capital para escalar verticalmente.
2. Las aplicaciones pueden aprovisionarse y desaprovisionarse rápidamente.
3. Las organizaciones solo pagan por lo que usan.
4. Las organizaciones no tienen un control total de los recursos y la seguridad.

Nube privada:

1. Las organizaciones tienen un control total de los recursos y la seguridad.
2. Los datos no se colocan con los datos de otras organizaciones.
3. Debe adquirirse hardware para la puesta en funcionamiento y el mantenimiento.
4. Las organizaciones son responsables del mantenimiento y las actualizaciones del hardware.

Nube híbrida:

1. Proporciona la máxima flexibilidad.
2. Las organizaciones determinan dónde se van a ejecutar sus aplicaciones.
3. Las organizaciones controlan la seguridad, el cumplimiento o los requisitos legales.

Nubes múltiples: Escenario de varias nubes donde se usan varios proveedores de nube pública.

<ins><b>MODELO BASADO EN EL CONSUMO:</b></ins>

Dos tipos de gastos que se deben tener en cuenta: Gastos de capital y gastos operativos.

Los gastos de capital suelen ser un gasto por adelantado único para comprar o proteger recursos tangibles.
En cambio, los gastos operativos es gastar dinero en servicios o productos a lo largo del tiempo.

La informática en la nube se encuentra en la partida de gastos operativos porque funciona en un modelo basado en el consumo. Este modelo basado en el consumo aporta muchas ventajas, por ejemplo:
  
1. Sin costes por adelantado.
2. Se puede pagar para obtener más recursos cuando se necesiten.
3. Se puede dejar de pagar por los recursos que ya no se necesiten.
  
Comparación de los modelos de precios en la nube: La informática en la nube es la prestación de servicios informáticos a través de Internet mediante un modelo de precios de pago por uso. Normalmente solo se paga por los servicios en la nube que se usan, lo que permite:

1. Planificar y administrar los costos operativos.
2. Ejecutar la infraestructura de forma más eficaz.
3. Escalar a medida que cambien las necesidades empresariales.