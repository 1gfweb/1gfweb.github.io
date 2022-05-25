---
title: Organizador de archivos
layout: post
post-image: "https://acf.geeknetic.es/imagenes/tutoriales/91-archivos-extensiones-programas-muestra.jpg"
description: Un simple programa escrito en Python para organizar archivos
tags:
- Utilidades
- Python
- Herramienta
- Programa

---

Imagine que tiene una carpeta con cientos de archivos diferentes. Por lo tanto, crea un desastre y ahora desea organizarlos en carpetas. para almacenar archivos con la misma extensión, solo necesita este programa  escrito en Python.

---

# Organizador de archivos <br>

### Para usar el codigo se necesitaran importar las sigentes librerias <br>

`os`

`shutil`
<br><br>

para installarla escribir el sigente comando en la terminal:

`pip install os`

`pip install pytest-shutil`

### El codigo es el siguiente <br>

>import os <br>
>import shutil
><br>
><br>print()
><br>print()
><br>print('░██████╗░░░░██████╗░██╗████████╗░██████╗')
><br>print('██╔════╝░░░░██╔══██╗██║╚══██╔══╝██╔════╝')
><br>print('██║░░██╗░░░░██████╦╝██║░░░██║░░░╚█████╗░')
><br>print('██║░░╚██╗░░░██╔══██╗██║░░░██║░░░░╚═══██╗')
><br>print('╚██████╔╝██╗██████╦╝██║░░░██║░░░██████╔╝')
><br>print('░╚═════╝░╚═╝╚═════╝░╚═╝░░░╚═╝░░░╚═════╝░')
><br>print()
><br>print()
><br>
><br>
>dirName = input('Introducir el Nombre de la Carpeta: ')<br>
>li = os.listdir(dirName)<br>
>for i in li:<br>
>    fileName, extencion = os.path.splitext(i)
><br>    
>    extencion = extencion[1:]<br>
>    if extencion == "":<br>
>        continue
><br>
>    if os.path.exists( dirName + '/' + extencion ):<br>
>        shutil.move( dirName + '/' + i, dirName + '/' + extencion + '/' + i )
><br>        
>    else:
>        os.makedirs( dirName + '/' + extencion )<br>
>        shutil.move( dirName + '/' + i, dirName + '/' + extencion + '/' + i )<br>
><br>

**Una ves copidado el codigo**<br>

Copiar y Pegar el codido en un archivo **.txt** y cambiar la estencion a **.py** y ejecutarlo con python3 si no lo tiene descargado puede ir al sigente link: [Descargar Python](https://www.python.org/downloads/)
<br><br>

**Para ejecutarlo:**
1. Abir la cmd o la Terminal
2. Escrivir: **python3 "ruta del archivo"**
3. Precionamos Enter
4. Introducir el nombre de la carpeta



