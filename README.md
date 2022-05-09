# GIT Básico

## Instalación

Instalación desde el asistente de Git

## Comandos para credenciales en nuestro equipo


```
git config --global user.name "JorgeCF"
git config --global user.email "jorgecarfacpsico@gmail.com"
```

## Crear un repositorio Git

```
git init
```

Ese comando crea tres fases.

Working directory: registra cambios en el proyecto: añadir código, modificarlo, eliminarlo. También registra cambios en el
directorio como crear directorios, añadir imágenes, etc.

```
comando 'add'
```

Los cambios se añaden mediante este comando a la segunda fase:

Staging Area: almacena los cambios registrados por el working directory, creando un grupo de cambios.

Cuando el conjunto de cambios sea suficiente para ser significativo, hace un proceso para pasar al repositorio

```
comando 'commit'
```

Repositorio: guarda grupos de cambios hechos en el código y les pone un identificador para diferenciarlos.

## Comprobar el estado de Git

Ver la situación en la que están los cambios desde el último commit

```
git status
```

## Añadir archivos al Staging Area

```
git add -A
```
Añade todos los cambios pendientes al staging area

## Añadir archivos al Repository

```
git commit -m "mensaje del commit"
```

Crea un commit con los cambios stageados y los manda al repositorio.
El mensaje del commit lo que hace es dejar clara la función del commit: arreglar un bug, cambiar algo, etc.
El primer commit se suele llamar initial.

Para ver los commit se puede utilizar git log, o una extensión llamada Git Graph.

## Deshacer cambios a partir de los commits

Tenemos dos opciones

```
git reset --soft <código-commit>
```
--soft nos hace volver a un commit anterior sin deshacer los cambios que hemos hecho. Es la opción menos
utilizada.

```
git reset --soft <código-commit>
```

--hard te vuelve a un commit anterior, y deshace los cambios de código que hayas hecho anteriores a ese commit.
No es útil si queremos hacer un cambio focalizado, por ejemplo, si queremos borrar algo del index.html pero quieres
conservar lo del readme.md, es mejor hacer un --soft para borrar la parte que nos interesa.

## Subir a GitHub

Github es una nube en la que subimos los repositorios para almacenarlos y poder trabajar en grupo, accediendo varias personas al mismo repositorio.