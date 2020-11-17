# Introducción a Builds con Openshift

El ejercicio anterior se basaba en la idea de tener una imagen pre-armada. Openshift permite, además, construir una imagen desde un repositorio usando una estrategia llamanda Source-to-image (S2I).

> Source-to-image (S2I) is a tool for building reproducible container images. S2I
> produces ready-to-run images by injecting source code into a container image and
> assembling a new container image which incorporates the builder image and built
> source. The result is then ready to use with docker run. S2I supports
> incremental builds which re-use previously downloaded dependencies, previously
> built artifacts, etc.



Openshift ejecuta el proceso de s2i dentro de un POD especial, llamado Build Pod. Al ser un POD, Openshift aplica las mismas politicas, controles, etc, que cualquier POD.
  
Se puede leer mas sobre el proyecto de S2I desde su web de [github](https://github.com/openshift/source-to-image) o en este video de [Openshift](https://youtu.be/flI6zx9wH6M)
  
