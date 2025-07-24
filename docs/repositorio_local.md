## Cómo crear un repositorio Git local

Para crear un repositorio Git local, sigue estos sencillos pasos. Puedes copiar y pegar los comandos directamente en tu terminal.

### 1\. Abre tu terminal y navega a la carpeta de tu proyecto

Primero, abre tu terminal (o línea de comandos) y usa el comando `cd` para ir a la carpeta donde quieres crear tu repositorio. Por ejemplo, si tu proyecto se llama "MiProyecto" y está en tu escritorio:

```bash
cd Desktop/MiProyecto
```

**Consejo:** Si la carpeta aún no existe, puedes crearla con `mkdir MiProyecto` y luego entrar en ella.

### 2\. Inicializa el repositorio Git

Una vez dentro de la carpeta de tu proyecto, ejecuta el siguiente comando para **inicializar el repositorio Git**:

```bash
git init
```

Este comando crea una subcarpeta oculta llamada `.git` dentro de tu proyecto. Esta carpeta es esencial, ya que contiene toda la información que Git necesita para rastrear los cambios en tus archivos.

### 3\. Verifica el estado (opcional)

Puedes usar `git status` para confirmar que el repositorio se ha inicializado correctamente. Te mostrará que aún no hay commits y que no hay archivos para añadir:

```bash
git status
```
