# Clase 02 - Git desarrollo colaborativo

## Repaso comando vistos.

> Muestro el estado y area en la que estan los archivos

> agrego archivos que estan en el working directory para posteriormente hacer un commit

```sh
git add class-01/_ref/* #Marco todos los archivos ques tan dentro de la carpeta _ref
git add . # Este comando me sirve para marcar todos los archivos para luego hacer un commit
```

> Hacemos un commit (Snapshot, instantanea)

```sh
git commit -m "Mensaje descriptivo" #80 caracteres
```

> Listo timeline de commits (Listado de commits)

```sh
git log --oneline
```

# .gitignore
Es un archivo que me permite indicarle a GIT que no quiero que la carpeta o el archivo sea controlado por Git

# .gitkeep
Es un archivo que me permite darle seguimiento a una carpeta que quiero sea parte del repo pero que este vacia.

**Se hace de esta manera porque GIT no versiona carpetas vacias.**

<htpps://www.campusmvp.es/recursos/post/que-son-los-archivos-gitkeep-en-git.aspx?srsltid=AfmBOopAgwXq8qolbnQNfpXDO2-9Wjq75qVgDspc0HQpq16JJw2MUZz>

# Ver la diferencia entre Wd y SA o LR

```sh
git diff
```

# Ver mas info. de un commit

```sh
git show<HASH>
git show cb20a1a
```
## Recuperar archivos desde el LOCAL REPO

```sh
git restore <nombre-archivo1> <nombre-archivo2>
git restore clase-02/README.md
git restore . #Recupera todos los archivos a la version actual del LR
```

## Comando para hacer add y commits en un solo paso

**IMPORTANTE**: Solo funciona con archivo que yan estan seguidos por GIT. Si tengo archivos intracked esos archivos cuando haga el commando no se van agregar al Staging Area

```sh
git commit -am "mensaje descriptivo" # -a <---- ADD | -m <----- Mensaje
```
