---
title: Comparador de Archivos
layout: post
post-image: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.adslzone.net%2Fapp%2Fuploads-adslzone.net%2F2019%2F06%2Fgoogle-docs-comparar-documentos.jpg&f=1&nofb=1"
description: Un simple programa escrito en Python para comparar archivos
tags:
- Utilidades
- Python
- Herramienta
- Programa

---

Este es un programa el cual sirve para comparar 2 archivos del mismo tipo ya que Cuando llevas mucho tiempo trabajando en un documento, es normal archivar diferentes versiones. Y a veces no recuerdas cual es la más nueva.

---

# Comparador de Archivos

### El codigo es el siguiente <br>

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
>print()
><br>
>archivo1 = input("Ruta del Archivo 1: ")
>archivo2 = input("Ruta del Archivo 1: ")
>print()
><br>
><br>f1 = open(archivo1, "r")   
>f2 = open(archivo2, "r")   
><br>  
>i = 0
>C = 0
>NC = 0  
><br>
>for line1 in f1: 
>    i += 1
><br>      
>    for line2 in f2: 
><br>          
>        if line1 == line2:
>            C = C + 1
><br>
>            print("Linea ", i, ": CONSIDENCIA")
><br>
>            print("\tArchivo 1:", line1, end='') 
>            print("\tArchivo 2:", line2, end='')      
>            print()
><br>
>        else:
>            NC = NC + 1
><br>
>            print("Linea", i, ": NO CONSIDE") 
><br>
>            print("\tArchivo 1:", line1, end='') 
>            print("\tArchivo 2:", line2, end='')
>            print()
><br>
>        break
><br>
>f1.close()                                        
>f2.close()  
><br>
>print("CONSIDENCIAS: ", C,)        
>print("NO CONCIDENCIAS: ", NC,)
><br>

**Una ves copidado el codigo**<br>

Copiar y Pegar el codido en un archivo **.txt** y cambiar la estencion a **.py** y ejecutarlo con python3 si no lo tiene descargado puede ir al sigente link: [Descargar Python](https://www.python.org/downloads/)
<br><br>

**Para ejecutarlo:**
1. Abir la cmd o la Terminal
2. Escrivir: **python3 "ruta del archivo"**
3. Precionamos Enter
4. Introducir la ruta de los archivos que se desea comparar



