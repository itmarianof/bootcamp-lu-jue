# Clase 15

## Configuración inicial.

```sh
git config --global user.name "Maximiliano Principe"
git config --global user.email "mlapeducacionit@gmail.com"
```

## Verificar si todo quedo bien o si hice estas configuraciones

```sh
git config --get-regexp user
```

## Crear un repositorio (Inicializar un repo)

```sh
git init
```

## Areas del repositorio de GIT

3 Áreas

* Working Directory (WD): Directorio de trabajo donde se van agregando o quitando los archivos durante el desarrollo
* Staging Area (SA): (Área de control de cambios. Área temporal/intermedia)
* Local Repo (LR): (Una caja donde voy a ir teniendo todas las fotos que vaya sacando)

## El estado de los archivos

* untracked: (Archivos que están en el WD pero GIT no les esta dando seguimiento)
* unmodified: (Archivos que GIT ya esta siguiendo y con respecto al WD, no fueron modificados)
* modified: Archivos que se encuentran en el repositorio (Están siendo seguidos por GIT) pero difieren con lo que se encuentra actualmente en el WD
* staged: Archivos que están en el area temporal/intermedia

## Saber estado actual de los archivos

```sh
git status
```

## Voy a poder mover los archivos de WD al SA

```sh
git add <nombre-archivo>
git add index.html
git add README.md css/estilos.css
git add . # Agrego todos los archivos que están (UNTRACKED, MODIFIED)
```

## La historia de commits (La caja de fotos)

```sh
git log # La historia de commit detallada
git log --oneline # Historia resumida
```

Nota: Si la consola queda bloqueada y no puedo salir del listado tengo apretar la tecla q (quit)


## Si quiero ver los cambios que tengo entre el WD y LR

```sh
git diff
```