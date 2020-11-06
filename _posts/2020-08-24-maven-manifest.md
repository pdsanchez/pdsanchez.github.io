---
title: "Custom properties en el MANIFEST.MF desde maven"
categories:
  - Utilidades
tags:
  - Utilidades
  - maven
---

Añadir información sobre versión y cambion en el fichero MANIFEST.MF al compilar el jar.

```XML
<plugin>
    <groupId>org.apache.maven.plugins</groupId>
    <artifactId>maven-jar-plugin</artifactId>
    <configuration>
        <archive>
            <manifestEntries>
                <version>${version}</version>
                <inf-20200820>#273 - Corregir excepción [vs. ${version}]</inf-20200820>
            </manifestEntries>
        </archive>
    </configuration>
</plugin>
```

El fichero MANIFEST.MF queda:

```txt
Manifest-Version: 1.0
inf-20200820: #273 - Corregir excepción F1 Failed [vs. 1.0.3]
Archiver-Version: Plexus Archiver
Built-By: pablo.sanchez
version: 1.0.3
Created-By: Apache Maven 3.3.9
Build-Jdk: 1.8.0_92
```
