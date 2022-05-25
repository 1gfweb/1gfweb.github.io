---
title: Geolocalizr IPs
layout: post
post-image: "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fwww.profesionalreview.com%2Fwp-content%2Fuploads%2F2019%2F12%2Fcompass-destination-direction-find-globe-gps-1569701-pxhere.com_.jpg&f=1&nofb=1"
description: Un simple programa escrito en Python para la geolocalizacion de equipos mediante su ip publica
tags:
- Utilidades
- Python
- Herramienta
- Programa
---

La Geolocalización de IPs es la identificación de la ubicación geográfica de un dispositivo, como un teléfono móvil, dispositivo, computadora portátil, servidor, etc., mediante el uso de una dirección IP publica.
este programa puede localizar la ip publica de un dispocitivo ya que esta conectado con una api

* [Link de la Api](http://ip-api.com/json/)

---

### Para usar el codigo se necesitaran importar las sigentes librerias <br>

`requests`

`json`
<br><br>

En caso de que no esten instaladas, escribir los sigentes comandos en la terminal:

`pip install requests`

`pip install json`

### El codigo es el siguiente <br>

>import requests 
><br>
>import json
><br>
>api_url = "http://ip-api.com/json/"
><br>
>parametros = 'status,country,countryCode,region,regionName,city,zip,lat,lon,timezone,isp,org,as,query'
><br>
>data = {"fields":parametros}
><br><br>
>def ip_scraping(ip=""):
><br>	res = requests.get(api_url+ip, data=data)
><br>	api_json_res = json.loads(res.content)
><br>	return api_json_res
>if __name__ == '__main__':
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
>ip = input("Ingrese la dirección IP: ")
><br>
>par = parametros.split(",")
>for x in par:
>print(x.upper(), ":")
>print(ip_scraping(ip)[x])
>print("\n")int("\nPuertos abiertos: "+ puertos_abiertos +" "+str(ip))
><br>


**Una ves copidado el codigo**<br>

Copiar y Pegar el codido en un archivo **.txt** y cambiar la estencion a **.py** y ejecutarlo con python3 si no lo tiene descargado puede ir al sigente link: [Descargar Python](https://www.python.org/downloads/)
<br><br>

**Para ejecutarlo:**
1. Abir la cmd o la Terminal
2. Escrivir: **python3 "ruta del archivo"**
3. Precionamos Enter
4. Introducir la direcion IP que desea Geolocalizar



