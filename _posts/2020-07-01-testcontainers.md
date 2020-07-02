---
title: "Testcontainers"
categories:
  - Utilidades
tags:
  - Utilidades
---

[Testcontainers](https://www.testcontainers.org/) es una librería de java que provee instancias de cualquier cosa que se pueda ejecutar en un contenedor Docker (bases de datos, navegadores, servicios etc.)

Cualquier aplicación dockerizada se podrá instanciar con testcontainer.

Esto es muy útil para desarrollar pruebas de integración y comprobar, por ejemplo, que nuestra aplicación comunica correctamente con la base de datos, como con el servicio. Testcontainer levantará un contenedor Docker de MySQL y otro de servicio.