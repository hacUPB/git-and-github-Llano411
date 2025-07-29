## Crear un repositorio remoto en GitHub y sincronizarlo con el repositorio local


### 1\. Crear un Repositorio en GitHub (Remoto)

1.  **Inicia sesión en GitHub:** Ve a [github.com](https://github.com/) e inicia sesión en tu cuenta.
2.  **Crea un nuevo repositorio:** En la esquina superior derecha, haz clic en el signo **'+'** y selecciona **"New repository"**.
3.  **Configura el repositorio:**
      * **Repository name:** Elige un nombre descriptivo para tu repositorio (ej. `mi-primer-proyecto`).
      * **Description (opcional):** Añade una breve descripción.
      * **Public/Private:** Selecciona si quieres que sea público (visible para todos) o privado (solo para ti y quienes compartas).
      * **NO marques "Add a README file", "Add .gitignore" ni "Choose a license" en este paso**, ya que sincronizaremos con un repositorio local existente.
4.  **Crea el repositorio:** Haz clic en el botón verde **"Create repository"**.
5.  **Copia la URL remota:** Una vez creado, se te mostrará una página con instrucciones. Busca la URL del repositorio (generalmente bajo "Quick setup" o "…or push an existing repository from the command line"). Será algo como `https://github.com/tu-usuario/mi-primer-proyecto.git`. **Cópiala.**

### 2\. Sincronizar con tu Repositorio Local

Abre tu **terminal o línea de comandos** y navega hasta la carpeta raíz de tu proyecto local (donde tienes tu repositorio Git ya inicializado, es decir, donde se encuentra la carpeta `.git` oculta).

Si aún no has inicializado un repositorio local, hazlo primero:

```bash
cd /ruta/a/tu/proyecto
git init
```

Ahora, sigue estos pasos para sincronizar:

1.  **Conectar tu repositorio local con el remoto:**
    Reemplaza `<URL_DEL_REPOSITORIO_REMOTO>` con la URL que copiaste de GitHub.

    ```bash
    git remote add origin <URL_DEL_REPOSITORIO_REMOTO>
    ```

    *Ejemplo:*

    ```bash
    git remote add origin https://github.com/tu-usuario/mi-primer-proyecto.git
    ```

2.  **Verificar la conexión (opcional pero recomendado):**

    ```bash
    git remote -v
    ```

    Deberías ver `origin` listado con las URLs de fetch y push.

3.  **Empujar los cambios de tu rama principal (o `main`) al repositorio remoto:**
    Si tu rama principal se llama `master`, usa `git push -u origin master`. Si es `main` (que es el nombre predeterminado en los repositorios nuevos de GitHub), usa `git push -u origin main`. La opción `-u` (o `--set-upstream`) establece la rama remota como la rama de seguimiento predeterminada para tu rama local, lo que facilita futuros `git push` y `git pull`.

    ```bash
    git push -u origin main
    ```



¡Listo\! Tu repositorio local ahora está sincronizado con el remoto en GitHub. Cada vez que hagas cambios y los confirmes (`git commit`), podrás subirlos a GitHub con un simple `git push`.
