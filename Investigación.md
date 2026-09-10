1. ¿Qué es Git?
Git es una herramienta que sirve para llevar un control de los cambios que hacemos en un proyecto. Por ejemplo, si estoy trabajando en gestor_tareas.py y agrego una función nueva, Git permite guardar ese cambio y saber qué se modificó.


2. ¿Qué es GitHub?
GitHub es una plataforma en Internet donde podemos guardar nuestros proyectos y compartirlos con otras personas.


3. ¿Cuál es la diferencia entre Git y GitHub?
La diferencia principal es que Git es la herramienta que usamos para controlar las versiones del proyecto, y subirlo al repositorio y GitHub es el lugar donde podemos guardar y compartir ese proyecto en Internet.


4. ¿Qué es un repositorio?
Un repositorio es el lugar donde está guardado el proyecto junto con su historial de cambios.
Dentro del proyecto existe una carpeta llamada .git, que normalmente está oculta. Ahí Git guarda toda la información relacionada con el historial del proyecto, como los commits, las ramas y otros datos que necesita para saber qué cambios se han hecho.


5. ¿Qué es un commit?
Un commit es como guardar una versión de los cambios que acabamos de hacer en el proyecto.
El commit también guarda información como quién hizo el cambio, cuándo lo hizo, un mensaje explicando qué se modificó y la información de los cambios realizados.


6. ¿Qué es una rama o branch?
Una rama es una forma de trabajar en una parte del proyecto sin afectar directamente el código principal.
Así se pueden trabajar al mismo tiempo sin estar modificando directamente el trabajo del otro. Después, cuando terminan, sus cambios se pueden revisar y unir al proyecto principal.


7. ¿Qué representa la rama main?
La rama main es la rama principal del proyecto. Es la versión que debería estar lista para funcionar.
Por eso no se debe estar metiendo directamente en main código que todavía estamos probando o que puede tener errores. Lo mejor es trabajar primero en otras ramas, probar los cambios y revisarlos antes de pasarlos a main.
De esta manera, main se mantiene como una versión estable del proyecto.


8. ¿Qué hace el comando push?
El comando push sirve para enviar los cambios que tengo guardados en mi computadora hacia GitHub.
Por ejemplo, si se realiza un commit donde se agrego una nueva función a gestor_tareas.py, con git push puedo subir ese commit a GitHub.
Después de hacerlo, las demás personas que tengan acceso al proyecto pueden ver esos cambios en GitHub.


9. ¿Qué hace el comando pull?
El comando pull hace prácticamente el proceso contrario. Sirve para traer a la computadora los cambios que otras personas ya subieron a GitHub.
Por ejemplo, puede que un compañero haya modificado gestor_tareas.py y haya subido sus cambios a GitHub. Se puede ver que existen en GitHub, pero eso no significa que ya estén en los archivos de la computadora.
Al hacer git pull, Git trae esos cambios y los aplica a el proyecto local. Así podemos tener la versión más actualizada del proyecto.


10. ¿Qué es un Issue?
Un Issue en GitHub es una forma de organizar el trabajo que hay que hacer en un proyecto.
También puede utilizarse para proponer una nueva función o dejar una tarea pendiente.
Por ejemplo:
"Agregar una opción para buscar tareas por nombre".
De esta forma, todos los integrantes del equipo pueden saber qué trabajo está pendiente y quién se está encargando de hacerlo.


11. ¿Qué es un Pull Request?
Un Pull Request, o PR, es una propuesta para pasar los cambios de una rama a otra, normalmente hacia main.
Lo importante es que antes de unir el código, los demás integrantes pueden revisarlo. Pueden hacer comentarios, encontrar errores o pedir algún cambio.


12. ¿Qué significa hacer un Merge?
Hacer un merge significa unir los cambios de una rama con otra.
Por ejemplo, si terminé de trabajar en la función de búsqueda y esa función está en mi rama, puedo hacer un merge para que esos cambios pasen a main.
De esta forma, el trabajo que estaba separado en una rama pasa a formar parte del proyecto principal y queda registrado en el historial.


13. ¿Qué es un conflicto de Git?
Un conflicto ocurre cuando dos personas cambian la misma parte del código de una manera diferente y Git no sabe cuál de los dos cambios debe utilizar.
Por ejemplo, si dos personas modifican la misma línea de gestor_tareas.py, una puede haber escrito una cosa y la otra algo diferente.
Git no puede decidir por sí solo cuál es la opción correcta, así que avisa que existe un conflicto y tenemos que revisar los cambios y decidir qué código debe quedar.


14. ¿Qué es un Code Review?
Un Code Review es cuando otra persona revisa el código que hemos hecho antes de que se incluya en el proyecto principal.
La idea es encontrar posibles errores, comprobar que el código funcione y ver si se puede mejorar.


15. ¿Para qué sirve el archivo README.md?
El README.md es como la presentación o guía del proyecto.
Ahí podemos explicar de qué trata el programa, cómo instalarlo, cómo ejecutarlo y cómo utilizarlo.
Por ejemplo, en nuestro proyecto podría explicar qué hace el gestor de tareas, cómo ejecutar gestor_tareas.py y qué opciones tiene el programa.
Es importante porque una persona que entra por primera vez al repositorio puede leer el README y entender rápidamente de qué trata el proyecto.


16. ¿Por qué son importantes los mensajes de commit?
Los mensajes de commit son importantes porque nos ayudan a recordar qué hicimos en cada cambio.
Un mensaje como:
"cambios"
no dice prácticamente nada. Si después aparece un error en el programa, sería difícil saber si ese commit tuvo algo que ver con el problema.
En cambio, un mensaje como:
"Corrige el borrado de tareas inexistentes"
nos da mucha más información. Al revisar el historial, podemos entender rápidamente qué se cambió y buscar más fácilmente dónde pudo aparecer un error.
Por eso es mejor escribir mensajes claros y específicos en los commits, especialmente cuando varias personas están trabajando en el mismo proyecto.