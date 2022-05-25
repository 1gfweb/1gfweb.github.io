---
title: Escaner de puertos 
layout: post
post-image: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.ccnahub.com%2Fwp-content%2Fuploads%2F2016%2F03%2Fnmap.png&f=1&nofb=1"
description: Un simple programa escrito en Python + nmap para facilitar el escaneo de puertos
tags:
- Utilidades
- Python
- Nmap
- Programa
---

El escaner de puertos permite conocer que puertos están abiertos en una dirección IP o host. existen 65535 puertos los cuales pueden estar abiertos o cerrados dependiendo de los programas que se esten ejecutando.
<br>
Nmap es un programa de código abierto que sirve para efectuar rastreo de puertos escrito originalmente por Gordon Lyon (más conocido por su alias Fyodor Vaskovich1​) y cuyo desarrollo se encuentra hoy a cargo de una comunidad. Fue creado originalmente para Linux aunque actualmente es multiplataforma. Se usa para evaluar la seguridad de sistemas informáticos, así como para descubrir servicios o servidores en una red.

* [Link de la Pagina de Nmap](https://nmap.org/)

---

# Escaner de puertos <br>

### Para usar el codigo se necesitaran importar las sigentes librerias <br>

`nmap`
<br><br>

para installarla escribir el sigente comando en la terminal:

`pip install python-nmap`

### El codigo es el siguiente <br>

><br>import nmap
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
>print("[Info] Herramienta para escanear los puertos abiertos en una dirección IP")<br>
>print("  ||   Escrito en Python y utiliza Nmap")<br>
><br>
>ip=input("[+] IP Objetivo => ")<br>
>nm = nmap.PortScanner()<br>
>puertos_abiertos="-p "<br>
>results = nm.scan(hosts=ip,arguments="-sT -n -Pn -T4")<br>
>count=0<br>
>#print (results)<br>
>print("\nHost : %s" % ip)<br>
>print("State : %s" % nm[ip].state())<br>
>for proto in nm[ip].all_protocols():<br>
><br>print("Protocol : %s" % proto)
><br>	print()
><br>	lport = nm[ip][proto].keys()
><br>	sorted(lport)
><br>	for port in lport:
><br>		print ("port : %s\tstate : %s" % (port, nm[ip][proto][port]["state"]))
><br>		if count==0:
><br>			puertos_abiertos=puertos_abiertos+str(port)
><br>			count=1
><br>		else:
><br>			puertos_abiertos=puertos_abiertos+","+str(port)
><br>
><br>print("\nPuertos abiertos: "+ puertos_abiertos +" "+str(ip))
><br>


**Una ves copidado el codigo**<br>

Copiar y Pegar el codido en un archivo **.txt** y cambiar la estencion a **.py** y ejecutarlo con python3 si no lo tiene descargado puede ir al sigente link: [Descargar Python](https://www.python.org/downloads/)
<br><br>

**Para ejecutarlo:**
1. Abir la cmd o la Terminal
2. Escrivir: **python3 "ruta del archivo"**
3. Precionamos Enter
4. Introducir la direcion IP que desea Geolocalizar



