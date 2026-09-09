# Resumen de comandos básicos de PowerShell y Git

# 1. Resumen de comandos básicos de PowerShell

## `cd` — cambiar de directorio

### Definición (qué hace)

`cd` permite cambiar el directorio o carpeta de trabajo actual.

---

### Ejemplo de uso (código en bloque)

```bash
cd Desktop
cd Documentos
```

---

## `ls` — listar contenido

### Definición (qué hace)

`ls` muestra el contenido de un directorio o carpeta en forma de lista.

---

### Ejemplo de uso (código en bloque)

```bash
ls
```

---

## `mkdir` — crear directorio

### Definición (qué hace)

`mkdir` permite crear una nueva carpeta o directorio.

---

### Ejemplo de uso (código en bloque)

```bash
mkdir sopa_de_pollo
```

---

## `clear` — limpiar la terminal

### Definición (qué hace)

`clear` limpia el contenido visible de la terminal.

---

### Ejemplo de uso (código en bloque)

```bash
clear
```

---

## `pwd` — mostrar directorio actual

### Definición (qué hace)

`pwd` muestra la ubicación o directorio de trabajo actual.

---

### Ejemplo de uso (código en bloque)

```bash
pwd
```

---

## `cat` — mostrar contenido

### Definición (qué hace)

`cat` permite mostrar el contenido de un archivo de texto en la terminal.

---

### Ejemplo de uso (código en bloque)

```bash
cat archivo.txt
```

---

## `cp` — copiar archivos

### Definición (qué hace)

`cp` permite copiar archivos o carpetas de una ubicación a otra.

---

### Ejemplo de uso (código en bloque)

```bash
cp a.txt copia.txt
```

---

## `mv` — mover o renombrar

### Definición (qué hace)

`mv` permite mover archivos o carpetas y también cambiarles el nombre.

---

### Ejemplo de uso (código en bloque)

```bash
mv a.txt b.txt
```

---

# 2. Resumen de comandos básicos de Git

## `git init` — inicializar un repositorio

### Definición (qué hace)

`git init` inicializa un nuevo repositorio de Git en la carpeta actual.

---

### Ejemplo de uso (código en bloque)

```bash
git init
```

---

## `git clone` — clonar un repositorio

### Definición (qué hace)

`git clone` crea una copia local de un repositorio remoto.

---

### Ejemplo de uso (código en bloque)

```bash
git clone https://github.com/usuario/proyecto.git
```

---

## `git diff` — mostrar diferencias

### Definición (qué hace)

`git diff` muestra las diferencias entre los cambios realizados en los archivos y las versiones anteriores.

---

### Ejemplo de uso (código en bloque)

```bash
git diff
```

---

## `git status` — mostrar estado

### Definición (qué hace)

`git status` muestra el estado actual del repositorio, incluyendo archivos modificados, nuevos o preparados para un commit.

---

### Ejemplo de uso (código en bloque)

```bash
git status
```

---

## `git merge` — combinar ramas

### Definición (qué hace)

`git merge` combina los cambios de una rama con otra rama.

---

### Ejemplo de uso (código en bloque)

```bash
git merge desarrollo
```

---

## `git config` — configurar Git

### Definición (qué hace)

`git config` permite configurar diferentes opciones de Git, como el nombre y correo electrónico del usuario.

---

### Ejemplo de uso (código en bloque)

```bash
git config --global user.name "Juan Pérez"
git config --global user.email "juan@ejemplo.com"
```

---

## `git add` — preparar cambios

### Definición (qué hace)

`git add` agrega archivos o cambios al área de preparación (*staging area*) para incluirlos posteriormente en un commit.

---

### Ejemplo de uso (código en bloque)

```bash
git add .
```

---

## `git log` — mostrar historial

### Definición (qué hace)

`git log` muestra el historial de commits realizados en el repositorio.

---

### Ejemplo de uso (código en bloque)

```bash
git log --oneline
```

---

## `git commit` — guardar cambios

### Definición (qué hace)

`git commit` guarda en el historial los cambios que fueron agregados previamente al área de preparación.

---

### Ejemplo de uso (código en bloque)

```bash
git commit -m "Agrega página principal"
```

---

## `git checkout` — cambiar de rama

### Definición (qué hace)

`git checkout` permite cambiar de rama o recuperar archivos de una versión determinada del repositorio.

---

### Ejemplo de uso (código en bloque)

```bash
git checkout desarrollo
```

---

## `git branch` — administrar ramas

### Definición (qué hace)

`git branch` permite crear, listar y administrar las ramas de un repositorio.

---

### Ejemplo de uso (código en bloque)

```bash
git branch desarrollo
```

---

## `git pull` — descargar e integrar cambios

### Definición (qué hace)

`git pull` descarga los cambios del repositorio remoto y los integra en la rama local actual.

---

### Ejemplo de uso (código en bloque)

```bash
git pull origin main
```

---

## `git push` — enviar cambios

### Definición (qué hace)

`git push` envía los commits de la rama local al repositorio remoto.

---

### Ejemplo de uso (código en bloque)

```bash
git push origin main
```

---

## `git fetch` — descargar cambios

### Definición (qué hace)

`git fetch` descarga información y cambios del repositorio remoto sin integrarlos automáticamente en la rama local actual.

---

### Ejemplo de uso (código en bloque)

```bash
git fetch origin
```

---

# 3. Proceso para crear un repositorio de Git desde PowerShell

Para crear un repositorio de Git desde PowerShell, se deben seguir los siguientes pasos.

## Paso 1. Crear una carpeta y entrar en ella

Primero se crea una carpeta para el proyecto utilizando `mkdir`. Después, se utiliza `cd` para entrar en la carpeta creada.

### Ejemplo de uso (código en bloque)

```powershell
mkdir MiProyecto
cd MiProyecto
```

---

## Paso 2. Inicializar el repositorio

Una vez dentro de la carpeta, se utiliza `git init` para convertirla en un repositorio de Git.

### Ejemplo de uso (código en bloque)

```powershell
git init
```

---

## Paso 3. Agregar los archivos

Después de crear o colocar los archivos del proyecto dentro de la carpeta, se utiliza `git add -A` para agregar todos los archivos y cambios al área de preparación.

### Ejemplo de uso (código en bloque)

```powershell
git add -A
```

---

## Paso 4. Realizar el primer commit

Finalmente, se realiza el primer commit utilizando `git commit -m`. El mensaje permite identificar los cambios guardados.

### Ejemplo de uso (código en bloque)

```powershell
git commit -m "mensaje inicial"
```

---

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