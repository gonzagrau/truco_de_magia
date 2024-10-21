# GIT CHEATSHEAT
*Algunos códigos que vamos a utilizar en el taller de Git/Github de CESABI en colaboración con EMBS ITBA*

## Comando básicos de git

**Configuración inicial de git**

```
git config --global user.name "TU NOMBRE"
git config --global user.email "tu.email@dominio.com"
git config --global core.editor "code --wait"
```

**Crear un repositorio**

```
mkdir cesabi_tutorial
cd cesabi_tutorial
git init
```

**Agregar un archivo a la staging area**

```
git add archivo
```

**Agregar todo el directorio local a la staging area**

```
git add .
```

**Resetear la staging area**

```
git reset
```

**Hacer un nuevo commit**

```
git commit -m 'mensaje descriptivo'
```


**Actualizar mi repositorio local con los nuevos commits del remoto**

```
git pull
```

**Actualizar el repositorio remoto con mis nuevos commits locales**

```
git push
```

**Crear una nueva rama**

```
git branch nombre_rama
```

**Mover HEAD a otra rama**

```
git checkout nombre_rama
```

**Combinar ramas**

```
git checkout main
git merge nombre_rama
```

**Clonar un repositorio remoto**

```
git clone direccion/del/repo
```

## Configuración SSH

**Ver claves ssh preexistentes en el sistema**

```
ls -al ~/.ssh
```

**Generar clave ssh**
```
ssh-keygen -t ed25519 -c "nombre_de_la_clave"
```

**Inicializar conexión con el agente ssh**

```
eval "$(ssh-agent -s)"
```

**Agregar la clave al agente**
```
ssh-add ~/.ssh/id_ed25519

```

**Imprimir la clave en consola para copiarla**
```
cat ~/.ssh/id_ed25519.pub
```

**Chequear la conexion**

```
ssh -T git@github.com
```


