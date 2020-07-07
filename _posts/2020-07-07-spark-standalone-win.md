---
title: "Spark Standalone Windows"
categories:
  - Utilidades
tags:
  - Utilidades
  - spark
---

Para windows es necesario `winutils.exe` - [winutils](https://github.com/steveloughran/winutils)

1. Descargar en C: el directorio `hadoop` que nos interese de la [URL anterior](https://github.com/steveloughran/winutils). Por ejemplo: `C:\hadoop-3.0.0`
2. Crear una nueva variable de entorno `HADOOP_HOME` apuntando a `C:\hadoop-3.0.0` (User Variables en System Properties -> Advance System Settings) o especificar ese hadoop home directamente en código: `System.setProperty("hadoop.home.dir","C:\\hadoop-3.0.0")`

Opcional: miniDFS cluster
- [Usar miniDFS](https://akashrehan.wordpress.com/2018/03/25/how-to-use-minidfs-cluster-in-hdfs-dependent-test-cases/)