# gestor-tareas-python
# Gestor de Tareas interactivo en Python con Control de Versiones Git y GitHub

## 1. Título del Proyecto
**Gestor de Tareas interactivo en consola (Python)**  
*Proyecto colaborativo de control de versiones con Git y GitHub.*

---

## 2. Descripción General y Objetivo
Este proyecto consiste en una aplicación de consola desarrollada en Python que permite gestionar una lista de tareas en memoria RAM durante la sesión de ejecución[cite: 1]. 

**Propósito pedagógico:** Experimentar y aplicar el flujo de trabajo colaborativo real en ingeniería de software mediante Git y GitHub[cite: 1]. Se implementa la planificación con Issues, aislamiento de funcionalidades en ramas (`feature/*`), integración mediante Pull Requests (PR), revisión de código entre pares (Code Review) y la resolución controlada de conflictos de fusión (*merge conflicts*)[cite: 1].

---

## 3. Funcionalidades del Sistema
El programa presenta un menú interactivo continuo con 6 opciones numéricas obligatorias[cite: 1]:

1. **Agregar una tarea:** Solicita la descripción de la tarea, genera un identificador (`id`) entero consecutivo automático (1, 2, 3...) y la registra con estado pendiente (`completada: False`)[cite: 1]. Rechaza descripciones vacías[cite: 1].
2. **Mostrar las tareas:** Imprime la totalidad de las tareas registradas con el formato visual `1. [Pendiente] Estudiar Python`[cite: 1]. Muestra un mensaje claro si la lista está vacía[cite: 1].
3. **Marcar una tarea como completada:** Solicita el `id` numérico de la tarea y actualiza su estado a completada si existe; de lo contrario, notifica el error sin detener el programa[cite: 1].
4. **Eliminar una tarea:** Solicita el `id` numérico y remueve la tarea del sistema manteniendo la integridad de los identificadores restantes[cite: 1].
5. **Buscar tareas:** Filtra y despliega todas las tareas cuya descripción contenga el término buscado (insensible a mayúsculas y minúsculas)[cite: 1].
6. **Salir del programa:** Muestra un mensaje de despedida y finaliza de forma limpia la ejecución del bucle principal[cite: 1].

---

## 4. Requisitos de Entorno
* **Lenguaje:** Python 3.8 o superior[cite: 1].
* **Dependencias:** Ninguna[cite: 1]. El proyecto utiliza exclusivamente la librería estándar de Python, sin paquetes externos ni bases de datos[cite: 1].

---

## 5. Instrucciones de Instalación y Ejecución

1. **Clonar el repositorio:**
   ```bash
   git clone [https://github.com/USUARIO_O_ORGANIZACION/gestor-tareas-python.git](https://github.com/USUARIO_O_ORGANIZACION/gestor-tareas-python.git)
   cd gestor-tareas-python
   ```[cite: 1]

2. **Ejecutar la aplicación:**
   ```bash
   python gestor_tareas.py