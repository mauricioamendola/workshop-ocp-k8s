# Workshop de Openshift / Kubernetes


### Contenido

1. Sumario del curso [TODO]
2. [Arquitectura de OCP](docs/arquitectura.md)
     * [Diferencias con Kubernetes](docs/openshift-vs-k8s.md)
3. Explorando Openshift
	 * [La consola Web](docs/web-ui.md)
	 * [La terminal de comandos](docs/cli-client.md)
4. Proyectos / Namespaces
	 * [Ejercicio: Creando un proyecto](docs/create-project.md)
	 * [Explorar el proyecto creado](docs/explore-project.md)
6. PODINFO App
	* [Revision POD y Containers](docs/application.md)
	* Ejercicio
		* [Deployar una imagen existente](docs/deploy-app.md)
		* [Examinando el POD](docs/exploring-pod.md)
	* [Exponiendo el servicio](docs/public-app.md)  
	* [Publicando una Ruta](docs/public-route.md)
7. Construyendo desde código
	* [Intro a Source-to-Image](docs/build.md)
	* [Ejercicio: Deployar desde el Código](docs/run-build-app.md)
	* [Ejercicio: Realizar un cambio en la aplicación](docs/change-build-app.md)
8. Health Checks
	* [Intro a los Health Checks](docs/health-checks.md)
	* [Ejercicio: Configurar chequeos](docs/set-health-checks.md)
9. Troubleshooting Openshift
	* [Eventos](docs/ts-events.md)
	* [Logs](docs/ts-logs.md)
10. Herramientas [TODO]
11. Usando YAMLs [TODO]
    * Estructura de los Objetos
        * POD
        * Deployment
        * Service
    * Ejercicio
        * Deployando PODInfo usando YAMLs
