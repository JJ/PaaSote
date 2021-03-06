---
author: JJ Merelo
title: Plataformas y apliaciones en la nube
---

# Plataformas y aplicaciones en la nube
## JJ Merelo [`@jjmerelo`](http://twitter.com)
## Universidad de Granada

---
# No se trata sólo de usar plataformas nubosas

## Se trata de aprender la metodología de desarrollo en la nube. 

---

# Qué os voy a contar

* Cómo se diseñan y crean aplicaciones para la nube
* Cómo usar `git` de forma básica.
* Qué es DevOps y por qué importa.
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

### Usadas, por ejemplo, en Android o el servidor Apache.

---
# Licencias *copyleft* 

## Las **fuertes** obligan a poner la misma licencia al código que las incluya: *copyleft*.

### Por ejemplo, el kernel de Linux. 

---
# Vamos a crear un repositorio en GitHub

* Nombre y `.gitignore` (usad lo que queráis)

* Readme.md (programa que usar MarkDown)

* *Licencia*: GPL fuerte, Apache o MIT débiles. Elegid la que queráis.

---
# GitHub sin git

## Prácticamente todo se puede hacer desde la web

## También se puede [descargar un interfaz gráfico](http://windows.github.com).

---
# "Editemos" un fichero

## Usando [Markdown](http://joedicastro.com/pages/markdown.html), un lenguaje de etiquetas simplificado, se puede editar el fichero README y añadirle la descripción del proyecto y cómo queremos hacerlo. 

---
# Añadamos a otros compañeros al proyecto

1. Crear un nuevo repositorio
2. Añadir al grupo de colaboradores

### Este repositorio lo usaremos para desarrollar la aplicación.

---
# Que alguien edite un artículo

## Y en el mensaje, que ponga `@nick` del siguiente editor (este recibirá email).

### Que lo editen todos los miembros y vuelva al primer editor para revisar.

---
# GitHub sabe lo que hiciste el último commit

## Te muestra los cambios y una serie de estadísticas

### Y es un sistema *social* porque facilita la colaboración.

---
# Koding: programación social

## A un primer nivel, [Koding](http://koding.com) es una máquina virtual.

### Pero es también un entorno colaborativo de trabajo y despliegue.

---
# Abramos una cuenta en Koding.

## Creemos una aplicación (+).

### ¡Y despleguemos!

---
# Koding crea aplicaciones en *CoffeeScript*

## Una versión simplificada de JavaScript.

### Se compila a JavaScript.

---
# Usaremos Koding como nuestra plataforma de desarrollo.

## Para despegar todo tipo de aplicaciones en Internet.

### ¿Todo el mundo familiar con la línea de órdenes de Linux?

---
# O usa cualquier otra máquina virtual.

## Siempre que tengas acceso shell y puedas instalar cosas.

---
# Creemos una aplicación para git

## Creemos una pequeña aplicación web

### Django, Ruby on Rails, node.js + express. 

### Usemos simplemente el generador que viene con esas aplicaciones.

---
# Por ejemplo, con `express.js`

```
sudo install npm -g express-generator
express mi_nueva_app
```
### Se siguen instrucciones para ejecutar.

---
# Pero esta aplicación tendrá su ciclo de vida

## Vamos a añadirla al repositorio

---
# Descargamos el repositorio

``` 
git clone git@github.com:minick/miproyecto.git
``` 

### Crea un repositorio local y descarga los fuentes de nuestro proyecto.

---
# Añadimos los nuevos fuentes

## Copiamos al subdirectorio, 

``` 
cd mi_nueva_app
git add .
``` 

### Añade todos los ficheros creados al repositorio

---
# Pero hay que sincronizar

``` 
git commit -am "Aplicación generada"
```
### Guarda el estado de los ficheros modificados 

```
git push
```
### Sincroniza los cambios locales con el repo remoto.

---
# Cuando hacer commit

## Cada vez que sehaga un cambio significativo.

### Regla 50+72: título en 50 caracteres, línea en blanco, resto en líneas de 72 caracteres.

---
# ¿Cuantos lenguajes llevamos ya?

## Se debe aprender a crear aplicaciones, no a programar en un lenguaje.

### Una aplicación web normal incluye varios: JavaScript, HTML, CSS, Python o PHP o Ruby, XML o YAML o JSON...  

---
# Interludio sobre PaaS

### (Úsese para acabar de hacer los ejercicios anteriores).

## *PaaS* == Platform as a Service. 

---
# Un PaaS proporciona un *full stack*

## Almacenamiento de datos + marco de aplicaciones + servidor web.

### En ocasiones, usable también como un IaaS.

---
# La mayoría siguen un modelo *freemium*

## Proporcionan un grado de servicio gratuito.

### Incluye pocas máquinas virtuales y con poca potencia.

---
# Ejemplos: Heroku y OpenShift

## Abrir cuenta en alguno de ellos o en los dos.

### Primero OpenShift, más flexibilidad.

---
# Creación rápida de aplicaciones

## OpenShift permite instalar Wordpress en segundos.

## Heroku, más enfocado a node.js. 

---
# Crea tu *stack* rápidamente en alguno de ellos

## Y tuitea con #paasunia el resultado.

---
# Pero no solo de *stacks* vive el hombre

## Vamos a desplegar nuestra aplicación en este PaaS

### Pero antes habrá que aprender una cosa o tres.

---
# ¿Cuantas máquinas estamos usando?

## Cada miembro del equipo tiene la suya.

## + máquina de pruebas + máquina de explotación.

---
# Mucho arroz para tan poco pollo

## Pero lo importante es que *el entorno de desarrollo tiene que ser el mismo*.

### Y puede que hagan falta varios entornos en el desarrollo.

---
# *DevOps* al rescate

## *DevOps* == Desarrollo + operaciones (+ calidad o test).

### Integra "Sistemas" con el equipo de desarrollo, para proporcionar soporte eficiente al mismo.

---
# *DevOps* también *programa* los sistemas

## Entornos de desarrollo/explotación reproducibles: descritos por software.

### E integrados en el sistema de control de fuentes.

---
# Un entorno para dominarlos a todos.

## `rbenv`, `rvm`, `virtualenv`, `perlbrew`, `nave`

### Descargan y seleccionan versiones específicas de lenguajes *a nivel de usuario*.

---
# Trabajemos con `nave`

## Instalad `nave` (u otro entorno) en koding y ejecutad el programa generado anteriormente.

### ¿Funciona en la última versión?  ¿Y en una antigua que puede estar instalada por alguien?

---
# PaaS no es sólo una plataforma para alojar aplicaciones

## Es un cambio de la filosofía de desarrollo que implica todo el ciclo de vida de una aplicación. 

### Lo que hemos dicho desde el principio. 

---
# Vamos a hacer pruebas con la aplicación

## Pero no queremos romper nada

```
git checkout -b pruebas
```

### Crea una nueva rama con los mismos ficheros que la original.

```
git push --set-upstream origin pruebas
```

### Crea la rama en el repo remoto y la une con el repo local (tras cambios).

---
# *Feature branches* o ramas *dev*

### Hay muchas escuelas de desarrollo: con dos ramas, con tres, con *n*. 

## Habitual: una rama de desarrollo (`dev`) y una principal (`master`)

---
# ¿Cómo se fusionan ramas?

## ¡No te lo digo!

### No se fusionan *a menos que hayan pasado los __tests__*.

---
# Venga, va, ¿cómo se pasan los tests?

## Todo desarrollo moderno es TDD: *Test-driven development*

### A cada *push*, se pasa una serie de tests.

---
# Sí, vale, eso es que se lo paso a mi colega...

## No. Los tests deben estar automatizados.

---
# Cada lenguaje de programación tiene sus marcos de tests

## Tests unitarios, tests de integración. 

## JUnit, *unit, mocha (para JS)...

---
# Los tests tiene un formato de salida estándar 

## Por eso se pueden ejecutar fácilmente y automáticamente por herramientas universales.

---
# Creemos tests unitarios para nuestra aplicación

## Ya que somos varios, podemos encargárselo a una persona del grupo.

---
# Ejemplo en mocha 

```
var request = require('supertest');  
var server=require(__dirname + '/../web.js');
var port = Number(process.env.PORT || 5000);
request=request("http://localhost:"+port);
```

---
# Continuando

```
describe('Web', function(){
	     it('Debería devolver la raíz', function(){
		    request.get("/")
			.expect(200)
			.end(function(err,res) {
				 if (err) {
				     throw err ;
				 }
			     });
		});
});
```

---
# El ejemplo lo dice todo

## Se guarda en `test/route.js`

## Se ejecuta con `mocha`

---
# No importa la herramienta.

## Ésta sólo es un ejemplo.

## Lo importante es *usar siempre tests*

---
## Porque una vez que tienes tests...

# Tienes integración continua. 

## GitHub se puede configurar para pasar tests cada vez que se haga un push. 

---
# Usemos [Travis](http://travis-ci.org) o Shippable

## Travis se activa desde GitHub, en la pestaña *Web Hooks*

## Configuración eh YAML

---
# Por ejemplo, para mocha en Shippable
```
language: node_js
node_js:
  - 0.10.25
before_install:
 - npm install supertest
before_script:
 - mkdir -p shippable/testresults
script:
  - mocha
```

---
# ¡Otro lenguaje más!

## Y los que te rondaré, morena.

---
# Recapitulemos

## ¿Qué lenguajes hace falta conocer?

1. Programación/scripting: Ruby, JavaScript, Perl, Python...
2. Presentación: HTML, CSS, pero también SASS, Jade...
3. Configuración/serialización: XML, YAML, JSON
4. Datos: SQL o lenguajes específicos de herramienta

---
# Ya hemos testeado

## Ahora ya podemos fusionar las ramas.

### git hace el "trabajo duro". 

---
# Para fusionar ramas

```
git checkout master
git pull pruebas
```

### Si no hay conflictos, esto se incorpora a la rama master. ¡CI!

---
# Despleganco una aplicación

1. Creación del entorno desde línea de órdenes o panel (seleccionar *gears* o *dynos*)

2. Configuración de la aplicación (`Procfile` o similar)

3. Desplegar la aplicación.

---
# Ya podemos desplegar

### (Aunque antes habría que hacer pruebas de integración).


```
git remote add \
    openshift ssh://{id}@objiv-jmerelo.rhcloud.com/~/git/objiv.git/
```

### Heroku también usa algo similar.

---

# Y colorín, colorado...

### (No sé si llegaremos hasta aquí)

1. Cambiad la forma de pensar y de crear aplicaciones.

2. Probad una herramienta nueva cada mes.

3. Pendad en la nube.

---
# Eso es todo

## Muchas gracias.

