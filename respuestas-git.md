1. ¿Qué diferencia existe entre `git add` y `git commit`?

git add prepara los cambios realizados en el directorio de trabajo pasándolos al área de preparación (staging area), indicando qué archivos formarán parte de la próxima versión. Por su parte, git commit toma esos archivos preparados y crea una instantánea permanente en el historial del repositorio local con un mensaje descriptivo.

2. ¿Qué hace `git push` y por qué puede ser rechazado?

git push sube los commits locales de tu repositorio hacia un repositorio remoto (como GitHub o GitLab). Puede ser rechazado principalmente porque el repositorio remoto contiene cambios que tú no tienes en local, lo que provocaría una sobrescritura de datos si no se sincronizan ambos historiales previamente.

3. ¿En qué se diferencian `git fetch` y `git pull`?

git fetch descarga los cambios y metadatos del repositorio remoto a tu repositorio local sin modificar tu rama de trabajo actual, permitiéndote revisar los cambios antes de aplicarlos. En cambio, git pull realiza un fetch y automáticamente intenta fusionar (merge) esos cambios remotos en tu rama activa en un solo paso.

4. ¿Qué significa `origin/main`?

origin/main es una referencia local que representa el estado actual de la rama principal (main) en el servidor remoto (origin). Permite conocer en qué punto se encontraba el remoto la última vez que se estableció comunicación con él mediante comandos como fetch o push.

5. ¿Qué muestra `git status` antes y después de `git add`?

Antes de git add, git status muestra los archivos modificados o nuevos en color rojo, indicando que están sin seguimiento o sin preparar (unstaged). Después de ejecutar git add, esos mismos archivos aparecen en color verde en el área de preparación, listos para ser guardados en el siguiente commit.

6. ¿Para qué sirve `git diff --cached`?

git diff --cached sirve para visualizar las diferencias exactas entre los cambios que ya has añadido al área de preparación (staging area) y el último commit realizado. Es muy útil para revisar qué es exactamente lo que vas a confirmar antes de ejecutar un commit.

7. ¿Qué indica `git log --oneline HEAD..origin/main`?

Este comando muestra una lista resumida de los commits que existen en la rama remota (origin/main) pero que todavía no están integrados en tu rama local actual (HEAD). Permite identificar con claridad el trabajo pendiente por descargar o fusionar.

8. ¿Por qué conviene realizar commits pequeños y descriptivos?

Conviene hacerlo porque facilita enormemente la lectura del historial de cambios, agiliza la revisión de código por parte de otros compañeros y permite aislar, depurar o revertir un error de forma mucho más precisa y rápida.

9. ¿Cómo resolviste el `push` rechazado y por qué no utilizaste `--force`?

El rechazo del push se resuelve descargando e integrando los cambios del remoto (mediante un pull o fetch y merge/rebase) y resolviendo posibles conflictos locales antes de volver a subir el código. No se utilizó --force porque este método sobrescribe a la fuerza el historial remoto, lo que puede borrar el trabajo de otros colaboradores y romper la integridad del proyecto.

10. ¿Qué diferencia hay entre un diagrama de clases y un diagrama de secuencia?

Un diagrama de clases es de naturaleza estática y muestra la estructura orientada a objetos del sistema, incluyendo clases, atributos, métodos y sus relaciones. En contraste, un diagrama de secuencia es dinámico y describe cómo interactúan los objetos entre sí a lo largo del tiempo mediante el intercambio de mensajes.

11. ¿Qué utilidad tienen los breakpoints durante una depuración?

Los breakpoints o puntos de interrupción sirven para pausar la ejecución de un programa en una línea de código específica. Esto permite inspeccionar en tiempo real el valor de las variables, el flujo de ejecución y el estado de la memoria para cazar errores con precisión quirúrgica.

12. ¿Por qué son importantes las pruebas antes y después de refactorizar?

Las pruebas previas aseguran que el código actual funciona correctamente y establecen una línea base de comportamiento funcional. Las pruebas posteriores confirman que la refactorización (la mejora interna del código) no ha roto ninguna funcionalidad ni introducido nuevos errores.

13. ¿En qué carpeta y ventana de IntelliJ estabas cuando se rechazó el `push`?

Esta ubicación depende enteramente del proyecto local en el que estabas trabajando; sin embargo, al ocurrir un rechazo de push en IntelliJ IDEA, el aviso suele mostrarse en la ventana inferior de notificaciones o en la pestaña dedicada a Git (Git Tool Window) dentro de la carpeta raíz del proyecto activo.
