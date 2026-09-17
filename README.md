# Práctica 2 - SEMANA 3: Desarrollo Web con Bootstrap 5 y Tailwind CSS

## 📋 Información del Proyecto
* **Tema Seleccionado:** N°6 Inmobiliaria – Propiedades, búsqueda y contacto
* **Curso / Asignatura:** Desarrollo Web / Desarrollo de Aplicaciones Web

### 👥 Integrantes
* **Janampa Jaime, Khaled Alejandro**
* **Pariona Ramos, Saúl Anibal**

---

## 🔗 Enlaces del Proyecto
* **Repositorio en GitHub:** [https://github.com/saulPariona/SEMANA3_DAW_PRACTICA2_AGUILAR](https://github.com/saulPariona/SEMANA3_DAW_PRACTICA2_AGUILAR)
* **Sitio Web Desplegado (GitHub Pages):** [https://saulpariona.github.io/SEMANA3_DAW_PRACTICA2_AGUILAR/](https://saulpariona.github.io/SEMANA3_DAW_PRACTICA2_AGUILAR/)

---

## 🚀 Descripción del Proyecto
Este proyecto consiste en la maquetación e implementación de una plataforma web inmobiliaria moderna, altamente responsive, accesible e interactiva. El desarrollo combina la estructura sintáctica y los componentes robustos de **Bootstrap 5.3.3** con la agilidad y el diseño utilitario refinado de **Tailwind CSS (Play CDN)**.

---

## ⚙️ Integración Híbrida: Bootstrap 5 + Tailwind CSS

Uno de los principales desafíos técnicos resolutivos de esta práctica fue la combinación estratégica de ambos frameworks para aprovechar lo mejor de dos mundos sin generar colisiones estéticas o estructurales:

1. **División de Responsabilidades:**
   * **Bootstrap 5:** Encargado del sistema de maquetación en grilla de 12 columnas (`container`, `row`, `col-*`), componentes de interacción compleja por JS (menú colapsable/navbar responsive) y clases sintácticas de estado de validación de formularios (`form-control`, `is-invalid`, `valid-feedback`).
   * **Tailwind CSS:** Utilizado para el acabado micro-estético, incluyendo sombras elevadas (`shadow-lg`), desenfoques de fondo (`backdrop-blur`), bordes suavizados (`rounded-xl`), tipografía fluida/balanceada (`text-balance`, `max-w-3xl`), degradados (`bg-gradient-to-r`) y animaciones interactivas al cursor (`hover:scale-105`, `transition-transform`).

2. **Resolución de Conflictos de Especificidad:**
   * Se ajustó el orden de importación en el `<head>` cargando primero las hojas de estilo base de Bootstrap y posteriormente Tailwind CSS para permitir la sobrescritura de utilidades de diseño visual.
   * En casos de conflicto en reseteos CSS (Reset/Preflight), se aplicaron clases específicas de Tailwind con modificadores de especificidad o utilidades explícitas en línea sin alterar el modelo de caja (*box-sizing*) global del Grid System de Bootstrap.

---

## 🛠️ Detalle de Pasos Implementados

### PASO 1: Configuración del Entorno Inicial
* Estructuración base en **HTML5** con idioma en español (`lang="es"`).
* Inclusión de metaetiqueta `viewport` para adaptación responsive en pantallas móviles, tablets y escritorio.
* Implementación de **Metaetiquetas SEO**: `description`, `keywords`, `author` y `robots`.
* Integración de CDNs oficiales: **Bootstrap 5.3.3** y **Tailwind CSS (Play CDN)**.

### PASO 2: Barra de Navegación Responsive Híbrida
* Construcción del componente `navbar` con las clases `navbar-expand-lg`, `collapse` y `navbar-toggler` de Bootstrap para garantizar colapso funcional en pantallas pequeñas.
* Inclusión de menú desplegable (*dropdown*) y *badges* de notificación para alertas inmobiliarias.
* Estilización avanzada con Tailwind: `shadow-lg`, `py-3` y `backdrop-blur` para un efecto translúcido de alta calidad visual.

### PASO 3: Sección Principal (Hero Section)
* Estructura con encabezado dinámico (`display-3`), texto descriptivo (`lead`) y botones de llamada a la acción (CTA) configurados con `d-flex` y `gap-3`.
* Aplicación de utilidades de Tailwind: `text-balance` para legibilidad tipográfica, `max-w-3xl` para control de ancho de lectura y fondos degradados `bg-gradient-to-r`.
* Documentación de la resolución de especificidad entre clases de tipografía de Bootstrap y utilidades de color/ancho de Tailwind.

### PASO 4: Cuadrícula de Inmuebles / Propiedades
* Maquetación mediante el Grid System de 12 columnas de Bootstrap (`container`, `row`, `col-md-4`) para respuesta adaptativa sin necesidad de media queries CSS manuales (`@media`).
* Tarjetas Inmobiliarias mejoradas con Tailwind CSS: bordes redondeados (`rounded-xl`), sombras dinámicas (`shadow-lg`) y microinteracciones fluidas al pasar el cursor (`hover:scale-105 transition-transform duration-300`).

### PASO 5: Formulario de Contacto e Interacción con Accesibilidad (WCAG)
* Diseño enfocado en pautas **WCAG 2.1 AA** garantizando un contraste visual mínimo de **4.5:1** entre texto y fondo.
* Vinculación semántica estricta entre etiquetas `<label>` e `<input>` mediante correspondencia `for` y `id`.
* Inclusión de atributos `aria-describedby` para asociar dinámicamente mensajes de error visuales y leídos por lectores de pantalla.
* Integración de validación nativa de Bootstrap (`form-control`, `is-invalid`, `valid-feedback`) en conjunto con el selector `peer` de Tailwind CSS para estilos de validación avanzados.

### PASO 6: Auditoría y Optimización (Lighthouse & WAVE)
* **Google Lighthouse:** Ejecución de pruebas de Performance, Accesibilidad, Buenas Prácticas y SEO en Chrome DevTools, alcanzando puntuaciones óptimas mediante carga diferida de scripts y optimización de metadatos.
* **WAVE Web Accessibility Evaluation Tool:** Corrección de contrastes de color, etiquetas de formulario faltantes y estructura jerárquica de encabezados (`h1`-`h6`) para asegurar cero errores críticos de accesibilidad.

---


## 🛠️ Tecnologías Utilizadas
* **HTML5** (Semántico y Accesible)
* **CSS3** (Tailwind CSS Play CDN)
* **JavaScript (ES6+)** (Bootstrap 5 Bundle JS)
* **Bootstrap 5.3.3** (Grid system, Navbar, Modales, Validación)
* **Tailwind CSS** (Utilidades de diseño, sombreado, hover, glassmorphism)
* **Git & GitHub** (Control de versiones)
* **GitHub Pages** (Despliegue continuo)
