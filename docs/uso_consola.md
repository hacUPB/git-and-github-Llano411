# Dominio de la Consola: Navegación y Gestión de Archivos

Esta unidad se centró en el dominio de la **consola de línea de comandos** para una interacción eficiente con el sistema operativo. Hemos aprendido a **navegar por el sistema de archivos**, y a **crear, manipular y eliminar directorios y archivos**. Esta metodología ha demostrado ser **altamente potente y eficiente**, superando la interfaz gráfica en operaciones complejas o repetitivas.

Un concepto clave fue la importancia del **directorio de trabajo actual** y cómo los comandos se ejecutan en relación a él. Se diferenciaron las **rutas absolutas** de las **rutas relativas**, comprendiendo la utilidad de atajos como `.` y `..`. En resumen, la capacidad de gestionar archivos y directorios directamente desde la línea de comandos es fundamental para un control eficaz y productivo del sistema.
Comandos Fundamentales para la Interacción con el Sistema de Archivos

## Comandos esenciales:

pwd: Este comando permite visualizar la ruta absoluta del directorio de trabajo actual (Print Working Directory), siendo indispensable para la orientación dentro de la jerarquía del sistema.

ls: Utilizado para listar el contenido de un directorio. Admite opciones como ls -l para obtener una lista detallada (incluyendo permisos, tamaño y fecha de modificación) y ls -a para mostrar todos los archivos, incluyendo los ocultos.

cd <directorio>: Comando empleado para cambiar el directorio de trabajo. Ejemplos incluyen cd Documentos para acceder a un subdirectorio o cd .. para ascender al directorio padre.

mkdir <nombre_directorio>: Permite la creación de uno o múltiples directorios nuevos. Se puede especificar varios nombres para una creación simultánea (mkdir dir1 dir2).

touch <nombre_archivo>: Empleado para crear archivos vacíos o actualizar la fecha de última modificación de un archivo existente.

cp <origen> <destino>: Comando para copiar archivos o directorios. Para copiar directorios de forma recursiva, se requiere la opción -r (ej. cp -r directorio_origen/ directorio_destino/).

mv <origen> <destino>: Se utiliza tanto para mover archivos o directorios a una nueva ubicación como para renombrarlos. Si el destino es un nuevo nombre en la misma ruta, el elemento es renombrado.

rm <archivo>: Comando para eliminar archivos. Se debe usar con precaución, ya que la operación es irreversible sin confirmación explícita.

rm -r <directorio>: Permite la eliminación recursiva de directorios y todo su contenido. Requiere extrema cautela debido a la naturaleza destructiva de la operación.

cat <archivo>: Utilizado para mostrar el contenido de archivos de texto directamente en la consola, facilitando una revisión rápida.

clear: Comando simple para limpiar la pantalla de la terminal, mejorando la legibilidad y organización del entorno de trabajo.
