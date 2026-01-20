# 📈 Herramienta de Fijación de Precios | CDN Sercotec Temuco

![Estado del Proyecto](https://img.shields.io/badge/Estado-Activo-success)
![Tecnología](https://img.shields.io/badge/HTML5-Bootstrap_5-purple)
![Licencia](https://img.shields.io/badge/Licencia-MIT-blue)

Una aplicación web interactiva diseñada para apoyar a emprendedores y pequeñas empresas en la **gestión estratégica de precios**. Desarrollada para el Centro de Desarrollo de Negocios (CDN) Sercotec Temuco, esta herramienta permite calcular costos, márgenes y precios de venta bajo distintos escenarios de temporada.

---

## 📋 Descripción del Proyecto

Esta herramienta soluciona la complejidad de calcular el precio de venta correcto al integrar costos variables, gastos fijos prorrateados e impuestos (IVA) en una interfaz amigable. Funciona totalmente en el lado del cliente (Client-side), asegurando que los datos del usuario permanezcan privados en su dispositivo.

### 🚀 Características Principales

* **Perfiles de Negocio Predefinidos:** Ajuste automático de márgenes sugeridos según el rubro (Minimarket, Ferretería, Boutique, Restaurante).
* **Gestión de Múltiples Productos:** Sistema de pestañas para trabajar varios SKUs en una sola sesión.
* **Escenarios de Temporada:** Simulación de precios para cuatro etapas comerciales:
    * *Avance* (Lanzamiento)
    * *Temporada Normal*
    * *Liquidación*
    * *Remate*
* **Modos de Costeo Flexibles:**
    * **Individual:** Asigna fletes y gastos específicos a cada producto.
    * **Global:** Distribuye automáticamente un monto total de gastos/fletes entre todos los productos según sus unidades.
* **Cálculos en Tiempo Real:** Visualización inmediata de Costo Unitario, Precio Neto, Utilidad, IVA Débito y Descuentos Reales.
* **Exportación Profesional:** Generación de reportes en PDF listos para imprimir mediante `jspdf`.
* **Persistencia de Datos:**
    * Guardado automático en el navegador (`localStorage`).
    * Exportación e importación de proyectos en formato JSON.

---

## 🛠️ Tecnologías Utilizadas

Este proyecto es una aplicación **SPA (Single Page Application)** construida con tecnologías estándar, sin dependencias de compilación complejas.

* **Core:** HTML5, JavaScript (ES6+ Vanilla).
* **UI/UX:** [Bootstrap 5.3](https://getbootstrap.com/) y Bootstrap Icons.
* **Generación de PDF:** [jsPDF](https://github.com/parallax/jsPDF) y [jspdf-autotable](https://github.com/simonbengtsson/jsPDF-AutoTable).
* **Fuentes:** Google Fonts (Roboto).

---

## 📦 Instalación y Uso Local

Al ser una aplicación estática basada en un solo archivo (o estructura simple), no requiere instalación de dependencias vía npm ni servidores backend.

1.  **Clonar el repositorio:**
    ```bash
    git clone [https://github.com/tu-usuario/fijacion-precios-cdn.git](https://github.com/tu-usuario/fijacion-precios-cdn.git)
    ```
2.  **Ejecutar:**
    Simplemente abre el archivo `index.html` en cualquier navegador web moderno (Chrome, Firefox, Edge).

### 🌐 Despliegue Sugerido
Se recomienda alojar este proyecto en **GitHub Pages** para acceso público inmediato:
1.  Ve a `Settings` en tu repositorio.
2.  Entra a la sección `Pages`.
3.  Selecciona la rama `main` (o `master`) como fuente.
4.  ¡Listo! Tu herramienta estará online.

---

## 📖 Guía de Uso

1.  **Configuración Inicial (Panel Izquierdo):**
    * Selecciona tu *Tipo de Negocio* para cargar márgenes sugeridos.
    * Define si distribuirás los costos indirectos (fletes/gastos) de forma global o por producto.
2.  **Carga de Productos:**
    * Ingresa el *Costo de Compra* (con IVA).
    * Define las unidades compradas.
    * Si elegiste costo "Individual", ingresa los fletes y gastos extras del producto.
3.  **Análisis de Precios:**
    * La tabla mostrará automáticamente el **Precio Mínimo** (Costo + Margen + IVA).
    * Ingresa un **Precio Sugerido** (el precio que pondrás en la etiqueta) para ver el % de descuento real que estás aplicando sobre el precio de lista.
4.  **Generar Reporte:**
    * Haz clic en "Generar PDF" en la barra superior para descargar un informe detallado de tu estrategia.

---
