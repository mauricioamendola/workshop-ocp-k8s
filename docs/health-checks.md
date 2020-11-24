# Health Checks

Los health checks sirven para establecer bajo que condiciones la aplicación se encuentra saludable y si está lista para recibir tráfico.  Existen tres chequeos que se pueden configurar en Openshift:  
* livenessProbe
* readinessProbe
* startupProbe  


## LivenessProbe

Es un chequeo que sirve para determinar si el container que tiene configurado dicho check esta **"vivo"**, en caso de no estarlo, Openshift toma la determinación de terminar el POD y crear uno nuevo.  

## ReadinessProbe

Es un chequeo que sirve para determinar si el POD está listo para recibir tráfico. Si el chequeo falla, el POD aún asi puede estar en estado **Running** pero no es tenido en cuenta como endpoint del servicio. 

## Startup Probe

Este chequeo es similar al ReadinessProbe pero se usa en ocasiones donde es necesario validar si la aplicación dentro del container **"levantó"** correctamente. Este chequeo se ejecuta una sola vez, al momento de ser instanciado el container.  

### Tipos de chequeos

* exec command
* httpGet
* tcpSocket

### Exec Command

Ejecuta el comando especificado al momento de ser instanciado el container.  

### Http Get

Ejecuta un request hacia una dirección. Tipicamente es un Get a un endpoint de la app que sirve para dar el estado de la app.  

### Tcp Socket

Abre una conexión TCP contra un host / IP y puerto.  

