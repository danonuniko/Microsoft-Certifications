<h1 align="center"><ins>RUTA 1: DESCRIPCIÓN DE LOS CONCEPTOS DE LA NUBE</ins></h1>
<h2 align="center">MÓDULO 2 - DESCRIPCIÓN DE LAS VENTAJAS DE USAR SERVICIOS EN LA NUBE</h2>

### Descripción de las ventajas de la alta disponibilidad y la escalabilidad en la nube:

Al compilar o implementar una aplicación en la nube, dos de las consideraciones más importantes son el tiempo de actividad (o la <b>disponibilidad</b>) y la capacidad de controlar la demanda (o <b>escala</b>).

<b>ALTA DISPONIBILIDAD:</b> Se centra en garantizar la máxima disponibilidad, independientemente de las interrupciones o eventos que puedan producirse. Al diseñar la solución, deberá tener en cuenta las garantías de disponibilidad del servicio. Azure es un entorno de nube de alta disponibilidad con garantías de tiempo de actividad en función del servicio. Estas garantías forman parte de los contratos de nivel de servicio.

<b>SLA o Acuerdo de Nivel de Servicio.</b> Es el acuerdo formal entre un proveedor de servicios y un cliente que garantiza al cliente un nivel de servicio establecido. En Azure, los acuerdos de nivel de servicio se representan como un porcentaje relacionado con la disponibilidad del servicio o la aplicación (tiempo de actividad o "uptime"). Normalmente un SLA incluye detalles como el tiempo de inactividad donde el servicio no está disponible o el crédito al que puede tener derecho si no se cumple el acuerdo de nivel de servicio. Los más comunes son el 99%, 99.9% y 99.95%, incluyendo el 99.99% en alguno de los servicios.

<b>ESCALABILIDAD:</b> Hace referencia a la capacidad de ajustar los recursos para satisfacer la demanda. Una ventaja es que no está pagando de más por los servicios. Dado que la nube es un modelo basado en el consumo, solo paga por lo que usa. Si la demanda baja, puede reducir los recursos y, por tanto, reducir los costos. Suele tener dos variedades: <b>vertical</b> y <b>horizontal</b>. El escalado vertical se centra en aumentar o disminuir las capacidades de los recursos. El escalado horizontal agrega o resta el número de recursos.

Escalado vertical: Agregar o disminuir más CPU o RAM a la máquina virtual.  
Escalado horizontal: Agregar o disminuir el número de máquinas virtuales utilizadas.

### Descripción de las ventajas de la confiabilidad y la previsibilidad en la nube:

- Confiabilidad: Capacidad de un sistema de recuperarse de los errores y seguir funcionando.
- Predicción: Se puede centrar en el rendimiento o los costos.
- Rendimiento: Predecir los recursos necesarios para ofrecer una experiencia positiva para los clientes.
- Coste: Se centra en pronosticar el costo del gasto en la nube.

### Descripción de las ventajas de la seguridad y la gobernanza en la nube:

Tanto si va a implementar infraestructura como servicio o software como servicio, las características en la nube admiten el cumplimiento y la gobernanza. Aspectos como las plantillas de conjunto ayudan a garantizar que todos los recursos implementados cumplan los estándares corporativos y los requisitos normativos de gobierno. Además, puede actualizar todos los recursos implementados a nuevos estándares a medida que estos cambien. La auditoría basada en la nube ayuda a marcar cualquier recurso que no cumpla los estándares corporativos y proporciona estrategias de mitigación. En función del modelo operativo, las revisiones de software y las actualizaciones también se pueden aplicar automáticamente, lo que ayuda tanto a la gobernanza como a la seguridad.

Del lado de la seguridad, puede encontrar una solución en la nube que coincida con sus necesidades de seguridad. Si quiere tener un control máximo de la seguridad, la infraestructura como servicio le proporciona recursos físicos, pero le permite administrar los sistemas operativos y el software instalado, incluidas las revisiones y el mantenimiento. Si quiere que las revisiones y el mantenimiento se administren automáticamente, las implementaciones de plataforma como servicio o software como servicio pueden ser las mejores estrategias en la nube.

Y dado que la nube está pensada como entrega mediante Internet de los recursos de TI, los proveedores de nube suelen ser adecuados para controlar cosas como ataques de denegación de servicio distribuido (DDoS), lo que hace que la red sea más sólida y segura.

### Descripción de las ventajas de la capacidad de administración en la nube:

Una ventaja importante de la informática en la nube son las opciones de administración. Hay dos tipos de administración para la informática en la nube:

<b>Administración DE la nube</b>

La administración de la nube trata sobre administrar los recursos en la nube. En la nube, puede hacer lo siguiente:
1. Escalar automáticamente la implementación de recursos en función de las necesidades.
2. Implementar recursos basados en una plantilla preconfigurada, lo que elimina la necesidad de realizar la configuración manual.
3. Supervisar el estado de los recursos y reemplazar automáticamente los recursos con errores.
4. Recibir alertas automáticas basadas en métricas configuradas, de modo que esté informado del rendimiento en tiempo real.

<b>Administración EN la nube</b>

La administración en la nube trata sobre cómo puede administrar el entorno y los recursos en la nube. Puede administrarlos de las siguientes maneras:
1. Mediante un portal web.
2. Con una interfaz de línea de comandos básica.
3. Mediante las API.
4. Mediante PowerShell.