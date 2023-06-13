# Clase 15

## Configuracion inicial. (una sola vez se hace, al hacer esto cada ves que se haga un commit, va a estar identificado con este nombre y email!) 

```sh
git config --global user.name "Luis Salcedo"   
git config --global user.email "lsalcedogo@gmail.com"
```

## Verificar si todo quedo bien o si hice estas configuraciones:

```sh
git config --get-regexp user
```
*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-*-

## Crear un repositorio (Inicializar un repo)

```sh
git init
```


## Areas del respositorio de GIT

Working Directory (WD): Directorio de trabajo donde se van agregando o quitando los archivos durante el desarrollo.

Staging Area (SA): (Area de Control de Cambios. Area temporal/intermedia).

Local Repo (LR): (Una caja donde voy a ir teniendo tomas las fotos que vaya sacando).

## El estado de los archivos en el repositorios

* untracked: (Archivos que estan en el WD pero git no les esta dando seguimiento) Es el estado actual de todos los archivos. 
* unmodified:(Son archivos que GIT ya esta siguiendo y con respecto al WD, no fueron modificados).
* modified: Archivos que se encuentran en el repositorio (Estan siendo seguidos por GIT) pero difieren con lo que se encuentra actualmente en el WD- .
* staged: Archivos que estan en el area temporal/intermedia

## El estado de los archivos en si mismo, de forma independiente

## Saber estado actual de los archivos
* git status

## Mover de una direccion (sacarle una foto):

* git add

## Sacarle la foto defintiva

* git commit -m "Agrego index.html"

## Saber estado actual de los archivos
* git estatus

## Quiero ver la cajita de fotos (la informacion que tengo en local repo)
* git log

    ## Cajita de foto mas corta (Resumen)
    * git log --oneline

## Saber estado actual de los archivos

```sh
git status
```

## Voy a poder mover los archivos de WD al SA eso lo hago con

```sh
git add <nombre-archivo>
git add index.html
git add readme.md css/estilos.css
git add . #agrego todos los archivos que estan (untracked,modified)
```

## La historia de commits (La caja de fotos)

```sh
git log # La historia de commit detallada
git log --oneline #Historia resumidad
```

## Nota: Si la consola queda bloqueada y no puedo salir del listado tengo apretar la tecla q (quit)


## validar que linea fue modificada

git diff

## restaurar la modificacion Git

git restore


## clase 16

## .gitignore

Este archivo me sirve para ingnorar carpetas o archivos que no quiero que sean parte del repositorio. Normalmente va sobre la raiz del proyecto.

Necesito crear el archivo **.gitignore**

```hs
touch .gitignore
```







