---
layout: post
title: Buscar cuentas en redes sociales por el nombre.
description: A veces queremos buscar información sobre alguien, ya sea por curiosidad o cualquier otro fin.
hide_last_modified: true
comments: false
---
# Buscar cuentas en redes sociales por el nombre.

Buscar cuentas de usuario de una persona no es nada ilegal ni puede acarrear consecuencias, pero si puede ser molesto para el usuario que es buscado.

### Esto no es ilegal, pero sin embargo puede molestarle al usuario a quien busquemos.

La herramienta que vamos a usar es un script **programado en Python 3** cuya utilidad es buscar cuentas con el nombre que le demos en la red.
El script se llama **Sherlock.py** y este es el github del proyecto [sherlock.py](https://github.com/sherlock-project/sherlock).

Como es lógico, para usar esta herramienta hace falta tener Python instalado en nuestro sistema. 
## Instalación de Python 3

**Si ya lo tenéis instalado** podéis saltaros este paso.
### Linux
*Normalmente* en linux siempre viene instalado, pero si no lo tenéis se puede instalar con el siguiente comando:
~~~
sudo apt update 
sudo apt upgrade -y
sudo apt install python3
~~~
O si usáis un derivado de arch:
~~~
sudo pacman -Syu
sudo pacman -S python3
~~~

### Windows
Hay varias formas de instalar Python en Windows, yo *solo voy a enseñar dos* si una no os funciona usáis la otra.

#### Primera forma.
Presionad el atajo "Win+R" y ponéis "cmd" en la ventanita que os sale.
Ponéis:
~~~
python3
~~~
Y se os abrirá la Tienda de Microsoft con la aplicación de Python. La instaláis y ya lo tendríais. Si no os funciona usad, la siguiente forma.

#### Segunda forma.
Accedéis a la página oficial de Python y en la [página de descargas](https://www.python.org/downloads/) le dais a descargar.

Ejecutáis el archivo descargado y os saldrá esta ventana, seleccionáis las opciones señaladas en rojo y le dais a *"Install Now"* como indica la flecha verde.
![](https://raw.githubusercontent.com/H4ckX0R/h4ckx0r.github.io/master/tutoriales/Imagenes/Buscar-usernames-en-la-red/Instalarpython3img1.png)

Esperáis a que se instale y cuando termine le dais al botón que pone *"Close"*

## Descargando e instalando Sherlock.py

Este proceso es muy sencillo, pero es diferente en Linux y Windows.
### Descargando e instalando el repositorio en Linux.
Solamente tenéis que ejecutar estos tres comandos en la Terminal.
Ponéis:
~~~
git clone https://github.com/sherlock-project/sherlock.git
cd sherlock
python3 -m pip install -r requirements.txt
~~~

### Descargando e instalando Sherlock.py en Windows.
Entramos en el github del proyecto a través de este [enlace](https://github.com/sherlock-project/sherlock).
Luego le damos a *"Code"* y luego a *"Download ZIP"* como se ve en la imagen.
![](https://raw.githubusercontent.com/H4ckX0R/h4ckx0r.github.io/master/tutoriales/Imagenes/Buscar-usernames-en-la-red/Descargarsherlockenwindows.png)

Luego nos vamos a la carpeta donde lo hayamos descargado y extraemos el zip, a continuación entramos en la carpeta sherlock. En la parte superior izquierda hay un botón que pone *"Archivos"*, le damos y luego seleccionamos *"Abrir Windows PowerShell"* (No hace falta abrirlo como administrador).

Ahora en esa ventana negra que se os ha abierto ponéis el siguiente comando:

Si usaste la primera forma de instalar Python, pon:
~~~
python3 -m pip install -r requirements.txt
~~~

Y si usaste la segunda forma
~~~
python -m pip install -r requirements.txt
~~~
Una vez termine ya se habrá instalado.

## Usando Sherlock.py

Se usan igual tanto en Linux como en Windows, así que no creo que haya problema. 
En Windows simplemente tenéis que abrir el Windows PowerShell en la carpeta de sherlock como habéis hecho antes, **pero entrando nuevamente en la carpeta sherlock que hay dentro de la anterior, y estando ahí iniciáis la terminal como antes**.

Y en Linux abrir la terminal con Ctrl+Alt+T (O el que tengamos configurado por defecto) y hacer:
~~~
cd sherlock/sherlock
~~~

En este punto las dos terminales están en el mismo punto. A partir de aquí se hace igual en los dos sistemas.
**Si en windows habéis usado la segunda forma, en vez de poner *"python3"*, ponéis simplemente *"python"*.**

Ahora para buscar un nombre de usuario en la red, ponéis:
~~~
python3 sherlock.py nombreabuscar
~~~

Podéis también buscar varios a la vez separándolos por espacios así:
~~~
python3 sherlock.py nombreabuscar1 nombreabuscar2 nombreabuscar3
~~~

Si necesitáis ayuda, con este comando os mostrará la ayuda del script:
~~~
python3 sherlock.py -h
~~~

**Es posible que algunas webs no sean correctas, ya que es un sistema automatizado, pero suele ir bien. También puede ser que falten algunas webs**
**En el campo de búsqueda solo podéis poner letras y números, la mayoría de símbolos diferentes no los soporta**