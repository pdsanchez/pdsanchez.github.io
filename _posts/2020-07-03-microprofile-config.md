---
title: "Microprofile Config"
categories:
  - Utilidades
tags:
  - Utilidades
---

[MicroProfile Config](https://github.com/eclipse/microprofile-config) ofrece una API para recuperar la información de configuración de diferentes orígenes.

Buscamos empaquetar aplicaciones inmutables en contenedores, dentro de los cuales podamos inyectar parámetros de configuración externos.

Esto es importante en los microservicios, donde se desconoce la información de conexión entre los microservicios y servicios de terceros en tiempo de desarrollo, y solo está disponible durante la ejecución.

 Se necesita un mecanismo para modificar la configuración dinamicamente en el despliegue del microservicio.

- [https://www.eclipse.org/community/eclipse_newsletter/2017/september/article3.php](https://www.eclipse.org/community/eclipse_newsletter/2017/september/article3.php)
- [https://www.ibm.com/support/knowledgecenter/es/SSEQTP_liberty/com.ibm.websphere.wlp.doc/ae/cwlp_microprofile_overview.html](https://www.ibm.com/support/knowledgecenter/es/SSEQTP_liberty/com.ibm.websphere.wlp.doc/ae/cwlp_microprofile_overview.html)