# Clase 01 - Git desarrollo colaborativo

## Markdown (md)
Me permite tomar apuntes y generar documentales. Ademas de introducir un repositorio de GIT. 

# h1
## h2
### h3
#### h4
##### h5
###### h6

### Listas ordenadas y desordenadas

* Punto
* Punto
* Punto

1. Numero 1
2. Numero 2
3. Numero 3

### Imagenes en Markdown

![Logo de Git](git.png)

### Links

<https://git-scm.com/>

## Git

### Instalaciones necesarias

* https://git-scm.com/
* https://code.visualstudio.com/

### Registrarse

* https://github.com/

## Git vs GitHub

![Git vs GitHub](Git vs GitHub.png)

## Verficamos que tenemos instalado git

```sh
git --version
```

## Configuración básica de Git (Se hace una sola vez)

```sh
git config --global user.name "JeroDB-9"
git config --global user.email "debajere@gmail.com"
```

## Listar datos cargados

```sh
git config --list | grep user
git config --global user.name "JeroDB-9"
git config --global user.email "debajere@gmail.com"
```

# Empezar a trabajar con el versionado de un proyecto

```sh
git init # El comando se ejecuta dentro de la carpeta del proyecto
## -- Initialized empty Git repository in C:/Users/Jere_/OneDrive/Desktop/Git - Desarrollo Colaborativo/.git/
```

## Comando para cambiar el nombre de la rama
```sh
git branch -m master main
```

## Para que los cambios sean de forma global
```sh
git config --global init.defaultBranch main
```

## ¿Cómo saber en que area y en que estado estan los archivos?

```sh
git status # Forma larga con info
```

## Areas de Git

## Estado de los Archivos

* untracked (rojo) -> El o los archvios lo ve git pero no les esta dando seguimiento (no sabe el contenido que tiene adentro el archivo)

* staged (verde) -> estado del archivo cuando esta en el staging area, listo para hacer una instanea (commit)

* modified (rojo) -> compara la version del archivo que tengo en el LR contra la version del archivo que tengo en Staging y el Working

## Marcar archivos (marcarlos en el staging area) para que se guarden en el proximo commit
```sh
git add <nombre-archivo>
git add <nombre-archivo1> <nombre-archivo2> <nombre-archivo3>
git add . # marco todos los archivos para que sean parte del proximo commit
```  

## Creamos un commit con los archivos marcados (en el staging area)

```sh
git commit -m "Descripcion del contenido de los archivos"
git comit -m "Empezando con git, explicando markdown y las bases"
```

## Listar commits (mostrar timeline de commits)

```sh
git log #Forma larga
git log --oneline #Forma corta
```
