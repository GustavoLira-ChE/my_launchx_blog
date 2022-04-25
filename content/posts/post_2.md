---
title: "Como crear un proyecto de JavaScript desde 0"
date: 2022-04-25
description: 'Usando Node y Git entenderemos como configurar el inico de un proyecto'
---

# Antes de empezar
Es necesario contar con NODE.js, NPM y Git para poder hacer realizar este mini tutorial

# Elegir el lugar del repositorio
Lo primero que hay que hacer es elegir donde queremos guardar nuestro proyecto de JavaScript, en este caso es importante al menos en Windows si se esta usando WSL guardar le proyecto en el "root" de ubuntu en windows, ya que esto ayuda a tener un mejor manejo del proyecto así como tener la funcionalidad de live server para proyecto de React y Vue.

# Crear la carpeta
Una vez elegido el lugar del proyecto, vamos a crear la carpeta del proyecto, aquí vivirán todos los archivos que tendrá el proyecto, esto se logra desde la terminal con el comando:
```
mkdir nombre_carpeta
```

# Ir a la carpeta del directorio
Vamos a movernos a la carpeta del proyecto y aquí desde la linea de comando vamos a ejecutar:
```
git init
```
Esto activará Git en nustro repo para poder llevar el control de versiones.
Posteriormente vamos nuevamente en la linea de comando a ejecutar el comando siguiente:
```
npm init
```
Esto creará un archivo llamado *package.json* este archivo contiene información del proyecto, como lo son el nombre, versión, privacidad, autor, licencia, dependencias, etc.

# Crear un .gitignore
Este archivo es importante crearlo para que git ignore cierto tipo de archivos o carpetas que no queremos que sean versionadas en el proyecto, el comando para generar este archivo es:
```
touch .gitignore
```
Este comando se ejecuta en el bash asegurandote que te encuentrás en la carpeta principal de tu proyecto o en la raiz del proyecto.
Aquí referenciamos todos los archivos que no son necesarios en el repo para ser versionados como archivos de video, sonido, archivos de imagen pesados o la carpeta node_modules.

# Para finalizar
Es importante tener un archivo *index* donde el proyecto tendrá salida, además de configurar los distintos directorios necesarios en el proyecto como lo son test/ y app/ que tendrás las archivos de las pruebas unitarias y los archivos propios de la aplicación.