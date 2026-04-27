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

