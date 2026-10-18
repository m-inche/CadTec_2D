# CadTec 2D - Web Engine Pro (Privado)

Repositorio de ingeniería y desarrollo para el motor CAD 2D basado en navegador, optimizado para trazados técnicos, gestión topográfica de áreas/perímetro, metrados de construcción y control por capas.

---

## 🔒 Clasificación de Seguridad
* **Estado del Repositorio:** Privado (Acceso restringido exclusivamente al propietario y colaboradores autorizados).
* **Uso Previsto:** Desarrollo personal, metrados de campo en baja tensión y validación de diseños topográficos.

---

## 🚀 Características Principales del Sistema

1. **Motor de Dibujo Geométrico en Canvas (HTML5):**
   * Herramientas de dibujo vectorial: Líneas, Rectángulos, Círculos, Arcos y Polilíneas.
   * Modificaciones precisas: Sistema de Recorte (*Trim* tipo AutoCAD), desplazamiento de elementos (*Move*) y copias (*Copy*).
   * Asistencias de precisión CAD: O-SNAP (imán de puntos), guías polares y restricciones ortogonales (Ortho).

2. **Gestión Profesional de Capas (Layers):**
   * Soporte multi-capa avanzado (capacidad para administrar 7 o más capas de forma simultánea).
   * Control independiente de visibilidad (`👁️`), bloqueo de seguridad (`🔒`), nombres personalizados y paletas de colores por capa.

3. **Topografía y Metrados Automáticos:**
   * Detección automática de polígonos cerrados y caras planares.
   * Cálculo en tiempo real de áreas ($m^2$) y perímetros ($m$).
   * **Módulo de Descuento de Vereda:** Inserción y cálculo automatizado de deducciones superficiales para elementos urbanos (postes de concreto/fierro, tapas de agua/desagüe, muretes y pozos a tierra).

4. **Configuración de Textos y Anotaciones:**
   * Inserción de notas técnicas directamente en el plano.
   * Personalización de tipografías, tamaño de fuente, opacidad, colores de relleno/contorno y factor de estiramiento (*tracking*).

5. **Interoperabilidad y Exportación de Alta Calidad:**
   * **Persistencia JSON:** Guardado y carga completa de proyectos incluyendo la estructura y estados de las capas.
   * **Exportación Vectorial (SVG):** Generación de planos limpios compatibles con software CAD de escritorio.
   * **Captura de Imagen (PNG Alta Resolución):** Función optimizada con `html2canvas` (`scale: 3` y suavizado avanzado) para evitar pérdida de detalles en los trazos finos.

---

## 🛠️ Especificaciones Técnicas

* **Estructura:** Aplicación web de archivo único (*Single-File Architecture*), autónoma y ligera.
* **Librerías Externas (Vía CDN):**
  * *Tailwind CSS* (Diseño de interfaz y paneles).
  * *FontAwesome* (Iconografía técnica).
  * *Html2Canvas* (Motor de captura gráfica de alta fidelidad).
* **Compatibilidad:** Navegadores web modernos de escritorio (Chrome, Edge, Firefox, Safari).

---

## 📋 Historial de Cambios y Optimizaciones Recientes

* **Persistencia de Capas:** Corrección en el motor de lectura/escritura JSON para garantizar que al cargar un archivo guardado se restauren todas las capas creadas sin pérdida de información.
* **Mejora Gráfica en Capturas:** Escalado y filtrado de alta resolución en la función `exportImagePNG()` para preservar la nitidez de cotas, textos y geometrías.

---
*Documentación interna confidencial — CadTec 2D Engine.*
