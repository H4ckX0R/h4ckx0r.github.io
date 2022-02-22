---
layout: post
title: No Sleep
description: Plugin para gestionar el uso de las camas en SMPs
hide_last_modified: true
comments: false
---
# No Sleep

### Versión más reciente: 1.1.0

### Links de descarga

No Sleep es un plugin que he programado y pienso seguir mejorando con la intención de ayudar a gestionar las camas en servidores SMP.

## Funcionamiento

Solo hay un comando: `/nodormir`
Este comando cumple **todas** las funciones del plugin.

**Para poder ejecutar el comando es obligatorio que los usuarios tengan el permiso `no.sleep.command.permision`**

### Bloqueo de camas

Cuando un jugador o la consola pongan el comando `/nodormir` el plugin avisa por el chat y bloquea las camas. Cuando se intenta dormir y las camas están bloqueadas, el plugin avisa solo al jugador que quiere dormir que las camas están bloqueadas.

### Desbloqueo de camas

Hay 2 formas por las que se pueden desbloquear las camas:

#### Desactivación por el ejecutor del comando

Cuando el jugador que ha bloqueado las camas vuelve a ejecutar el comando, estas se desbloquean instantáneamente y el plugin envía un mensaje por el chat, diciendo que las camas han sido desbloqueadas.

Otra forma es que el jugador que las ha bloqueado, se salga del servidor, esto también desactiva el bloqueo.

#### Por votación

En el caso de que se quieran desbloquear las camas y el jugador que las ha bloqueado esté AFK o las haya bloqueado para molestar al resto del servidor, estas se pueden desbloquear por votación.

Para ello, los jugadores que quieran desbloquear las camas, deben poner `/nodormir`. Al poner este comando, por defecto calcula el [50%](https://h4ckx0r.github.io/plugins/es) de los jugadores en el servidor, (sin contar al jugador que ha ejecutado el comando) y redondea ese porcentaje, una vez tiene el porcentaje, dice cuantos jugadores quedan por votar para que se desbloqueen las camas por votación.

Cada jugador solo puede votar 1 vez, en el caso de que intente votar varias veces, el servidor le avisará con un mensaje de que ya ha votado.

En cuanto se desbloquean las camas, si se ejecuta el comando `/nodormir` se vuelven a bloquear las camas.

## Próximamente

Este plugin por ahora está preconfigurado y no se puede cambiar su configuración. Añadiré dentro de poco un archivo de configuración donde se podrá cambiar de idioma y el porcentaje de jugadores que tienen que votar.

## Changelog

### [Página web de Spigot](https://www.spigotmc.org/resources/no-sleep.99950/history)


| **Versión** | **Enlace de descarga**                                                            | **Cambios**                                                                                                      | **Fecha de actualización** |
| -------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------- |
| 1.1.0        | [link](https://www.spigotmc.org/resources/no-sleep.99950/download?version=440894) | Ahora durante la votación, el plugin no tiene en cuenta en el porcentaje al jugador que ha bloqueado las camas. | 12/02/2022                  |
| 1.0.1        | [link](https://www.spigotmc.org/resources/no-sleep.99950/download?version=440882) | Soluciona un error que sucedía durante la votación.                                                            | 12/02/2022                  |
| 1.0.0        | [link](https://www.spigotmc.org/resources/no-sleep.99950/download?version=440870) | Publicación del plugin.                                                                                         | 12/02/2022                  |
