# TRAZA//CO2 🚗💨

**TRAZA//CO2** es una aplicación web progresiva (PWA) avanzada orientada al cálculo de la huella de carbono y la valoración económica de flotas de vehículos. Permite consultar fichas técnicas en tiempo real (mediante integración con la DGT o base de datos local de respaldo), analizar emisiones bajo los estándares **TTW (Tank-to-Wheel)** y **WTW (Well-to-Wheel)**, y proyectar escenarios de retorno de inversión (**Payback**) en función de la evolución del precio del CO₂ hasta 2035.

---

## 🚀 Características Principales

* **Ficha Técnica por Matrícula:** Consulta de datos de vehículos, distintivo ambiental DGT (CERO, ECO, B, C) y verificación de exenciones RTVV. Soporta modo DEMO local y conexión a API en producción.
* **Análisis de Alcance (TTW / WTW):** Alterna fácilmente entre el impacto directo en escape y el ciclo completo de los combustibles (incluyendo extracción y refinado).
* **Comparador de Flotas:** Simulación antes y después de la transición energética con métricas de ahorro en toneladas de CO₂ y equivalencia en árboles.
* **Valoración Económica y Payback Dinámico:** Modelado financiero que cruza el coste de emisiones con tres escenarios de precios del carbono (Pesimista 40 €/t, Actual ETS 73 €/t y Objetivo UE 2030 a 150 €/t).
* **Exportación de Informes:** Generación de informes ejecutivos en formato **PDF** y exportación de datos tabulares a **CSV**.
* **Capacidad PWA:** Instalable en dispositivos móviles y de escritorio con soporte de funcionamiento offline básico mediante *Service Worker*.

---

## 🛠️ Tecnologías Utilizadas

* **HTML5 & CSS3** (Diseño responsivo con variables CSS y animaciones fluidas).
* **JavaScript Vanilla (ES6+)** para la lógica de negocio y gestión de eventos.
* **Chart.js (v4.4.0)** para la renderización de gráficos interactivos.
* **jsPDF & html2canvas** para la exportación y renderizado de informes en PDF.

---

## 📂 Estructura del Proyecto

```text
traza-co2/
├── index.html          # Interfaz principal y lógica de la aplicación
├── manifest.json       # Manifiesto de la aplicación web progresiva (PWA)
├── sw.js               # Service Worker para caché y soporte offline
└── icons/
    ├── icon-192.png    # Icono de la app (192x192 px)
    └── icon-512.png    # Icono de la app (512x512 px)