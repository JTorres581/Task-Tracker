https://github.com/JTorres581/Task-Tracker


### README - **Task Tracker CLI**

---

#### **Descripción del Proyecto**
**Task Tracker CLI** es una aplicación de línea de comandos diseñada para gestionar tareas de manera sencilla. Permite agregar, actualizar, eliminar y cambiar el estado de tareas, almacenándolas en un archivo JSON. Es una herramienta ligera y práctica que no requiere librerías externas.

---

#### **Características Principales**
- **Agregar tareas**: Permite registrar tareas con un título.
- **Actualizar tareas**: Modifica el título de una tarea existente.
- **Eliminar tareas**: Elimina una tarea específica por su número.
- **Marcar estado de tareas**: Cambia el estado de una tarea a **pendiente**, **en progreso** o **completada**.
- **Listar tareas**:
  - Todas las tareas.
  - Filtrar por estado: **pendiente**, **en progreso** o **completada**.

---

#### **Requisitos del Sistema**
- Python 3.x instalado.
- Sistema operativo con soporte para comandos en terminal (Windows, macOS, Linux).

---

#### **Instalación**
1. **Clona el repositorio o descarga el archivo `task_tracker.py`.**
   ```bash
   git clone https://github.com/JTorres581/Task-Tracker
   cd <directorio_del_proyecto>
   ```
2. **Ejecuta el script desde la terminal.**
   ```bash
   python task_tracker.py
   ```

---

#### **Uso**
La aplicación utiliza comandos en la terminal para realizar las diferentes acciones.

##### **1. Agregar una tarea**
```bash
python task_tracker.py agregar "<título de la tarea>"
```
**Ejemplo**:
```bash
python task_tracker.py agregar "Comprar alimentos"
```

##### **2. Listar tareas**
- **Todas las tareas**:
  ```bash
  python task_tracker.py listar
  ```
- **Tareas por estado**:
  ```bash
  python task_tracker.py listar <estado>
  ```
  **Estados válidos**:
  - `pendiente`
  - `en progreso`
  - `completada`

**Ejemplo**:
```bash
python task_tracker.py listar pendiente
```

##### **3. Actualizar una tarea**
```bash
python task_tracker.py actualizar <número_tarea> "<nuevo título>"
```
**Ejemplo**:
```bash
python task_tracker.py actualizar 1 "Comprar frutas y verduras"
```

##### **4. Eliminar una tarea**
```bash
python task_tracker.py eliminar <número_tarea>
```
**Ejemplo**:
```bash
python task_tracker.py eliminar 2
```

##### **5. Cambiar el estado de una tarea**
```bash
python task_tracker.py marcar <número_tarea> <estado>
```
**Estados válidos**:
- `pendiente`
- `en progreso`
- `completada`

**Ejemplo**:
```bash
python task_tracker.py marcar 3 completada
```

---

#### **Almacenamiento**
- Las tareas se guardan en un archivo llamado `tareas.json` ubicado en el mismo directorio del script.
- Este archivo se crea automáticamente si no existe.

---

#### **Manejo de Errores**
- El programa verifica que los índices de las tareas sean válidos.
- Valida los estados permitidos al usar el comando `marcar`.
- Muestra mensajes claros cuando faltan argumentos en los comandos.

---

#### **Contribuciones**
Si deseas contribuir, puedes:
1. Realizar un fork del repositorio.
2. Implementar tus cambios o mejoras.
3. Enviar un pull request.

---

#### **Licencia**
Este proyecto está bajo la licencia MIT. ¡Siéntete libre de usarlo y mejorarlo! 😊

--- 

Para cualquier consulta, no dudes en preguntar. ¡Gracias por usar **Task Tracker CLI**! 🚀