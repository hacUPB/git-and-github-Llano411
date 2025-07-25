[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/cyLOSpir)
# Unidad No. 1 - Git y GitHub
## Información del estudiante  
Nombre del estudiante: Alejandro Llano  
Id.:  000540191


Este repositorio contiene la estructura de un proyecto de programación básico, diseñado para demostrar la organización de archivos y la documentación de los procesos clave en el uso de **Git** y **GitHub**. El enfoque principal de este proyecto es la creación y gestión de un repositorio, abarcando desde la navegación básica en la consola hasta la sincronización de un repositorio local con uno remoto en GitHub.

Aquí encontrarás:

  * Un ejemplo de **código fuente** en Python dentro de la carpeta `src`.
  * **Documentación detallada** en la carpeta `docs` sobre comandos de consola, creación de repositorios locales y remotos, y su sincronización.
  * Archivos `.gitignore` para el **control de versiones** efectivo.
  * Imágenes de apoyo para visualizar los pasos realizados.

Este proyecto sirve como una guía práctica para entender cómo estructurar un proyecto, documentar su desarrollo y utilizar Git para el control de versiones.

-----

### Cómo clonar y ejecutar el proyecto

Para obtener una copia local de este proyecto y ejecutar el script de ejemplo, sigue estos pasos:

1.  **Clonar el repositorio:** Abre tu terminal o línea de comandos y ejecuta el siguiente comando:

    ```bash
    git clone https://github.com/tu-usuario/git-and-github-Llano411.git
    ```

    (Asegúrate de reemplazar `tu-usuario` con tu nombre de usuario de GitHub real y el enlace al repositorio clonado de la evaluación).

2.  **Navegar al directorio del proyecto:** Una vez clonado, dirígete a la carpeta raíz del proyecto:

    ```bash
    cd git-and-github-Llano411
    ```

3.  **Ejecutar el script de Python (Opcional):** Si deseas probar el script de ejemplo, asegúrate de tener Python instalado y luego ejecuta:

    ```bash
    python src/script.py
    ```

    Este script te pedirá que ingreses números para calcular su promedio.

-----

### Documentación del Proyecto

Explora los siguientes enlaces para aprender más sobre los temas cubiertos en este proyecto:
- [Uso de la consola](./docs/uso_consola.md)
- [Repositorio local](./docs/repositorio_local.md)
- [Repositorio remoto](./docs/repositorio_remoto.md)
---
# Evaluación

### **Descripción de la Actividad:**

El objetivo de esta actividad es crear y estructurar un proyecto de programación utilizando Git y GitHub. Aunque el código fuente será un componente mínimo, el enfoque estará en la organización del proyecto y la documentación de lo aprendido sobre los siguientes temas:

1. Uso de la consola para navegar entre directorios, crear directorios y archivos.
2. Creación de repositorios locales usando comandos de Git.
3. Creación de repositorio remoto en GitHub y sincronización con el repositorio local.

**Instrucciones:**

1. **Crea la estructura del proyecto:**
    - Clona el repositorio de la evaluación.
    - De ahora en adelante seguirás trabajando en tu repositorio local.
    - Ubícate en el directorio raíz llamado `prog-Eval_Template`.
    - Dentro de este directorio, crea las siguientes carpetas:
        - `src`: para almacenar el código fuente.
        - `docs`: para guardar la documentación.
        - `images`: para imágenes relacionadas con el proyecto.
2. **Código fuente:**
    - En la carpeta `src`, crea un script en Python (ej. script.py) con el siguiente código:
        
        ```python
        # Programa para calcular el promedio de una lista de números
        
        print("Bienvenido al programa de cálculo de promedios.")
        print("Ingresa números uno por uno. Escribe 'salir' para terminar.")
        
        # Lista para almacenar los números
        numeros = []
        
        while True:
            entrada = input("Ingresa un número (o escribe 'salir'): ")
            
            if entrada.lower() == 'salir':
                break  # Salir del bucle si el usuario escribe 'salir'
            
            try:
                # Convertir la entrada a número
                numero = float(entrada)
                numeros.append(numero)
            except ValueError:
                print("Por favor, ingresa un número válido.")
                continue
        
        # Verificar si hay números en la lista antes de calcular el promedio
        if len(numeros) > 0:
            promedio = sum(numeros) / len(numeros)
            print(f"El promedio de los números ingresados es: {promedio:.2f}")
        else:
            print("No ingresaste ningún número.")
        
        ```
        
    - Este código es solo un ejemplo básico para incluir un archivo funcional en el proyecto.
3. **Archivo .gitignore:**
    
    Investiga qué es un archivo `.gitignore` y cuál es su función dentro de un proyecto de programación. Crea el archivo `.gitignore` y guárdalo en a tu repositorio. Ahora, según la consulta que hiciste, escribe en él, los nombres de archivos y carpetas que quieres ignorar. Pregunta al profesor en caso de dudas.
    
4. **Documentación:**
    - Dentro de la carpeta `docs`, crea los siguientes archivos de tipo Markdown (.md):
        - `uso_consola.md`: Describe los conceptos aprendidos sobre cómo usar la consola para navegar y crear directorios y archivos. Haz un listado de los principales comandos utilizados en esta unidad.
        - `repositorio_local.md`: Explica cómo crear un repositorio local con comandos de Git.
        - `repositorio_remoto.md`: Detalla el proceso para crear un repositorio remoto en GitHub y sincronizarlo con el repositorio local.
5. **Archivo README.md:**
    - En la raíz del proyecto, encontrarás un archivo `README.md`, es este mismo que estás leyendo. Lo vas a editar y vas a incluir al inicio del archivo la siguiente información:
        - Una breve descripción del contenido de tu repositorio. Recuerda que los archivos README.md están ahí para explicarle a las personas que vean tu repositorio, de qué se trata y qué contiene.
        - Explica cuáles son los pasos necesarios para clonar y ejecutar el proyecto.
        - Crea una tabla de contenido con enlaces a los archivos Markdown de la carpeta `docs`.
6. **Uso de Git:**
    - Realiza commits para cada etapa del desarrollo (creación de carpetas, scripts, archivos Markdown, etc.). **Debes realizar mínimo 10 commits.** Los mensajes que utilices deben ser claros, con buena ortografía y con información relevante sobre el cambio que acabas de realizar.
    - Asegúrate de incluir imágenes con pantallazos de los pasos que realices cuando añadas elementos a tu repositorio y de los comandos de Git que utilices y su resultado.
    - Recuerda que los archivos son de Markdown, por lo tanto, debes utilizar los comandos correctos para que los archivos se puedan visualizar de manera correcta.
7. **Entrega:**
    - Sube los cambios en tu proyecto al repositorio remoto en GitHub.
    - Asegúrate de que toda la documentación esté completa y correctamente estructurada.
