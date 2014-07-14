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

# El ciclo se gestiona automáticamente.

## Si no, no hay manera de saber qué produce un error y por qué.

### O simplemente, hacer las cosas con eficiencia y efectividad.

---

# Continuando integración y lanzamientos

## [**Integración continua**](http://es.wikipedia.org/wiki/Integraci%C3%B3n_continua): tests automáticos + integración.

## [**Lanzamiento continuo**](http://en.wikipedia.org/wiki/Continuous_delivery): ciclos rápidos de lanzamiento

---
# Ventajas de integración/lanzamiento continuos

* Incorporación rápida de mejoras.
* Cambios atómicos: fácil localizar errores.
* Integración desarrollo/operaciones/pruebas de calidad

---
# Pero todo empieza por el primer paso.

## Creación de un repositorio para tu proyecto.

### Y que el repo sea público.

---
# Usaremos `git` para gestionar el respositorio

## Git es un sistema de control de fuentes

### Lo clásico: versionado, atribución, puntos de control del código, fusión.

---
# Pero `git` va mucho más allá

* Es un sistema distribuido
* Almacena el estado del repositorio en cada momento.
* Es un sistema de ficheros direccionado por contenido. 
