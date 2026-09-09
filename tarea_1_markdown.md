# 1 tabla de markdown.

| comando | nombre o significado | para que sirve |
|---------|----------------------|----------------|
| **cd** | *change directory* | Cambiar de carpeta | 
| **ls** | *list* | Contenido de un directorio en forma de lista | 
| **mkdir** | *make directory* | Crear directorio/carpeta |
| **clear** | *clear* | Limpiar la terminal | 
| **pwd** | *print working directory* | te dice en qué carpeta estás actualmente.
| **cat** | *concatenate* | Mostrar contenido de archivos |
| **mv** | *move* | Mover o renombrar | 
| **cp** | *copy* | Copiar archivos/carpetas | 
| **touch** | *tactil o toque* | Crear archivos vacíos | 
| **kill** | *kill* | Enviar una señal a un proceso | 
| **ps** | *process status* | Ver procesos | 

```bash
cd Desktop
cd Documentos
```
```bash
ls
```
```bash
mkdir sopa_de_pollo
```
```bash
clear 
```
```bash
pwd
```
```bash
cat archivo.txt
```
```bash
mv a.txt b.txt
```
```bash
cp a.txt copia.txt
```
```bash
touch nombre_archivo.txt
```
```bash
kill 1234
```
```bash
ps aux
```
# 2. Resumen de comandos básicos de Git

| Comando | Definición / Función |
|---|---|
| `git init` | Inicializa un nuevo repositorio de Git. |
| `git clone` | Crea una copia local de un repositorio remoto. |
| `git diff` | Muestra las diferencias entre los cambios realizados. |
| `git status` | Muestra el estado actual del repositorio. |
| `git merge` | Combina los cambios de una rama con otra. |
| `git config` | Configura opciones de Git, como el nombre y correo. |
| `git add` | Agrega cambios al área de preparación. |
| `git log` | Muestra el historial de commits. |
| `git commit` | Guarda los cambios preparados en el historial. |
| `git checkout` | Permite cambiar de rama o recuperar una versión. |
| `git branch` | Permite crear, listar y administrar ramas. |
| `git pull` | Descarga e integra cambios del repositorio remoto. |
| `git push` | Envía los commits locales al repositorio remoto. |
| `git fetch` | Descarga cambios remotos sin integrarlos. |

```bash
git init
```
```bash
git clone https://github.com/usuario/proyecto.git 
```
```bash
git diff
```
```bash
git status
```
```bash
git merge desarrollo
```
```bash
git config --global user.name "Juan Pérez"
```
```bash
git config --global user.email "juan@ejemplo.com"
```
```bash
git add .
```
```bash
git log --oneline
```
```bash
git commit -m "Agrega página principal"
```
```bash
git checkout desarrollo
```
```bash
git checkout -b nueva-funcionalidad
```
```bash
git branch desarrollo
```
```bash
git pull origin main
```
```bash
git push origin main
```
```bash
git fetch origin
```

# 3. Proceso para crear un repositorio de Git desde PowerShell

Para crear un repositorio de Git desde PowerShell, se deben seguir los siguientes pasos:

## Paso 1. Crear una carpeta y entrar en ella

Primero se crea una carpeta para el proyecto utilizando `mkdir`. Después, se utiliza `cd` para entrar en la carpeta.

```powershell
mkdir MiProyecto
cd MiProyecto
```

## Paso 2. Inicializar el repositorio

Una vez dentro de la carpeta, se utiliza `git init` para convertirla en un repositorio de Git.

```powershell
git init
```

## Paso 3. Agregar los archivos

Después de crear o colocar los archivos del proyecto dentro de la carpeta, se utiliza `git add -A` para agregar todos los archivos y cambios al área de preparación.

```powershell
git add -A
```

## Paso 4. Realizar el primer commit

Finalmente, se realiza el primer commit utilizando `git commit -m`. El mensaje permite identificar qué cambios se guardaron.

```powershell
git commit -m "mensaje inicial"
```

## Proceso completo

Los comandos se deben ejecutar en el siguiente orden:

```powershell
mkdir MiProyecto
cd MiProyecto
git init
git add -A
git commit -m "mensaje inicial"
```

> **Nota:** Antes de utilizar `git add -A`, debe existir al menos un archivo dentro de la carpeta del proyecto.