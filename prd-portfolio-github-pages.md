# Documento de Requisitos del Producto (PRD)
## Proyecto: Portafolio Profesional (Landing Page)

### 1. Resumen Ejecutivo
El objetivo de este proyecto es diseñar y desarrollar una Landing Page estática para ser alojada en **GitHub Pages**. Este sitio web actuará como portafolio profesional, diseñado para centralizar la trayectoria y destacar capacidades técnicas. **Para la versión inicial y pruebas de UI, se utilizarán proyectos ficticios (mock data) con el fin de validar el diseño, espaciado y componentes visuales.**

---

### 2. Objetivos del Negocio y del Usuario
* **Para el Usuario:** Disponer de una plataforma rápida, minimalista y moderna que consolide la marca personal, validando primero la experiencia de usuario (UX/UI) de manera controlada.
* **Para la Audiencia:** Evaluar de forma limpia la estructura de la información, el stack tecnológico y la fluidez de navegación del sitio.

---

### 3. Stack Tecnológico Sugerido
* **Frontend:** HTML5, CSS3 (Tailwind CSS sugerido para desarrollo rápido de componentes) y JavaScript.
* **Despliegue/Hosting:** GitHub Pages.

---

### 4. Requisitos Funcionales (Estructura de la Landing Page)

El sitio constará de una sola página dividida en las siguientes secciones:
* **4.1. Sección Hero (Inicio):** Mensaje de impacto, subtexto y botones principales de acción.
* **4.2. Sección de Tecnologías / Stack:** Visualización de iconos o badges técnicos (Desarrollo, DevOps, Automatización).
* **4.3. Sección de Proyectos Destacados (Ficticios para Pruebas de UI):** *Ver detalle en la sección 4.3.1.*
* **4.4. Sección Sobre Mí / Trayectoria:** Breve biografía profesional.
* **4.5. Sección de Contacto:** Formulario básico vinculado a un servicio *form-to-email*.

#### 4.3.1. Detalle de Proyectos Ficticios para Validación de UI
Para asegurar que el diseño de las tarjetas (*cards*) sea versátil y soporte diferentes longitudes de texto, tecnologías y enlaces, se implementarán los siguientes 4 entornos de prueba:

##### Proyecto 1: Sistema de Monitoreo IoT (Enfoque: Backend & Data)
* **Título:** *OmniSense API*
* **Descripción:** API REST de alta disponibilidad diseñada para la ingesta masiva de datos provenientes de sensores en tiempo real. Incluye un pipeline de procesamiento que normaliza los datos antes de su almacenamiento, optimizando las consultas analíticas en un 40%.
* **Tecnologías (Tags):** Python, FastAPI, PostgreSQL, Redis.
* **Elementos UI a probar:** Tarjeta con descripción de longitud media y múltiples tags técnicos. Dos botones activos ("Ver Código", "Ver Demo").

##### Proyecto 2: Automatización de Infraestructura (Enfoque: DevOps & Cloud)
* **Título:** *CloudForge Orchestrator*
* **Descripción:** Herramienta de automatización basada en CLI para el despliegue rápido de entornos aislados de microservicios. Permite levantar arquitecturas complejas de desarrollo local con un solo comando, reduciendo el tiempo de configuración de entornos.
* **Tecnologías (Tags):** Docker, Bash, Linux, Podman.
* **Elementos UI a probar:** Tarjeta con textos cortos y tags orientados a infraestructura. Un solo botón activo ("Ver Código") y un botón deshabilitado/oculto ("Demo no disponible").

##### Proyecto 3: Plataforma E-learning Automatizada (Enfoque: Full Stack & CRM)
* **Título:** *Apex Learning Portal*
* **Descripción:** Sistema integral de gestión de aprendizaje enfocado en tecnología. Cuenta con un módulo de automatización que aprovisiona laboratorios prácticos en contenedores de manera dinámica para cada estudiante mediante webhooks y colas de tareas.
* **Tecnologías (Tags):** Django, JavaScript, Tailwind CSS, Celery.
* **Elementos UI a probar:** Tarjeta con descripción larga para verificar el comportamiento del contenedor de texto (*text overflow*) y la alineación vertical de los botones.

##### Proyecto 4: Pipeline de Integración Continua (Enfoque: CI/CD & Automatización)
* **Título:** *AutoShip CI Pipeline*
* **Descripción:** Configuración avanzada de flujos de trabajo automatizados para la validación de código, ejecución de pruebas unitarias y empaquetado de aplicaciones. Envía alertas dinámicas a canales de mensajería del equipo ante fallos críticos en el despliegue.
* **Tecnologías (Tags):** GitHub Actions, Node.js, Webhooks.
* **Elementos UI a probar:** Tarjeta con pocos tags pero de longitud horizontal variable para testear el comportamiento del contenedor (*flexbox/grid layout*).

---

### 5. Requisitos No Funcionales (Calidad de UI)
* **Estabilidad del Grid:** Las 4 tarjetas de los proyectos deben alinearse simétricamente en una cuadrícula (grid) que se adapte automáticamente de 1 columna (móvil) a 2 o 3 columnas (pantallas grandes).
* **Estados de los Botones:** Validación visual de los estados *Hover*, *Focus* y *Active* en los botones de "Código" y "Demo" de cada tarjeta.

---

### 6. Roadmap Actualizado (Fases)
* **Fase 1:** Maquetación HTML/CSS e inclusión del contenido de texto estático (incluyendo los 4 proyectos de prueba).
* **Fase 2:** Refinamiento visual, pruebas de diseño responsivo y comportamiento de las tarjetas con diferentes resoluciones de pantalla.
* **Fase 3:** Reemplazo de los datos ficticios por tus proyectos reales y enlaces definitivos.
* **Fase 4:** Despliegue en GitHub Pages.
