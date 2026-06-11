**Objetivo:** Comprender el problema, analizar casos de éxito y fracaso empíricos, y dominar las variables de diseño físico-químicas e hidráulicas para rediseñar un biofiltro pasivo de bajo costo.

---

## Fase 1: El Problema, el Contexto y la Aceptación Social (El "Por qué")

La ingeniería sin adopción social es infraestructura muerta. Antes de medir, debes entender el riesgo real del agua sin tratar, el impacto en los suelos y los factores que hacen que una comunidad appropie o abandone una ecotecnología.

### Temas a dominar

Diferencias entre aguas grises/negras, impacto de la salinidad, apropiación tecnológica e índices de transferencia.

### Documentos existentes a consultar (26 abstracts analizados)

* `giz_grey_water_recycling_and_reuse_2011`: Definiciones base de aguas grises, volúmenes de generación y comparación de cadenas de tratamiento.
* `Effect_of_Treated_Grey_Water_Reuse_in_Irrigation_o.pdf`: Riesgos de acumulación de salinidad y necesidad de lavado de suelos al reusar el agua.
* `LaEcotecnologiaenMexico2014.pdf`: Marco conceptual nacional sobre impacto socioeconómico y sustentabilidad verdadera.
* `Diagnóstico participativo para la transferencia de ecotecnología... Oaxaca.pdf`: Contexto local real y disposición comunitaria al saneamiento.
* `Dialnet-TransferenciaDeEcotecnologiasYSuAdopcionSocial...pdf`: Índice de Transferencia Ecotecnológica (ITE) para medir viabilidad de adopción.
* `Biojardineras_como_alternativas_para_el_tratamient SOCIAL.pdf`: Casos de integración institucional y comunitaria en Costa Rica.

### Documentos a generar (Cierre Brecha Fase 1)

**`08_Análisis_Regulatorio_México.md`** ⚠️ FALTA GENERAR
* Normativas CONAGUA, PROFEPA, NOM-* aplicables
* Permisos y trámites por entidad
* Comparación estándares locales vs internacionales
* *Prioridad:* MEDIA | *Estado:* Pendiente | *Fuente:* Búsqueda nueva (regulatoria)

---

## Fase 2: Estado del Arte y Casos Reales (Lo que ya se hizo y cómo funcionó)

Para no diseñar a ciegas, aquí analizarás evaluaciones de biofiltros y humedales ya construidos. Esto te dirá qué métricas esperar y qué fallas operativas son comunes en campo.

### Temas a dominar

Benchmarking de tecnologías, eficiencias de remoción reales (DQO, DBO, nutrientes, metales) y evaluación mediante bioindicadores. Análisis de fracasos documentados.

### Documentos existentes a consultar (26 abstracts analizados)

* `ghaitidak2013`: Revisión integral de 22 tecnologías. Argumento técnico de por qué los biofiltros son superiores a otras alternativas descentralizadas.
* `INFORMEFINALINTERCTI01-2021_VFINAL3.pdf`: Casos en Guatemala y Perú con métricas exactas de remoción de metales/nutrientes y costos por metro cuadrado (0.5 a 2 m²/persona).
* `servicio socoal UAM analsisi agua del biofiltro Xochimilco.pdf`: Evaluación real fisicoquímica (oxígeno, amonio) y biodiversidad que demuestra mejora en calidad del agua en campo.
* `REPORTFINALSESSION2023-2024.pdf`: Análisis de prototipo de biofiltro de bajo costo en zonas rurales de India, usando materiales altamente accesibles.

### Documentos a generar (Cierre Brecha Fase 2)

**`05_Contaminantes_Emergentes.md`** ⚠️ FALTA GENERAR
* Medicinas, microplásticos, PFAS en aguas grises
* Capacidad actual de biofiltros para remover estos contaminantes
* Post-tratamiento recomendado
* *Prioridad:* MEDIA | *Estado:* Pendiente | *Fuente:* Búsqueda nueva (literatura reciente)

**`06_Análisis_Fracasos_Documentados.md`** ⚠️ FALTA GENERAR
* 2-3 casos de abandono/fracaso identificados
* Análisis de por qué fallaron
* Lecciones aprendidas para prevención
* *Prioridad:* MEDIA | *Estado:* Pendiente | *Fuente:* Búsqueda nueva (entrevistas + literatura)

---

## Fase 3: Principios Hidráulicos y Pretratamiento (El "Cómo llega el agua")

La mayoría de las fallas operativas (taponamientos, desbordes) ocurren antes de que el agua llegue al sustrato. Debes dominar la gestión de sólidos, grasas y energía hidráulica. Incluye variabilidad climática.

### Temas a dominar

Trampas de grasas, filtros gruesos, disipación de energía, flujos de gravedad y pendientes. Impacto de lluvia extrema y sequía.

### Documentos existentes a consultar (26 abstracts analizados)

* `Manual de diseño para manejo de aguas grises.pdf`: Biblia para diseñar flujos por gravedad, trampas de lavadoras y riego seguro.
* `Guia diseño filtración en multiples etapas.pdf`: Sistemas FiME. Clave para diseñar cámaras de amortiguación (filtros gruesos dinámicos) previas al biofiltro.
* `medio libro tratamiento Wetlands`: Base teórica definitiva para comprender hidrología y comportamiento hidráulico en sistemas pasivos (sin bombeo).
* `IJREISS_2937_50867.pdf / Dahake et al. (2019)`: Datos sobre cómo variación de espesores (200-600mm) afecta eficiencia, aplicable a diseño robusto.

### Documentos a generar (Cierre Brecha Fase 3)

**`08_Impacto_Lluvia_Extrema_Sequia.md`** ⚠️ FALTA GENERAR
* Modelo lluvia extrema → desbordamiento → prevención
* Ciclos de sequía prolongada → capacidad de respuesta del sistema
* Adaptación a cambio climático en diseño
* *Prioridad:* MEDIA | *Estado:* Pendiente | *Fuente:* Modelización existente + datos climáticos

---

## Fase 4: Dimensionamiento, Medios Filtrantes y Modelado (El "Motor" interno)

Traducir la química y biología en variables de ingeniería. Aquí defines geometría, tiempos de retención y la interacción del agua con diversas capas de materiales filtrantes.

### Temas a dominar

Cálculos hidráulicos, tiempos de retención, variación de espesores en sustratos (arena, grava, biochar, tezontle/zeolita) y su impacto en la turbidez/DQO.

### Documentos existentes a consultar (26 abstracts analizados)

* `Guia_didactica_sobre_diseno_de_humedales_artificia.pdf`: Criterios matemáticos y de ingeniería para dimensionamiento y cálculos hidráulicos.
* `articulo-_-modelizacion-integral-de-una-biojardinera...pdf`: Modelo matemático en Scilab que ayuda a entender zonas aeróbicas/anaeróbicas e impacto de descargas súbitas (ej. lavadora).
* `IJREISS_2937_50867.pdf / Dahake, D. et al. (2019)`: Datos empíricos sobre cómo alterar alturas de capas de sustrato (200mm, 400mm, 600mm) modifica parámetros de filtración.
* `Application of horizontal series filtration...pdf`: Alternativas de medios filtrantes (zeolita, piedra pómez, carbón) por si materiales estándar no están disponibles.
* `GSTFJETgreywater.pdf`: Uso de turba y carbón para neutralizar pH en aguas residuales (estudio en Malasia).
* `biocarbono revision de filtros que usas a donde va la tecnologia.pdf`: Información vanguardista sobre filtros de biocarbón para olores y remoción avanzada.
* `sharaf2020.pdf`: Diseño compacto de una sola etapa usando carbón activado granular (GAC) para optimizar espacio.
* `1-s2.0-S2588912521000394-main.pdf`: Estudio de remoción en sistemas multicapa domésticos (TSS 94%, DQO 85%).

### Documentos a generar (Cierre Brecha Fase 4)

**`13_Herramienta_Computacional_Diseño.md`** ⚠️ FALTA GENERAR - CRÍTICO
* Interfaz usuario para cálculos automáticos de dimensionamiento
* Adaptación/mejora del modelo Scilab existente
* Generación automática de especificaciones y planos
* Validación automática contra eficiencias esperadas
* *Prioridad:* ALTA | *Estado:* Pendiente | *Fuente:* Modelo Scilab existente + interfaz de diseño

---

## Fase 5: Prototipado, Construcción y Manuales (La "Implementación")

Convirtiendo los cálculos en un sistema construible, replicable y mantenible por las usuarias. Esta es la fase CON MAYOR BRECHA actualmente (50% completitud).

### Temas a dominar

Nomenclatura, cuantificación de materiales locales, armado físico, solución de problemas (fugas) y diseño de manuales operativos amigables. Construcción fotográfica detallada.

### Documentos existentes a consultar (26 abstracts analizados)

* `Manual para la construcción y mantenimiento de Biojardineras.pdf`: Guía maestra de ACEPESA para lista de materiales, ensamblaje y pasos constructivos.
* `tesis construccion biojardinera.pdf`: Ejemplo de cómo estructurar entregables (implementación física, análisis pre/post y manual de operación).

### Documentos a generar (Cierre Brecha Fase 5 - ALTÍSIMA PRIORIDAD)

**`11_Guía_Construcción_Fotografica_Detallada.md`** ⚠️ FALTA GENERAR - ALTÍSIMA PRIORIDAD
* Paso a paso CON FOTOS/VIDEOS por cada etapa
* Herramientas necesarias y procedimientos
* Cronograma detallado (horas/días por etapa)
* Control de calidad constructiva
* *Prioridad:* **ALTÍSIMA** | *Estado:* Pendiente | *Fuente:* Manual ACEPESA + validación visual nueva

**`12_Presupuesto_Detallado_por_Región.md`** ⚠️ FALTA GENERAR - ALTA PRIORIDAD
* Costos unitarios de materiales por región (México)
* Mano de obra estimada (capacitación requerida)
* Contingencias y riesgos (+ 10-15%)
* Opciones de financiamiento
* *Prioridad:* ALTA | *Estado:* Pendiente | *Fuente:* INFORMEFINALINTERCTI + REPORT2023-2024 + presupuestos reales

**`13_Curriculum_Capacitación_Comunitaria.md`** ⚠️ FALTA GENERAR - ALTA PRIORIDAD
* Capacitación operadores (4 módulos estructurados)
* Protocolo de integración institucional
* Sistema de rotación de responsabilidades
* Seguimiento y evaluación
* *Prioridad:* ALTA | *Estado:* Pendiente | *Fuente:* LaEcotecnología + Costa Rica + Diagnóstico Oaxaca

---

## Análisis de Cobertura

| Fase | Documentos Generados | Documentos a Generar | Completitud | Prioridad Cierre |
|------|---|---|---|---|
| **1** | 6 | 1 | 85% | MEDIA |
| **2** | 4 | 2 | 65% | MEDIA |
| **3** | 4 | 1 | 80% | MEDIA |
| **4** | 8 | 1 | 88% | ALTA |
| **5** | 2 | 3 | 40% | **ALTÍSIMA** |
| **TOTAL** | **24** | **8** | **75%** | **Enfatizar Fase 5** |

---

## Notas Importantes

1. **Este documento es la guía del PIPELINE PRODUCTIVO** - mapea qué generar basado en 26 abstracts analizados
2. **Fase 5 es CRÍTICA** - hoy 40% completa, requiere 3 documentos urgentes (construcción fotográfica, presupuestos, capacitación)
3. **8 documentos nuevos cerraran brechas críticas** → elevará cobertura de 60% a 85%
4. **Después de generar estos documentos**, se aplicará la reestructuración planificada en `../PLAN_Reestructuración_Wiki_Referencia.md`
5. **Obsidian se usará como visualizador provisional** durante la generación de contenido
