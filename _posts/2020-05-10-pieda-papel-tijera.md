---
title: Pidera Papel Tijera
layout: post
post-image: "https://external-content.duckduckgo.com/iu/?u=http%3A%2F%2Fis1.mzstatic.com%2Fimage%2Fpf%2Fus%2Fr30%2FPurple1%2Fv4%2F4e%2F75%2F17%2F4e75172a-aba2-9e47-6649-9674b857d320%2Fpr_source.png&f=1&nofb=1"
description: El mitico juego de Piedra Papel o Tijera recreado en python
tags:
- Juegos
- Python
- Programa
---

El mitico juego de Piedra Papel o Tijera recreado en python.

---

# Pidera Papel Tijera <br>

### Para usar el codigo se necesitaran importar las sigentes librerias <br>

`random`
<br><br>

para installarla escribir el sigente comando en la terminal:

`pip install random`

### El codigo es el siguiente <br>

> import random <br>
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
>
> aleatorio = random.randrange(0, 3) <br>
> elijePc = "" <br>
> print("1)Piedra") <br>
> print("2)Papel") <br>
> print("3)Tijera") <br>
> opcion = int(input("Que elijes: ")) <br>
> <br>
> if opcion == 1: <br>
>     elijeUsuario = "piedra" <br>
> elif opcion == 2: <br>
>     elijeUsuario = "papel" <br>
> elif opcion == 3: <br>
>     elijeUsuario = "tijera" <br>
> print("Tu elijes: ", elijeUsuario) <br>
> <br>
> if aleatorio == 0: <br>
>     elijePc = "piedra" <br>
> elif aleatorio == 1: <br>
>     elijePc = "papel" <br>
> elif aleatorio == 2: <br>
>     elijePc = "tijera" <br>
> print("PC elijio: ", elijePc) <br>
> print("...") <br>
> if elijePc == "piedra" and elijeUsuario == "papel": <br>
>     print("Ganaste, papel envulve piedra") <br>
> elif elijePc == "papel" and elijeUsuario == "tijera": <br>
>     print("Ganaste, Tijera corta papel") <br>
> elif elijePc == "tijera" and elijeUsuario == "piedra": <br>
>     print("Ganaste, Piedra pisa tijera") <br>
> if elijePc == "papel" and elijeUsuario == "piedra": <br>
>     print("perdiste, papel envulve piedra") <br>
> elif elijePc == "tijera" and elijeUsuario == "papel": <br>
>     print("perdiste, Tijera corta papel") <br>
> elif elijePc == "piedra" and elijeUsuario == "tijera": <br>
>     print("perdiste, Piedra pisa tijera") <br>
> elif elijePc == elijeUsuario: <br>
>    print("empate") <br>
> <br>

<br>

**Una ves copidado el codigo**<br>

Copiar y Pegar el codido en un archivo **.txt** y cambiar la estencion a **.py** y ejecutarlo con python3 si no lo tiene descargado puede ir al sigente link: [Descargar Python](https://www.python.org/downloads/)
<br><br>

**Para ejecutarlo:**
1. Abir la cmd o la Terminal
2. Escrivir: **python3 "ruta del archivo"**
3. Precionamos Enter y a Jugar 



