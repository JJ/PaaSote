---
author: JJ Merelo
title: Plataformas y apliaciones en la nube
---

# Plataformas y aplicaciones en la nube
## JJ Merelo [`@jjmerelo`](http://twitter.com)
## Universidad de Granada

---
# Qué os voy a contar

* Cómo se diseñan y crean aplicaciones para la nube
* Cómo usar `git` de forma básica.
* Qué es el *despliegue* y cómo usarlo.
* Qué es un PaaS y qué ejemplos hay.
* Cómo usar un PaaS de forma básica.
* Cómo desplegar aplicaciones en un PaaS. 

---

# Ciclo de vida de una aplicación

- Diseño
- Implementación
- Prueba
- Despliegue
- Actualización

---
# Vamos a construir algo

## Vamos a crear una mini-aplicación en la nube.

### Asequible y que podamos probar en breve. Una mini-web

---
# ¿Sugerencias?

* Blog muy simple
* Lista to-do
* Trivial

---
# El ciclo se gestiona automáticamente.

## Si no, no hay manera de saber qué produce un error y por qué.

### O simplemente, hacer las cosas con eficiencia y efectividad.

---

# Continuando integración y lanzamientos

## [**Integración continua**](http://es.wikipedia.org/wiki/Integraci%C3%B3n_continua): tests automáticos + integración.

## [**Lanzamiento continuo**](http://en.wikipedia.org/wiki/Continuous_delivery): ciclos rápidos de lanzamiento.

---
# Por qué molan CI/CD

* Incorporación rápida de mejoras.
* Cambios atómicos: fácil localizar errores.
* Integración desarrollo/operaciones/pruebas de calidad.

---
# Pero todo empieza por el primer paso.

## Creación de un repositorio para tu proyecto.

### Y que el repo sea público.

---
# Usaremos `git` para gestionar el repositorio

## Git es un sistema **moderno** de control de fuentes

### Lo clásico: versionado, atribución, puntos de control del código, fusión.

---
# Pero `git` va mucho más allá

* Permite trabajar de forma distribuida.
* Almacena el estado del repositorio en cada momento.
* Es un sistema de ficheros direccionado por contenido. 
* Se ha convertido en un modo de vida para el programador.

---
# Mejor empezar por GitHub

## Alta en [GitHub](http://github.com).

---
# Software libre

## Toda la nube está basada en software libre

### El mismo concepto no se podría entender si no existiera.

---
# El software es libre si tiene una licencia

## La licencia indica qué se puede hacer con él.

### Pero nunca se puede cambiar la autoría 

---
# Licencias débiles y fuertes

## Las licencias débiles son más fáciles de combinar con software comercial y libre.

## Las **fuertes** obligan a poner la misma licencia al código que las incluya: *copyleft*.

---
# Vamos a crear un repositorio en GitHub

* Nombre y `.gitignore` (usad lo que queráis)

* Readme.md (programa que usar MarkDown)

* *Licencia *: GPL fuerte, Apache o MIT débiles. Elegid la que queráis.

---
# GitHub sin git

## Prácticamente todo se puede hacer desde la web

## También se puede [descargar un interfaz gráfico](http://windows.github.com).

---
# "Editemos un fichero*

## Usando [Markdown](http://joedicastro.com/pages/markdown.html), un lenguaje de etiquetas simplificado, se puede editar el fichero README y añadirle la descripción del proyecto y cómo queremos hacerlo. 

---
# Añadamos a otros compañeros al proyecto

## Empezamos con un repositorio por persona, pero ahora creemos otro y añadamos a las personas con las que vamos a colaborar

---
# Que alguien edite un artículo

## Y en el mensaje, pone `@nick` del siguiente editor (este recibirá email).

### Que lo editen todos los miembros y vuelva al primer editor para revisar.

---
# GitHub sabe lo que hiciste el último commit

## Te muestra los cambios y una serie de estadísticas

### Y es un sistema *social* porque facilita la colaboración.

---
# Koding: programación social

## A un primer nivel, [Koding] es una máquina virtual

### Pero se pueden hacer más cosas.

---
# Abramos una cuenta en Koding.

## Creemos una aplicación (+)

### ¡Y despleguemos!

---
# Usaremos Koding como nuestra plataforma

## Para despegar todo tipo de aplicaciones en Internet.

### ¿Todo el mundo familiar con la línea de órdenes de Linux?

---
# Volvamos a git

## Creemos una pequeña aplicación web

### Django, Ruby on Rails, node.js + express. Ante la duda, este último.

### Usemos simplemente el generador que viene con esas aplicaciones

---
# Por ejemplo, con `express.js`

```
sudo install npm -g express-generator
express mi_nueva_app
```
### Se siguen instrucciones para ejecutar.




