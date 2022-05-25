---
title: Generador de Contraseñas
layout: post
post-image: "https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fwww.riial.org%2Fwp-content%2Fuploads%2F2020%2F07%2Fcuidados-contrase%25C3%25B1as-scaled.jpg&f=1&nofb=1"
description: Un simple programa escrito en Python para generar contraseñas seguras
tags:
- Utilidades
- Python
- Herramienta
- Programa
---

Esta herramienta escrita en Python es capas de generar contraseñas seguras y a su ves usa un  algoritmo de criptografía el cual es MD5 (En criptografía, MD5 es un algoritmo de reducción criptográfico de 128 bits ampliamente usado).

---

# Generador de Contraseñas <br>

### Para usar el codigo se necesitaran importar las sigentes librerias <br>

`random`<br>

`werkzeug`
<br><br>

para installarla escribir el sigente comando en la terminal:

`pip install random`

`pip install Werkzeug`

### El codigo es el siguiente <br>

> import random <br>
> from werkzeug.security import generate_password_hash <br>
>
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
> rango = int(input("Nuemro de Contraseñas Max(100): ")) <br>
> print() <br>
> longitud = int(input("Longitud de Contraseñas Max(86): ")) <br>
> print() <br>
><br>
> minus = "abcdefghijklmnopqrstuvwxyz" <br>
> mayus = minus.upper() <br>
> numeros = "0123456789" <br>
> simbolos = "@()[]{}+*.:,;/-_'¡!€%$&=" <br>
><br>
> base = minus + mayus + numeros + simbolos <br>
><br>
> for _ in range(rango): <br>
>     muestra = random.sample(base, longitud) <br>
>     password = "".join(muestra) <br>
>    password_Encrip = generate_password_hash(password) <br>
>     print("{} => {}".format(password, password_Encrip)) <br>
> <br>

<br>

**Una ves copidado el codigo**<br>

Copiar y Pegar el codido en un archivo **.txt** y cambiar la estencion a **.py** y ejecutarlo con python3 si no lo tiene descargado puede ir al sigente link: [Descargar Python](https://www.python.org/downloads/)
<br><br>

**Para ejecutarlo:**
1. Abir la cmd o la Terminal
2. Escrivir: **python3 "ruta del archivo"**
3. Precionamos Enter 
4. Introducimos el numero de Contraseñas a Generar y la longitud de las mismas


