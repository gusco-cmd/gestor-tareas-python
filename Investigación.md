# Investigación Aplicada: Control de Versiones con Git y GitHub
**Proyecto:** Gestor de Tareas en Python  
**Equipo:** 3 Integrantes  

---

### 1. ¿Qué es Git? Explica qué realiza localmente en tu equipo al registrar los cambios en `gestor_tareas.py`.
Git es un sistema de control de versiones distribuido que rastrea el historial de cambios en los archivos de un proyecto dentro de nuestra computadora. En nuestro equipo, cuando modificamos `gestor_tareas.py` y registramos los cambios, Git no duplica el archivo completo, sino que guarda un registro interno exacto de las líneas agregadas o eliminadas. Por ejemplo, si añadimos la función de agregar tareas y el programa falla, Git nos permite regresar al estado anterior exacto del código antes de introducir dicha modificación[cite: 1].

---

### 2. ¿Qué es GitHub? Explica su rol como plataforma remota en la nube frente al software Git local.
GitHub es una plataforma basada en la nube que aloja repositorios de Git y facilita la colaboración en equipo mediante herramientas como Pull Requests e Issues[cite: 1]. Mientras que Git trabaja localmente en la terminal de cada integrante guardando versiones en su propia máquina, GitHub actúa como un servidor centralizado[cite: 1]. Por ejemplo, cuando el Estudiante 1 programa la opción de eliminar tareas en su computadora, utiliza GitHub para publicar ese código en la nube y permitir que sus otros dos compañeros lo descarguen[cite: 1].

---

### 3. ¿Cuál es la diferencia fundamental entre Git y GitHub? Presenta una analogía clara sobre cómo interactúan.
La diferencia fundamental radica en que Git es el software local que gestiona el historial de cambios, mientras que GitHub es el servicio web que almacena y permite compartir esos proyectos alojados en Git[cite: 1]. Una analogía clara es un procesador de textos e Internet: Git es como Microsoft Word en tu máquina (donde creas y guardas tus documentos), mientras que GitHub es como Google Drive (donde subes el archivo para que tu equipo lo revise juntos)[cite: 1]. En el proyecto, Git fotografía los cambios en `gestor_tareas.py` y GitHub expone esa galería al grupo[cite: 1].

---

### 4. ¿Qué es un repositorio y qué almacena exactamente? Describe qué contiene la carpeta oculta `.git`.
Un repositorio es una estructura de almacenamiento digital que contiene todos los archivos, carpetas, código fuente y el historial completo de cambios de un proyecto[cite: 1]. La carpeta oculta `.git` ubicada en la raíz almacena la base de datos interna de Git, incluyendo configuraciones, referencias a las ramas y todos los commits realizados[cite: 1]. En nuestro Gestor de Tareas, si borráramos la carpeta `.git`, el archivo `gestor_tareas.py` seguiría existiendo, pero perderíamos todo el historial de versiones y la conexión con GitHub[cite: 1].

---

### 5. ¿Qué es un commit y por qué se le compara con una "fotografía del estado del proyecto"? Detalla qué metadatos contiene.
Un commit es un registro intencional, atómico y verificado que guarda un instante preciso del estado de los archivos del proyecto, funcionando como una "fotografía" a la que se puede regresar en cualquier momento[cite: 1]. Cada commit guarda metadatos esenciales: un hash identificador único, el nombre del autor, el correo electrónico, la fecha y hora exacta, y un mensaje descriptivo[cite: 1]. Por ejemplo, al validar la entrada de un ID, el commit registra que el Estudiante 3 modificó 8 líneas el lunes a las 4:00 PM con el mensaje "Validar que el ID ingresado sea numérico"[cite: 1].

---

### 6. ¿Qué es una rama (branch) y para qué se utiliza al trabajar en equipo? Ejemplifica trabajo simultáneo sin interferencias.
Una rama es una línea de desarrollo independiente que permite aislar cambios y nuevas funcionalidades sin alterar el código estable de la rama principal (`main`)[cite: 1]. Permite que varias personas programen simultáneamente sin estorbarse[cite: 1]. Por ejemplo, el Estudiante 3 puede trabajar en la rama `feature/buscar-tarea` creando la función de búsqueda por palabra clave, mientras el Estudiante 1 modifica `feature/eliminar-tarea` en su máquina; ambos avanzan al mismo tiempo sin que los errores de sintaxis temporales de uno afecten al otro[cite: 1].

---

### 7. ¿Qué representa la rama `main` en este proyecto? Explica por qué debe contener únicamente código estable y probado.
La rama `main` representa la línea de código oficial, limpia y terminada de la aplicación que está lista para ser ejecutada[cite: 1]. Debe contener únicamente código funcional y probado para evitar que errores en desarrollo bloqueen el trabajo de los demás integrantes[cite: 1]. En el Gestor de Tareas, si alguien sube directamente a `main` un menú con un bucle infinito, romperá el proyecto para todo el grupo; por ello, los cambios solo entran a `main` tras ser aprobados mediante una revisión de código[cite: 1].

---

### 8. ¿Qué hace exactamente el comando `push`? Explica hacia dónde viajan los commits locales y cómo cambian la vista de GitHub.
El comando `git push` transfiere los commits registrados localmente en una rama de nuestra computadora hacia el repositorio remoto alojado en los servidores de GitHub[cite: 1]. Al ejecutarlo, las "fotografías" guardadas en la terminal viajan a través de Internet e integran los cambios a la plataforma en la nube[cite: 1]. Por ejemplo, cuando el Estudiante 2 completa la Opción 1 y ejecuta `git push -u origin feature/agregar-tarea`, la rama y su historial aparecen publicados inmediatamente en la página web de GitHub[cite: 1].

---

### 9. ¿Qué hace exactamente el comando `pull`? Explica la diferencia entre un commit existente en GitHub y tenerlo localmente.
El comando `git pull` descarga los nuevos commits disponibles en el repositorio remoto de GitHub y los combina (*merge*) automáticamente en la rama activa de nuestra computadora[cite: 1]. La diferencia es que un commit en GitHub existe solo en la nube y no afecta la ejecución de nuestros archivos locales hasta que es descargado[cite: 1]. Por ejemplo, si el Estudiante 1 aprueba en GitHub la función de buscar tareas, el Estudiante 2 no podrá probar dicha función en su consola hasta que ejecute `git pull origin main` en su terminal[cite: 1].

---

### 10. ¿Qué es un Issue en GitHub? Explica por qué se utiliza como una tarea técnica planificada y no solo para errores.
Un Issue en GitHub es una herramienta de gestión de proyectos utilizada para planificar, asignar y dar seguimiento al trabajo, abarcando desde nuevas funcionalidades hasta tareas de documentación y corrección de fallas[cite: 1]. No es solo para errores, sino para estructurar el desarrollo[cite: 1]. En nuestro proyecto, el Issue #2 se titula `[Feature] Registro de tareas con ID autoincremental`, donde asignamos al Estudiante 2 la responsabilidad y establecemos los criterios de aceptación que debe cumplir antes de empezar a escribir código[cite: 1].

---

### 11. ¿Qué es un Pull Request (PR)? Explica su función como espacio de diálogo y validación técnica antes del merge.
Un Pull Request (PR) es una solicitud formal en GitHub para integrar los cambios de una rama de trabajo hacia la rama principal (`main`)[cite: 1]. Funciona como una sala de control de calidad y diálogo donde el equipo revisa el código antes de fusionarlo[cite: 1]. Por ejemplo, al finalizar la función de marcar tareas completadas, el Estudiante 3 abre un PR adjuntando la salida de la consola; el Estudiante 1 revisa que las variables estén bien nombradas y aprueba la solicitud para realizar el merge[cite: 1].

---

### 12. ¿Qué significa hacer un Merge? Explica qué sucede con los historiales de dos ramas al integrarse.
Hacer un *Merge* es la operación de combinar el historial de commits y las líneas de código de dos ramas distintas en una sola[cite: 1]. Al realizarse, Git une los cambios de la rama de característica con la rama destino generando un commit de integración[cite: 1]. En el Gestor de Tareas, al hacer merge de la rama `feature/listar-tareas` hacia `main`, el código escrito para imprimir la lista formateada pasa a formar parte oficial del script principal `gestor_tareas.py`[cite: 1].

---

### 13. ¿Qué es un conflicto de Git y por qué ocurre? Describe una situación técnica de conflicto.
Un conflicto de Git es una interrupción del proceso de integración que ocurre cuando dos personas modifican exactamente las mismas líneas de un archivo de manera incompatible en ramas diferentes, impidiendo que Git decida automáticamente qué versión conservar[cite: 1]. Por ejemplo, si el Estudiante A cambia el título del menú a `"=== GESTOR CLÁSICO ==="` y el Estudiante B cambia esas mismas líneas a `"*** SISTEMA DE TAREAS ***"`, al fusionar ambas ramas a `main`, Git solicitará que el equipo edite el archivo manualmente para resolver la discrepancia[cite: 1].

---

### 14. ¿Qué es un Code Review y qué responsabilidades éticas y técnicas tiene el revisor?
El Code Review es la evaluación técnica que hace un compañero de equipo sobre el código propuesto en un Pull Request antes de su aprobación[cite: 1]. Técnicamente, el revisor debe verificar que el programa se ejecute sin excepciones, cumpla con las restricciones (sin POO ni librerías externas) y satisfaga los criterios del Issue[cite: 1]. Éticamente, debe ofrecer críticas constructivas, respetuosas y enfocadas en mejorar el Gestor de Tareas, garantizando la calidad del proyecto sin desvalorizar el trabajo del autor[cite: 1].

---

### 15. ¿Qué función cumple el archivo `README.md` en la raíz de un repositorio?
El archivo `README.md` es la portada e instructivo principal de un repositorio, redactado en formato Markdown para ofrecer una visión clara de la aplicación a usuarios, colaboradores y docentes[cite: 1]. Su función es detallar qué hace el sistema, cómo instalarlo, cómo ejecutarlo y quiénes lo desarrollaron[cite: 1]. En nuestro caso, el `README.md` incluye las instrucciones para ejecutar `gestor_tareas.py`, la tabla de responsabilidades de los 3 integrantes, los enlaces a los Pull Requests y la bitácora del conflicto de Git[cite: 1].

---

### 16. ¿Por qué son indispensables los mensajes de commit descriptivos? Da un ejemplo con un mal mensaje.
Los mensajes descriptivos son indispensables para mantener un historial auditable y comprensible, permitiendo entender qué problema resuelve cada commit sin tener que leer todo el código[cite: 1]. Los mensajes vagos dificultan detectar el origen de un fallo[cite: 1]. Por ejemplo, si la opción de eliminar tareas arroja un error y el historial muestra un commit que dice `"arreglos"`, el equipo perderá tiempo adivinando qué se cambió; en cambio, un mensaje como `"Agregar bloque try-except para validar entrada numerica en menu"` identifica la solución de inmediato[cite: 1].