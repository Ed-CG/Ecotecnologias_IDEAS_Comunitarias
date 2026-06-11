# Prompts Handoff de Extracción Bibliográfica y Web

## Para Generación de 8 Documentos Markdown (Fases 1-5)

**Objetivo General:** Extraer información de 98_Bibliografia_PDFs + búsqueda web complementaria para generar 8 documentos Markdown estructurados según criterios del archivo 001_Handoff_Investigación.

**Instrucciones Globales para el LLM:**

- Rol: Redactor técnico experto en ingeniería sanitaria, ecotecnologías y gestión del agua
- Formato: Markdown puro para Obsidian
- Tono: Objetivo, descriptivo, universal (SIN reflexiones personales)
- Regla de Universalidad: OMITE contextos geográficos específicos (ciudades, países) → abstrae a valor técnico puro
- Diferenciación: NUNCA generalices → nombra tecnologías exactas
- Formato: Viñetas simples (PROHÍBIDO listas anidadas profundas)
- Salida: ÚNICAMENTE código Markdown (sin introducción conversacional)

---

# FASE 1: EL PROBLEMA, CONTEXTO Y ACEPTACIÓN SOCIAL

## DOCUMENTO 1: Definición y Clasificación de Aguas Grises

**Prompt Handoff:**

```
Actúa como redactor técnico. Procesa los siguientes PDFs para generar un documento 
Markdown sobre DEFINICIÓN Y CLASIFICACIÓN DE AGUAS GRISES.

PDFs a consultar (Fuentes OBLIGATORIAS):
1. giz_grey_water_recycling_and_reuse_2011.pdf
2. Diagnóstico_participativo_Oaxaca.pdf (contexto de definiciones locales)

Estructura Estricta:

## 1. Definición Técnica
Genera párrafos que definan aguas grises versus aguas negras versus aguas blancas. 
Incluye volúmenes típicos de generación per cápita (L/persona/día).
Especifica: ¿cuáles son las fuentes (lavadora, cocina, ducha, baño)?

## 2. Diferenciación por Origen y Contaminantes
- Tabla Markdown: Tipo de agua | Fuentes | Contaminantes principales | Posibilidades de reúso
- Sé específico: no digas "grasas" sino "ácidos grasos libres, ésteres, colesterol"
- Incluye: DQO, DBO, SST esperados (rango) para cada tipo

## 3. Impacto de No Tratamiento
Describe (sin mencionar países específicos):
- Impacto en acuíferos y recarga
- Impacto en suelos (salinización, sodificación)
- Riesgo sanitario (patógenos, coliformes)
- Ciclo del vector Aedes aegypti

## 4. Justificación Técnica de Tratamiento Descentralizado
- Por qué es viable tratar en origen (aguas grises)
- Potencial de recuperación en áreas urbanas, periurbanas y rurales

Entrega ÚNICAMENTE el Markdown resultante (sin explicaciones adicionales).
```

---

## DOCUMENTO 2: Análisis Regulatorio México (CON BÚSQUEDA WEB)

**Prompt Handoff:**

```
Actúa como redactor técnico. Genera un documento Markdown sobre 
ANÁLISIS REGULATORIO Y NORMATIVO PARA MÉXICO.

PDFs a consultar (Fuentes PARCIALES):
1. Diagnóstico_participativo_Oaxaca.pdf (menciona CONAGUA 2016, 2018)
2. Tesis_construcción_biojardinera.pdf (referencia a registros oficiales)

BÚSQUEDA WEB REQUERIDA:
- Normativas CONAGUA 2024-2025 sobre reúso de aguas grises
- Regulaciones PROFEPA sobre descarga de aguas tratadas
- NOMs aplicables: NOM-001-SEMARNAT (descargas en cuerpos receptores), 
  NOM-002-SEMARNAT (reúso en riego agrícola)
- Requisitos para permisos de operación (CONAGUA) por estado
- Estándares de calidad de agua para reúso no-potable

Estructura Estricta:

## 1. Marco Regulatorio Federal
- CONAGUA: autoridades competentes, permisos requeridos
- PROFEPA: autorización ambiental, descargas permitidas
- SEMARNAT: NOMs y estándares aplicables

## 2. Normas Mexicanas Específicas (NOMs)
- Tabla: Norma | Aplicabilidad | Parámetro de control | Límite máximo
- Ejemplo: NOM-001-SEMARNAT: DQO máx 150 mg/L, DBO máx 30 mg/L, SST máx 50 mg/L
- Incluye NOMs para reúso en riego (NOM-002), contacto humano, industria

## 3. Procedimiento de Permisos por Entidad
- Pasos generales: diagnóstico → solicitud → evaluación → autorización
- Documentación requerida mínima
- Tiempos estimados (rangos)

## 4. Comparación: Estándares Mexicanos vs Internacionales
- Tabla: Parámetro | Estándar México | Estándar Sudamérica | Estándar OMS
- Análisis: ¿México es más/menos estricto?

## 5. Riesgos de Incumplimiento
- Sanciones PROFEPA
- Clausura de operaciones
- Pasivos ambientales

Entrega ÚNICAMENTE el Markdown resultante.
```

---

# FASE 2: ESTADO DEL ARTE Y CASOS REALES

## DOCUMENTO 3: Contaminantes Emergentes (CON BÚSQUEDA WEB)

**Prompt Handoff:**

```
Actúa como redactor técnico especializado en contaminantes emergentes en aguas grises.
Genera un documento Markdown sobre CONTAMINANTES EMERGENTES EN AGUAS GRISES.

PDFs a consultar (Fuentes LIMITADAS):
1. GSTFJETgreywater.pdf (menciona pH, metales)
2. Cualquier PDF que mencione "contaminantes" o "parámetros"

BÚSQUEDA WEB REQUERIDA (CRÍTICA):
- Presencia de fármacos (antibióticos, hormonas, antiinflamatorios) en aguas grises
- Microplásticos: fuentes (cosméticos, ropa sintética), concentraciones reportadas
- PFAS (per- y polifluoroalcanos): fuentes, riesgos de bioacumulación
- Nanopartículas de plata en cosméticos y ropa
- Capacidad de biofiltros convencionales para remover estos contaminantes
- Post-tratamiento recomendado (carbón activado, luz UV, ozonización)
- Legislación emergente (UE, USA, México) sobre estos contaminantes

Estructura Estricta:

## 1. Definición de Contaminantes Emergentes
Explica: qué son, por qué NO están en legislación tradicional, por qué importan

## 2. Tipología y Fuentes en Aguas Grises
- Fármacos: tipos, fuentes de entrada, concentraciones típicas (ng/L a µg/L)
- Microplásticos: tamaño (µm), tipo (primarios vs secundarios), fuentes (cosméticos, ropa)
- PFAS: compuestos específicos, aplicaciones, persistencia
- Otros: nanopartículas, aditivos, interferentes endócrinos

## 3. Riesgos para Salud y Ambiente
- Bioacumulación en suelos y plantas
- Impacto en recarga de acuíferos
- Riesgos a largo plazo (estudios emergentes)

## 4. Capacidad de Biofiltros Actuales
- Remoción de fármacos: % típicos reportados
- Remoción de microplásticos: mecanismos (sedimentación, tamizado)
- Remoción de PFAS: ¿se pueden remover con tecnología actual?
- Tabla: Contaminante | Mecanismo de remoción | Eficiencia (%) | Limitaciones

## 5. Opciones de Post-Tratamiento
- Carbón activado: especificaciones, vida útil
- Luz UV: dosis requerida
- Ozonización: eficiencia
- Combinaciones efectivas

Entrega ÚNICAMENTE el Markdown resultante.
```

---

## DOCUMENTO 4: Análisis de Fracasos Documentados (CON BÚSQUEDA WEB)

**Prompt Handoff:**

```
Actúa como redactor técnico. Genera un documento Markdown sobre 
ANÁLISIS DE FRACASOS Y LECCIONES APRENDIDAS EN IMPLEMENTACIÓN.

PDFs a consultar (Fuentes MUY LIMITADAS):
1. Cualquier PDF que mencione "problemas", "fallas", "limitaciones"
2. Revisar anexos y discusiones críticas

BÚSQUEDA WEB REQUERIDA (CRÍTICA):
- Reportes ONG sobre proyectos de biojardineras/biofiltros ABANDONADOS
- Causas de fracaso: técnicas vs sociales vs económicas
- Casos documentados en Latinoamérica (Centro/Sudamérica) 
  donde sistemas fueron descontinuados
- Lecciones de proyectos fallidos en tecnologías descentralizadas
- Por qué la adopción social falló en algunos casos

Estructura Estricta:

## 1. Tipología de Fracasos
Agrupa fracasos en categorías:
- Fracasos Técnicos: diseño inadecuado, materiales inapropiados, insuficiente TRH
- Fracasos de O&M: colmatación, acumulación de grasas, falta de mantenimiento
- Fracasos Económicos: costos operativos no sostenibles, falta de financiamiento
- Fracasos de Adopción Social: rechazo comunitario, desconocimiento, responsabilidad difusa

## 2. Casos Documentados
Para cada caso (sin mencionar ubicación específica):
- Tipo de sistema implementado
- Año de implementación
- Duración operativa antes de abandono
- Causa raíz de fracaso
- Costo no recuperado
- Lecciones técnicas aprendidas

## 3. Errores de Diseño Más Comunes
- Tabla: Error de diseño | Síntomas de falla | Cómo prevenirlo | Ejemplo normativo

## 4. Errores de Operación Más Comunes
- Falta de capacitación
- Responsabilidad institucional poco clara
- Falta de repuestos o insumos de mantenimiento
- Monitoreo insuficiente

## 5. Recomendaciones Preventivas
- Checklist: criterios que DEBE cumplir un proyecto para evitar fracaso
- Indicadores de riesgo de abandono

Entrega ÚNICAMENTE el Markdown resultante.
```

---

# FASE 3: PRINCIPIOS HIDRÁULICOS Y PRETRATAMIENTO

## DOCUMENTO 5: Impacto de Lluvia Extrema y Sequía

**Prompt Handoff:**

```
Actúa como redactor técnico especializado en hidrología e impacto climático.
Genera un documento Markdown sobre IMPACTO DE LLUVIA EXTREMA, SEQUÍA Y VARIABILIDAD CLIMÁTICA.

PDFs a consultar (Fuentes PARCIALES):
1. Biojardineras_Costa_Rica.pdf (menciona cambio climático, sequía 2016)
2. La_Ecotecnología_México.pdf (contexto)
3. medio_libro_tratamiento_Wetlands.pdf (hidrología)

BÚSQUEDA WEB REQUERIDA:
- Proyecciones de cambio climático para Latinoamérica (precipitación, sequía)
- Datos de eventos extremos históricos (lluvia máxima, duración de sequías)
- Impacto de eventos extremos en sistemas descentralizados de tratamiento

Estructura Estricta:

## 1. Variabilidad Climática Regional
Describe (sin mencionar país específico):
- Patrones de precipitación: estaciones secas y lluviosas
- Duración típica de sequías
- Intensidad máxima registrada de lluvia
- Tendencias de cambio climático (aumento/disminución de precipitación)

## 2. Impacto de Lluvia Extrema en Biofiltros
- Desbordamiento: caudal máximo que un sistema típico puede recibir
- Saturación del sustrato: tiempo de recuperación
- Riesgo de afloramiento de efluentes sin tratar
- Soluciones de diseño: canales de desborde, cámaras de amortiguación

## 3. Impacto de Sequía en Biofiltros
- Reducción de aporte de agua: efecto en biopelículas
- Deshidratación del sustrato: recuperación post-sequía
- Variabilidad en eficiencia de remoción
- Tabla: Duración sequía (días) | Impacto esperado en eficiencia | Recuperación (días)

## 4. Adaptación de Diseño a Variabilidad
- Dimensionamiento para máxima lluvia: cálculo de caudal pico
- Diseño de contingencia para sequías prolongadas
- Mecanismos de retención de humedad
- Sistemas híbridos (almacenamiento + tratamiento)

## 5. Monitoreo Preventivo
- Indicadores de alerta para evento extremo
- Protocolo de operación durante lluvia extrema
- Protocolo de operación durante sequía

Entrega ÚNICAMENTE el Markdown resultante.
```

---

# FASE 4: DIMENSIONAMIENTO, MEDIOS FILTRANTES Y MODELADO

## DOCUMENTO 6: Documentación del Modelo Scilab

**Prompt Handoff:**

```
Actúa como redactor técnico especializado en modelado matemático.
Genera un documento Markdown sobre MODELO MATEMÁTICO SCILAB PARA BIOFILTROS.

PDFs a consultar (Fuentes ESPECÍFICAS):
1. articulo-modelizacion-integral-de-una-biojardinera.pdf (CRÍTICO)

BÚSQUEDA WEB REQUERIDA:
- Tutorial Scilab: cómo ejecutar scripts
- Interpretación de variables de estado en modelos de biofiltros
- Herramientas open-source alternativas para modelado hidráulico

Estructura Estricta:

## 1. Descripción Conceptual del Modelo
Explica en lenguaje técnico (sin ecuaciones aún):
- ¿Qué simula el modelo?
- ¿Cuáles son las zonas principales (aeróbica, anaeróbica, transición)?
- ¿Qué procesos bioquímicos captura?
- ¿Cuáles son sus limitaciones?

## 2. Ecuaciones Diferenciales Fundamentales
- Presenta ecuaciones en formato Markdown (usando notación clara)
- Balance de masa general
- Cinética de degradación aeróbica vs anaeróbica
- Variables de estado clave (concentración de sustrato, biomasa, oxígeno disuelto)

## 3. Parámetros del Modelo
Tabla Markdown:
| Parámetro | Símbolo | Unidad | Rango típico | Definición |
|-----------|---------|--------|---------------|-----------|
| Velocidad máxima degradación | µm | 1/día | 0.15-0.25 | ... |

## 4. Datos de Entrada Requeridos
- Caudal de entrada (L/d)
- Concentración de DQO, DBO, SST, nutrientes
- Temperatura (°C)
- Especificaciones del biofiltro (área, profundidad, tipo sustrato)

## 5. Datos de Salida Generados
- Concentración de salida (DQO, DBO, SST, nutrientes)
- Perfil de oxígeno disuelto vs profundidad
- Eficiencia de remoción (%)
- Predicción de colmatación

## 6. Instrucciones de Uso Básicas
- Cómo instalar Scilab (open-source)
- Cómo cargar el script
- Cómo cambiar parámetros de entrada
- Cómo interpretar gráficas de salida

## 7. Ejemplos de Simulación
- Caso 1: Biofiltro pequeño (5 m²) con entrada de 100 L/d
- Caso 2: Biofiltro mediano (20 m²) con entrada de 500 L/d
- Comparación: cómo varía eficiencia con caudal

## 8. Limitaciones y Validez del Modelo
- Supuestos del modelo (mezcla perfecta, estado quasi-estacionario, etc.)
- Validación experimental con datos reales
- Cuándo es válido usar este modelo y cuándo no

Entrega ÚNICAMENTE el Markdown resultante.
```

---

# FASE 5: PROTOTIPADO, CONSTRUCCIÓN Y MANUALES

## DOCUMENTO 7: Presupuesto Detallado por Región

**Prompt Handoff:**

```
Actúa como redactor técnico especializado en costos de proyectos.
Genera un documento Markdown sobre PRESUPUESTO DETALLADO DE IMPLEMENTACIÓN.

PDFs a consultar (Fuentes ESPECÍFICAS):
1. Tesis_construcción_biojardinera.pdf (Tabla 24: presupuesto Ecuador)
2. Biojardineras_Costa_Rica.pdf (Tabla 1: costos modelo)

Estructura Estricta:

## 1. Metodología de Costing
Explica:
- Cómo se estimaron costos
- Escalas consideradas (pequeña 5m², mediana 20m², grande 50m²)
- Año base y tasa de inflación asumida
- Variabilidad por región (Costa Rica, Ecuador, México)

## 2. Presupuesto por Escala (en USD)
Para CADA escala (pequeña, mediana, grande):

### Escala Pequeña (5 m² aprox, 4-5 personas)

#### 2.1 Materiales de Construcción
Tabla Markdown:
| Ítem | Cantidad | Unidad | Costo unitario (USD) | Costo total |
|------|----------|--------|----------------------|-------------|
| Geomembrana HDPE | 50 | m² | 1.50 | 75 |
| Grava (tamaño 2-4 cm) | 5 | m³ | 25 | 125 |
| Arena (tamaño 0.5-2 mm) | 3 | m³ | 20 | 60 |
| Madera/marcos | 8 | unidad | 10 | 80 |

#### 2.2 Mano de Obra
| Tarea | Horas | Costo/hora (USD) | Costo total |
|------|-------|------------------|-------------|
| Excavación y preparación | 16 | 8 | 128 |
| Instalación geomembrana | 8 | 12 | 96 |
| Llenado de capas | 12 | 10 | 120 |
| Instalación tuberías | 6 | 15 | 90 |

#### 2.3 Servicios Técnicos
- Diseño y supervisión: $300-500
- Muestreo inicial (agua bruta vs tratada): $100-200

#### 2.4 Subtotal Escala Pequeña: $1,200-2,000

### Escala Mediana (20 m² aprox, 15-20 personas)
[Repetir estructura con cantidades escaladas]
Subtotal: $3,500-6,000

### Escala Grande (50 m² aprox, 40-50 personas)
[Repetir estructura con cantidades escaladas]
Subtotal: $8,000-15,000

## 3. Análisis de Costos por Componente
Tabla resumen:
| Componente | % del costo total | Rango (USD) |
|-----------|-----------------|-------------|
| Materiales | 45-55% | $800-3,000 |
| Mano de obra | 35-45% | $600-2,500 |
| Servicios técnicos | 5-10% | $200-500 |

## 4. Variabilidad por Región
Tabla: Región | Factor de ajuste | Justificación
- Nota: Costos originales de Centro/Sudamérica; aplicar factor para México

## 5. Opciones de Financiamiento
- Fondos propios (pago en efectivo)
- Crédito de bancos de desarrollo (tasa, plazo)
- Subsidios gubernamentales (CONAGUA, estados)
- Esquemas de pago: mensual, anual

## 6. Costo de Ciclo de Vida (10 años)
Tabla:
| Ítem | Año 1 | Años 2-10 (anual) | Total 10 años |
|-----|-------|------------------|---------------|
| Inversión inicial | $1,500 | - | $1,500 |
| O&M (electricidad, mantenimiento) | $0 | $50/año | $450 |
| Reemplazo de sustrato (año 5-7) | - | - | $300 |
| Monitoreo (laboratorio) | $100 | $50/año | $550 |
| **TOTAL** | | | **$2,800** |

## 7. Costo Unitario por m³ Tratado
Tabla: Escala | m³/año tratado | Costo ciclo de vida / m³ tratado (USD)

Entrega ÚNICAMENTE el Markdown resultante.
```

---

## DOCUMENTO 8: Guía de Construcción Detallada

**Prompt Handoff:**

```
Actúa como redactor técnico especializado en construcción.
Genera un documento Markdown sobre GUÍA DE CONSTRUCCIÓN PASO A PASO.

PDFs a consultar (Fuentes ESPECÍFICAS):
1. Manual_para_construcción_Biojardineras_ACEPESA.pdf (CRÍTICO)
2. Tesis_construcción_biojardinera.pdf (detalles adicionales)

BÚSQUEDA WEB REQUERIDA:
- Técnicas de impermeabilización con geomembrana HDPE
- Métodos de compactación de sustratos
- Estándares de pendiente y drenaje en sistemas hidráulicos pasivos

Estructura Estricta:

## 1. Pre-construcción: Verificación de Sitio

### 1.1 Evaluación del Terreno
Checklist:
- Topografía: pendiente suficiente (mínimo 2%)
- Suelo: infiltración, permeabilidad (test de permeabilidad)
- Acceso: maquinaria, transporte de materiales
- Servitudes: paso de tuberías, límites de propiedad
- Cercanía a fuentes de agua: pozo, toma, etc.

### 1.2 Dimensiones Finales
Tabla de entrada:
| Parámetro | Fórmula | Ejemplo |
|-----------|---------|---------|
| Caudal diario (L/d) | Población × 100 L/persona/día | 500 personas × 100 = 50,000 L/d |
| Área superficial mínima (m²) | Caudal (L/d) / Carga superficial (40 L/m²/d) | 50,000 / 40 = 1,250 m² |
| Profundidad efectiva (m) | 0.6-1.0 m típico | 0.8 m |
| Volumen total (m³) | Área × profundidad | 1,250 m² × 0.8 m = 1,000 m³ |

## 2. Materiales Requeridos (Desglose Completo)

### 2.1 Excavación
- Volumen de tierra a remover: [fórmula]
- Disposición de material excedente: [opciones]

### 2.2 Impermeabilización
- Geomembrana HDPE: espesor 0.75-1.5 mm
- Capa de arena de protección: 5-10 cm
- Tuberías de drenaje perimetral (PVC 2-3")

### 2.3 Capas de Sustrato (de abajo a arriba)
Tabla detallada:
| Capa | Material | Granulometría | Espesor (cm) | Volumen (m³) |
|-----|----------|---------------|-------------|-------------|
| 1 (fondo) | Grava | 4-8 mm | 10-15 | - |
| 2 | Arena | 0.5-2 mm | 15-20 | - |
| 3 | Arena/lodo | 0.1-0.5 mm | 20-30 | - |
| 4 (superficie) | Arena fina/turba | <0.1 mm | 5-10 | - |

### 2.4 Plantas Macrófitas
- Especie recomendada: [nombre científico], cantidad
- Densidad de plantación: [plantas/m²]
- Época óptima de plantación: [meses]

### 2.5 Sistemas de Entrada/Salida
- Tubería entrada: diámetro, altura de descarga
- Tubería salida: diámetro, altura de rebose
- Caja de registro (dimensiones, acceso)

## 3. Secuencia de Construcción (Paso a Paso)

### Etapa 0: Preparación (Día 1-2)
1. Limpiar y nivelar el terreno
2. Marcar límites del biofiltro (usando cordel y estacas)
3. Establecer nivel de referencia (cota 0)

### Etapa 1: Excavación (Día 3-5)
1. Excavar hasta profundidad calculada + 10 cm (holgura)
2. Compactar fondo (densidad 90% Proctor estándar)
3. Verificar pendiente: mínimo 2% hacia salida
4. Inspección: suelo sin raíces, rocas, objetos

### Etapa 2: Drenaje Perimetral (Día 6-7)
1. Colocar zanja perimetral 0.5 m de ancho, 0.3 m profundidad
2. Instalar tubería PVC 2" con perforaciones (cada 20 cm)
3. Cubrir con grava gruesa (3-5 cm) y geotextil

### Etapa 3: Impermeabilización (Día 8-10)
1. Colocar capa de arena 5 cm (amortiguación)
2. Desenrollar geomembrana HDPE (cuidado con roturas)
3. Anclar bordes: 30-40 cm sobre nivel máximo de agua
4. Revisar: sin arrugas, sin daños
5. Uniones: soldadura o pegamento específico para HDPE

### Etapa 4: Llenado de Capas (Día 11-15)
**Capa 1 (Grava gruesa, 10-15 cm):**
1. Extender grava gruesa (4-8 mm) uniformemente
2. Verificar nivel con cinta métrica (cada metro)

**Capa 2 (Arena media, 15-20 cm):**
1. Humedecer arena antes de colocar (facilita compactación)
2. Extender y compactar ligeramente (evitar ruptura de geomembrana)
3. Nivelación: diferencia máxima 2 cm

**Capa 3 (Arena fina, 20-30 cm):**
1. Repetir proceso de capa 2
2. Esta capa es donde ocurre la mayor actividad biológica

**Capa 4 (Sustrato final, 5-10 cm):**
1. Mezcla arena fina + lodo + materia orgánica (30%)
2. Compactación mínima (mantener porosidad)

### Etapa 5: Sistema de Entrada y Salida (Día 16-17)
1. Instalar tubería entrada en caja de registro
2. Conectar salida con rebose configurable
3. Probar flujo: sin fugas, distribución uniforme

### Etapa 6: Plantación de Macrófitas (Día 18-20)
1. Previo: saturar sustrato con agua durante 24 h
2. Plantación: densidad [X] plantas/m²
3. Distribución: uniforme, respetando distancia entre plantas
4. Riego inicial: mantener humedad durante 2-3 semanas

## 4. Control de Calidad Durante Construcción

Checklist por etapa:
| Etapa | Parámetro | Especificación | Frecuencia de inspección |
|------|-----------|-----------------|------------------------|
| Excavación | Profundidad | ±5 cm tolerancia | Cada 5 m² |
| Impermeabilización | Integridad geomembrana | 0 perforaciones visibles | Después de colocación |
| Capas | Granulometría | ±10% del rango especificado | Muestreo cada capa |
| Plantación | Sobrevivencia | >90% a 30 días | Control semanal |

## 5. Cronograma Típico

| Tarea | Duración | Días calendarios |
|------|----------|-----------------|
| Preparación | 2 días | 2 |
| Excavación | 3 días | 3 |
| Drenaje | 2 días | 2 |
| Impermeabilización | 3 días | 3 |
| Capas de sustrato | 5 días | 5 |
| Entrada/Salida | 2 días | 2 |
| Plantación | 3 días | 3 |
| **TOTAL** | | **20 días** |

## 6. Herramientas Requeridas (Desglose)

### Herramientas Mayor (alquiler o compra)
- Retroexcavadora (3 días): $400
- Niveladora (2 días): $300
- Compactadora manual o vibratoria (3 días): $150

### Herramientas Mano (por operario)
- Pala, azadón, regla de nivel
- Cinta métrica (10-25 m)
- Nivel de agua
- Brújula (verificar pendientes)

## 7. Mano de Obra Requerida

| Rol | Cantidad | Duración (días) | Costo |
|-----|----------|-----------------|-------|
| Maestro constructor | 1 | 20 | $X |
| Peones | 4-6 | 20 | $X |
| Técnico verificación | 1 | 5 (intermitente) | $X |

## 8. Errores Comunes a Evitar

- Profundidad insuficiente: genera colmatación rápida
- Impermeabilización rota: pérdida de agua tratada, contaminación
- Capas invertidas: reduce eficiencia de remoción
- Pendiente negativa: estancamiento de agua
- Plantación deficiente: bajo enraizamiento
- Ausencia de caja de registro: dificulta mantenimiento

Entrega ÚNICAMENTE el Markdown resultante.
```

---

## DOCUMENTO 9: Curriculum de Capacitación Comunitaria

**Prompt Handoff:**

```
Actúa como redactor técnico especializado en capacitación y transferencia tecnológica.
Genera un documento Markdown sobre CURRICULUM DE CAPACITACIÓN COMUNITARIA.

PDFs a consultar (Fuentes ESPECÍFICAS):
1. Diagnóstico_participativo_Oaxaca.pdf (metodología de capacitación)
2. Biojardineras_Costa_Rica.pdf (estructura de módulos)
3. Transferencia_Ecotecnologías_Oaxaca.pdf (enfoque participativo)

Estructura Estricta:

## 1. Objetivo General de la Capacitación
Describe qué se espera que aprendan los participantes al final del programa

## 2. Población Objetivo
- Operadores de sistemas (responsables de O&M)
- Representantes comunitarios (gestión, autorización)
- Tomadores de decisión (alcaldías, juntas de agua)
- Técnicos de laboratorio (análisis de agua)

## 3. Módulo 1: Entendimiento del Problema Hídrico (4 horas)
Subtemas:
- Crisis del agua: escasez, contaminación, impacto en salud
- Ciclo del agua: natural vs contaminado
- ¿Por qué tratar aguas grises? Justificación técnica y económica
- Impacto local de agua sin tratar (suelos, acuíferos, salud)

Metodología: Presentación interactiva + visita a sitio con problema real

## 4. Módulo 2: Principios de Biofiltros y Tratamiento Pasivo (6 horas)
Subtemas:
- ¿Cómo funciona un biofiltro? Explicación paso a paso (físico, químico, biológico)
- Diferencia: biofiltro vs humedal vs FiME vs pozo absorbente
- Ventajas de tratamiento pasivo: sin electricidad, bajo costo, bajo riesgo
- Ciclo de vida del sistema (10+ años)

Metodología: Videos cortos + demostración con prototipo a escala + Q&A

## 5. Módulo 3: Diseño y Dimensionamiento (8 horas)
Subtemas:
- Cálculo de caudal: ¿cuánta agua genera una persona?
- Área mínima requerida: fórmulas simples (para no-ingenieros)
- Profundidad, materiales, plantas
- Especificaciones técnicas en lenguaje accesible

Metodología: Ejercicio práctico grupale para su comunidad específica

## 6. Módulo 4: Construcción, O&M e Indicadores de Funcionamiento (10 horas)
Subtemas:
- Construcción paso a paso (PRÁCTICO)
- Operación diaria: cómo monitorear el sistema
- Mantenimiento preventivo: cronograma, tareas simples
- Indicadores de problemas: color del agua, olores, vegetación
- Protocolo de comunicación: a quién reportar qué problema

Metodología: Taller constructivo (construir prototipo) + demostraciones en campo

## 7. Módulo 5: Apropiación Social e Integración Institucional (4 horas)
Subtemas:
- Responsabilidades: quién opera, quién paga, quién autoriza
- Conflictos comunes: cómo resolverlos
- Vinculación con autoridades locales (CONAGUA, salud, ambiente)
- Sostenibilidad: financiera, técnica, social

Metodología: Conversatorio facilitado + definición colaborativa de roles

## 8. Evaluación del Aprendizaje
Tabla:
| Módulo | Tipo evaluación | Criterio de aprobación |
|--------|-----------------|----------------------|
| 1 | Cuestionario | 70% respuestas correctas |
| 2 | Demostración oral | Explicar 3 principios clave |
| 3 | Ejercicio cálculo | Dimensionar correctamente 2 casos |
| 4 | Desempeño práctico | Ejecutar 5 tareas de O&M sin error |
| 5 | Participación | Definir roles y responsabilidades |

## 9. Certificación
- Diploma de "Operador Certificado de Biofiltro"
- Validez: 2 años (requiere refresco)
- Re-certificación: actualización anual

## 10. Materiales Educativos Requeridos
- Videos cortos (5-10 min cada uno): [títulos]
- Folletos en lenguaje local: [listado]
- Prototipo a escala (1:4 o 1:5): para demostración
- Manuales operativos: versión técnica + versión comunitaria
- Equipo de muestreo básico: para prácticas de laboratorio

## 11. Cronograma de Implementación
Mes 1: Módulo 1-2
Mes 2: Módulo 3 + ejercicio práctico
Mes 3: Módulo 4 + taller constructivo
Mes 4: Módulo 5 + evaluación final

## 12. Sostenibilidad de Capacitación
- Programa de "capacitadores de capacitadores" (local, multiplicador)
- Materiales disponibles en digital (bajo costo de distribución)
- Vinculación con institutos técnicos locales para formación continua

Entrega ÚNICAMENTE el Markdown resultante.
```

---

# NOTAS FINALES PARA EL LLM EXTRACTOR

1. **Cada prompt genera UN documento completo** (8 documentos en total)
2. **Sigue ESTRICTAMENTE los criterios del 001_Handoff_Investigación:**
   - Tono objetivo, universal, SIN reflexiones personales
   - OMITE contextos geográficos específicos (ciudades, países)
   - Diferenciación: NUNCA generalices
   - Prohíbe listas anidadas profundas
   - Entrega ÚNICAMENTE Markdown
3. **Búsqueda web complementaria:** Para documentos 2, 3, 4, realiza búsqueda web sobre temas específicos indicados
4. **Síntesis:** Integra información de múltiples PDFs + búsqueda web en UNA narrativa coherente
5. **Formato:** Markdown puro compatible con Obsidian
6. **Output:** Cada documento debe ser copiable directamente a Obsidian como nota individual

---

**Documentos esperados:**

1. ✅ Definición y Clasificación de Aguas Grises
2. ✅ Análisis Regulatorio México
3. ✅ Contaminantes Emergentes
4. ✅ Análisis de Fracasos Documentados
5. ✅ Impacto de Lluvia Extrema y Sequía
6. ✅ Documentación del Modelo Scilab
7. ✅ Presupuesto Detallado por Región
8. ✅ Guía de Construcción Paso a Paso
9. ✅ Curriculum de Capacitación Comunitaria
