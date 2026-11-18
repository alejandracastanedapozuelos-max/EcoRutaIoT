# Instructivo de Uso — EcoRutaIoT

**Plataforma SaaS de Smart City · Telecomunicaciones de Nueva Generación**
Reciclaje Inteligente con IoT para Guatemala
**Por:** Leslie Castañeda — 06144094 · Lester Mota — 23005621

---

## ¿Qué es EcoRutaIoT?

EcoRutaIoT es una plataforma web interactiva que presenta un **Social Business Model Canvas de 12 bloques** para un proyecto de reciclaje inteligente con sensores IoT en contenedores urbanos. No es una plantilla estática: es un **dashboard ejecutivo** donde puedes explorar métricas, simular escenarios de escalamiento, filtrar bloques, inspeccionar riesgos y exportar el análisis completo.

Toda la aplicación vive en un **único archivo** (`index.html`) con HTML + CSS + JavaScript Vanilla — sin frameworks, sin dependencias externas, lista para abrir en cualquier navegador o publicar en GitHub Pages.

---

## Mapa de la Página

La página tiene **9 apartados** en flujo vertical. La barra de navegación superior (sticky) te permite saltar entre ellos:

| # | Apartado | ID | Para qué sirve |
|---|---|---|---|
| 1 | Navbar | — | Navegación rápida + exportar resumen |
| 2 | Hero | — | Presentación + autoría + KPIs de impacto |
| 3 | Dashboard Ejecutivo | `#dashboard` | 8 KPIs + insignia de factibilidad |
| 4 | Bill of Materials | `#bom` | Inventario del prototipo (Q 800) |
| 5 | Eco Ruta Financiera | `#ruta` | Carretera visual de recuperación de inversión |
| 6 | Comparador Antes vs. Después | — | Transformación operativa |
| 7 | Canvas de 12 Bloques | `#canvas` | Modelo de negocio + madurez + props de valor |
| 8 | Inteligencia Estratégica | `#inteligencia` | Análisis por bloque + ODS + simulador |
| 9 | Footer | — | Enlaces, alineación ODS, paleta institucional |

---

## 1. Navbar (barra superior)

**Qué hace:** Se mantiene fija al hacer scroll (sticky) con efecto glassmorphism.

- **Logo EcoRutaIoT** — identidad de la plataforma
- **Enlaces:** Dashboard · Prototipo · Eco Ruta Financiera · Canvas · Inteligencia · Simulador
- **Botón "Exportar Resumen"** — descarga un archivo de texto (`EcoRutaIoT_Guatemala.txt`) con los 12 bloques, sus riesgos, oportunidades, impacto e indicadores. Útil para entregas o correos.

---

## 2. Hero (portada)

**Qué hace:** Presenta el proyecto en una frase e impacta visualmente.

- **Badge verde:** `GreenTech · Telecomunicaciones de Nueva Generación · IoT · ESG · Guatemala`
- **Título:** "Reciclaje Inteligente para Ciudades Sostenibles"
- **Párrafo:** Descripción del prototipo (3 contenedores, BOM de Q 800, escalable)
- **Autoría:** `Por: Leslie Castañeda — 06144094 · Lester Mota — 23005621`
- **2 botones CTA** con iconos SVG:
  - **Ver impacto del Canvas** → salta a la sección 7
  - **Explorar métricas** → salta a la sección 3
- **4 tags de impacto rápido:** CO₂, material, sensores, ROI

---

## 3. Dashboard Ejecutivo — KPIs (#dashboard)

**Qué hace:** Muestra los **8 indicadores clave** del proyecto en tarjetas con hover, tooltips y animación de entrada.

| KPI | Valor | Significado |
|---|---|---|
| CO₂ Reducido | 1,2 t/año | Emisiones evitadas por rutas optimizadas (prototipo campus) |
| Material Recuperado | 2,4 t/año | Toneladas desviadas de relleno sanitario |
| Sensores Instalados | 3 | Sensores HC-SR04 en el prototipo |
| Optimización de Rutas | 84 % | Reducción de km recorridos en vacío |
| Gestores Ambientales | 3 | Gestores universitarios del prototipo |
| Break Even | 3 meses | Tiempo para recuperar la inversión |
| ROI | 350 % | Retorno sobre inversión a 12 meses |
| Ganancia Proyectada | Q 2,800 | Ganancia neta del prototipo |

**Interacción:** Pasa el cursor sobre cada tarjeta → muestra un tooltip explicativo + se eleva con animación.

Debajo de los KPIs está la **Insignia de Factibilidad**:
> Proyecto Económicamente Viable · ROI 350% · Recuperación 3 meses · Ganancia Q 2,800 · Impacto 2,4 t recuperadas

---

## 4. Bill of Materials del Prototipo (#bom)

**Qué hace:** Detalla **todo lo que necesitas armar el prototipo físico** y su costo en Quetzales.

### Tarjeta 1 — Materiales Principales (Q 585)

| Componente | Cant. | Unitario | Subtotal |
|---|---|---|---|
| Basurero plástico 20–30 cm | 3 | Q 25 | Q 75 |
| Arduino UNO R4 WiFi | 1 | Q 350 | Q 350 |
| Sensor ultrasónico HC-SR04 | 3 | Q 20 | Q 60 |
| Protoboard 830 puntos | 1 | Q 30 | Q 30 |
| Cables Dupont macho-macho | 1 | Q 15 | Q 15 |
| Cables Dupont macho-hembra | 1 | Q 15 | Q 15 |
| Cable USB-C | 1 | Q 12 | Q 12 |
| Fuente USB 5 V | 1 | Q 20 | Q 20 |
| Cables adicionales 50 cm–1 m | 1 | Q 8 | Q 8 |

### Tarjeta 2 — Indicadores Visuales (Q 13,50)

| Componente | Cant. | Unitario | Subtotal |
|---|---|---|---|
| LED verde | 3 | Q 1 | Q 3 |
| LED amarillo | 3 | Q 1 | Q 3 |
| LED rojo | 3 | Q 1 | Q 3 |
| Resistencia 220 Ω | 9 | Q 0,50 | Q 4,50 |

### Resumen ejecutivo

- **Inversión total hardware:** Q ≈ 600
- **+ 25% contingencia** (filamentos, soldaduras, impresión 3D)
- **Inversión con margen:** Q 800
- **Costo hardware/contenedor:** Q ≈ 200
- **Costo all-in/contenedor:** ~Q 267

**Para qué te sirve:** Justifica la inversión ante un jurado o profesor mostrando que cada Quetzal está asignado a un componente real.

---

## 5. Eco Ruta Financiera (#ruta)

**Qué hace:** Visualiza el **recorrido de recuperación de inversión** como una carretera horizontal con 6 estaciones interactivas.

```
Inicio → Instalación IoT → Optimización → Rutas Inteligentes → Equilibrio → Ganancia
```

| Estación | Datos |
|---|---|
| 1 · Inicio | Inversión Inicial — Q 800 (prototipo de 3 contenedores) |
| 2 · Despliegue | Instalación IoT — 3 sensores HC-SR04 — Mes 1 |
| 3 · Operación | Optimización — Ahorro 25% |
| 4 · Escala | Rutas Inteligentes — Campus universitario — 84% eficiencia |
| 5 · Equilibrio | Punto de Equilibrio — Mes 3 |
| 6 · Retorno | Ganancia — ROI 350% — Q 2,800 |

**Interacción:** Hover sobre cada estación → la tarjeta se agranda y muestra información detallada. Un punto luminoso viaja por la carretera en animación continua.

---

## 6. Comparador Antes vs. Después

**Qué hace:** Contraste visual entre la recolección municipal tradicional y la gestión con IoT.

| Antes | Después |
|---|---|
| Rutas fijas e ineficientes | Sensores IoT en tiempo real |
| Sin monitoreo de llenado | Monitoreo continuo de nivel |
| Contenedores desbordados | Alertas automáticas anticipadas |
| Alto consumo de combustible | Menor combustible y emisiones |
| Sin trazabilidad de material | Datos ESG municipales |

**Para qué te sirve:** El jurado entiende en 5 segundos el valor diferencial del proyecto.

---

## 7. Canvas de 12 Bloques (#canvas)

**Qué hace:** Es el **corazón de la plataforma** — un Social Business Model Canvas con 12 bloques organizados en 3 niveles.

### Controles superiores

- **Filtro por nivel:** Vista Completa (12) · Impacto Social (4) · Modelo de Negocio (6) · Finanzas (2)
- **Buscador:** Escribe "Arduino", "SaaS", "empleo"… y los bloques coincidentes se resaltan, los demás se atenúan
- **Exportar** — descarga el resumen en .txt
- **Restablecer** — revierte el canvas a su estado inicial (doble clic para confirmar)

### Los 12 bloques

**Nivel 1 — Impacto Social (4 bloques)**

| # | Bloque | Icono | Qué contiene |
|---|---|---|---|
| 01 | Problema Social | 🚨 | Desbordamiento de residuos y precariedad operativa |
| 02 | Beneficiarios | 👥 | Gestores ambientales, municipios, comunidades |
| 03 | Impacto Social | ❤️ | Empleo verde digno + eficiencia ambiental medible |
| 04 | ODS Alineados | 🌍 | 5 ODS: 8, 9, 11, 12, 13 |

**Nivel 2 — Modelo de Negocio (6 bloques)**

| # | Bloque | Icono | Qué contiene |
|---|---|---|---|
| 05 | Socios Clave | 🤝 | Municipalidades, cooperativas, compradores |
| 06 | Actividades Clave | ⚙️ | Instalación IoT, calibración, soporte |
| 07 | Recursos Clave | 📡 | Arduino + HC-SR04 + Wi-Fi + plataforma |
| 08 | Propuesta de Valor | ✨ | Reciclaje inteligente con empleo digno |
| 09 | Relación | 💬 | Soporte técnico + reportes automáticos |
| 10 | Canales | 🚀 | Venta B2G + plataforma web + portal móvil |

**Nivel 3 — Finanzas (2 bloques)**

| # | Bloque | Icono | Qué contiene |
|---|---|---|---|
| 11 | Estructura de Costos | 💳 | CAPEX Q 800 + OPEX mínimo (USB 5V) |
| 12 | Fuentes de Ingreso | 💰 | Venta + leasing + SaaS + comisión |

**Interacción:** Clic en cualquier bloque → se selecciona (borde verde/azul) y el **Centro de Inteligencia Estratégica** (sección 8) se actualiza con sus riesgos, oportunidades, impacto, madurez e indicadores específicos.

### Propuestas de Valor (debajo del canvas)

6 tags: ✨ Reciclaje Inteligente · 📡 IoT Tiempo Real · 🚛 Optimización · ♻️ Economía Circular · 💰 Rentabilidad · 🏆 Empleo Verde

### Indicador de Madurez

Barra animada al **72 %** con 5 etapas del ciclo de vida:
- ✅ Idea · ✅ Diseño · ✅ Prototipo · 🟡 Piloto · ⚪ Escalamiento

---

## 8. Centro de Inteligencia Estratégica (#inteligencia)

**Qué hace:** Es el **panel de análisis dinámico**. Se actualiza automáticamente al seleccionar un bloque del canvas.

### Panel izquierdo — Inteligencia del bloque seleccionado

Muestra 4 categorías de análisis + indicadores:

| Categoría | Qué muestra |
|---|---|
| ⚠️ Riesgos | 3 riesgos específicos del bloque + tags |
| 💡 Oportunidades | 3 oportunidades + tags |
| ❤️ Impacto | 3 impactos esperados + tags |
| 📈 Madurez | Estado de validación + tags |
| Indicadores Clave | 2 KPIs numéricos del bloque |

- **Botón "Marcar como validado"** — toggle para marcar/desmarcar el bloque como validado (cambia el pill de estado en el canvas)

### Panel derecho — ODS + Simulador

**Explorador ODS:** 5 píldoras clicables (ODS 8, 9, 11, 12, 13). Al clicar, la tarjeta inferior muestra el título y descripción del ODS seleccionado.

**Simulador de escala:**
- **Slider "Contenedores con sensor IoT"** — arrastra de 3 a 300 para simular escalamiento
- **Selector "Esquema de ingresos"** — Híbrido / SaaS / Venta directa
- **4 tiles en tiempo real:**
  - Gestores integrados (1 gestor / 5 nodos)
  - Material recuperado (t/mes)
  - Cobertura de costos (según esquema)
  - Hardware base (kits Arduino + HC-SR04)

**Para qué te sirve:** Demuestra que el prototipo de Q 800 escala a pilotos municipales de 300 contenedores con proyección realista.

---

## 9. Footer

**Qué hace:** Cierre institucional con enlaces y metadata.

- Descripción + instituciones aliadas (MAGA, MARN, MCP)
- Enlaces a todas las secciones
- Alineación ODS (8, 9, 11, 12, 13)
- Paleta institucional y nota técnica
- Moneda: Quetzal (Q) · Tipo de cambio referencial: 1 USD ≈ 7.8 Q

---
