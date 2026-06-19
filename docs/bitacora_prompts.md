# 📝 Bitácora de Desarrollo y Prompts
**Proyecto:** Sistema de Gestión para Estudio de Yoga Valentina  
**Herramientas:** Gemini / AI Studio / Claude / NotebookLM / Stitch

---

## 🔗 Enlaces del Proyecto
* **Prototipo Interactivo (Stitch):** [Ver Prototipo en Stitch](https://ai.studio/apps/ff32e7ba-21db-4656-b118-c17fb883aeb9)
* **Video Pitch (Demostración):** [Ver Video en YouTube](https://www.youtube.com/watch?v=EUoJPguwDGs)

---

## 🔍 Fase 1: Descubrimiento y Prototipado (Ideación)

### Análisis del Caso con NotebookLM
Para la fase inicial de comprensión del negocio, se utilizó NotebookLM con el objetivo de extraer la lógica del problema.

* **Prompt 1:**
  > "Analiza el caso del estudio de yoga Valentina e identifica los principales problemas operativos y oportunidades de mejora."
* **Resultado:** Se identificaron problemas relacionados con el uso de Excel para la gestión de alumnos, reservas realizadas por Instagram, errores en los cobros y falta de métricas para la toma de decisiones.

* **Prompt 2:**
  > "Genera los requerimientos funcionales para una plataforma que automatice la gestión del estudio."
* **Resultado:** Se definieron los módulos principales del sistema: Gestión de alumnos, horarios, instructores, membresías/paquetes, control de pagos, registro de asistencia y dashboard de indicadores.

* **Prompt 3:**
  > "Diseña una solución tecnológica que elimine los procesos manuales del negocio."
* **Resultado:** Se propuso una plataforma centralizada con sistema de reservas por créditos, control de asistencia, automatización de pagos y panel administrativo con métricas de negocio.

### Prototipado con Stitch
* **Prompt 1:**
  > "Genera un prototipo visual para la administración de un estudio de yoga con una interfaz moderna y profesional."
* **Resultado:** Se creó la estructura general de navegación de la aplicación y un panel administrativo orientado a la gestión del estudio.

* **Prompt 2:**
  > "Diseña las pantallas principales necesarias para operar el negocio."
* **Resultado:** Se generaron las interfaces de Dashboard General, Gestión de Horarios, Gestión de Instructores, Gestión de Membresías y Configuración del Estudio.

* **Prompt 3:**
  > "Genera los archivos base del proyecto para ser utilizados en la etapa de implementación."
* **Resultado:** Se exportaron los módulos y archivos del prototipo, los cuales sirvieron como base para el desarrollo posterior del sistema.

---

## 🛠️ Fase 2: Desarrollo Asistido por IA (Implementación)

### Arquitectura y Configuración Inicial
* **Prompt 1:**
  > "Necesito crear una aplicación web para la gestión de alumnos de yoga. ¿Cómo debería estructurar una API con FastAPI y SQLite para registrar alumnos, sus pagos y controlar la asistencia?"
* **Resultado:** Definición de la estructura de la base de datos (tablas alumnos, pagos y clases) y configuración inicial del archivo `main.py` utilizando FastAPI y SQLite.

### Integración del Frontend y Resolución de Errores (CORS / 404)
* **Prompt 2:**
  > "Estoy recibiendo un error `{"detail":"Not Found"}` al intentar desplegar mi aplicación en Render. ¿Por qué el servidor no encuentra mi archivo index.html?"
* **Resultado:** Identificación de problemas en la ruta del archivo y falta de coincidencia entre la ruta definida en `FileResponse` y la ubicación real dentro del repositorio.

* **Prompt 3:**
  > "He movido mi archivo a la raíz como sugeriste, pero sigue fallando. ¿Cómo debo organizar los archivos en GitHub para que Render los reconozca automáticamente?"
* **Resultado:** Optimización de la estructura de archivos en el repositorio raíz, eliminando carpetas redundantes y estandarizando el nombre del archivo `index.html`.

### Depuración y Despliegue en Render
* **Prompt 4:**
  > "El despliegue en Render me da 'Exited with status 1'. ¿Cómo puedo saber qué está fallando durante el despliegue?"
* **Resultado:** Revisión de logs, ajuste del *Start Command* y verificación de dependencias en `requirements.txt`.

* **Prompt 5:**
  > "Logré que la página cargue, pero en mi computadora el archivo se ve solo como 'index' y en GitHub como 'index.html'. ¿Es esto correcto?"
* **Resultado:** Configuración de visualización de extensiones en Windows y validación de la estructura del repositorio.

### Finalización y Preparación para Entrega
* **Prompt 6:**
  > "Tengo que entregar el proyecto con carpetas específicas (/docs, /db, /backend, /frontend). ¿Cómo organizo mi repositorio final y qué debería contener el script .sql?"
* **Resultado:** Organización final del repositorio y generación del script SQL de inicialización.

* **Prompt 7:**
  > "¿Cómo debería estructurar un Video Pitch de 5 minutos para explicar este proyecto de manera efectiva?"
* **Resultado:** Diseño del guion de presentación técnica y funcional del proyecto.

---

## ⚙️ Tecnologías y Herramientas Utilizadas
* **Diseño e Ideación:** NotebookLM, Stitch
* **Asistencia de IA:** Gemini / Google AI Studio
* **Backend:** FastAPI, Python, SQLite
* **Despliegue y Control de Versiones:** GitHub, Render

---

## 📈 Metodología Aplicada
Se utilizó un proceso iterativo apoyado por herramientas de IA. Primero se analizaron los problemas del negocio y se definieron los requerimientos mediante **NotebookLM**. Luego se construyó un prototipo funcional en **Stitch** y finalmente se desarrolló la aplicación utilizando generación asistida de código para backend, frontend y base de datos.
