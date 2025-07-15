# 1.1. LISTA DE HISTORIAS DE USUARIO POR FUNCIONALIDAD

ANÁLISIS DE CV

1. Extracción automática de habilidades
Historia de usuario:
Como reclutador startup, quiero que el sistema extraiga automáticamente las habilidades y experiencias clave del CV, para ahorrar tiempo en el análisis inicial.
Descripción:
El sistema debe identificar habilidades técnicas y blandas directamente desde los CVs cargados, sin intervención manual.
Criterios de aceptación:

Dado que he subido uno o más CVs al sistema,
cuando el análisis se complete,
entonces debo ver un listado automático de habilidades, experiencias y competencias relevantes para cada candidato.

2. Visualización simplificada para no técnicos
Historia de usuario:
Como reclutador sin experiencia técnica, quiero una visualización clara y destacada de las competencias detectadas por IA, para tomar decisiones rápidas.
Descripción:
El sistema debe mostrar la información extraída del CV en un formato amigable y visual, sin jerga técnica.
Criterios de aceptación:

Dado que accedo al perfil de un candidato,
cuando el sistema haya procesado su CV,
entonces debo ver las competencias organizadas por categoría y resaltadas según su relevancia.

3. Alertas de coincidencia crítica
Historia de usuario:
Como founder o líder de equipo, quiero recibir alertas cuando un candidato coincida con habilidades críticas del rol, para actuar con rapidez.
Descripción:
El sistema debe notificar automáticamente cuando encuentra un perfil que cumple requisitos marcados como “críticos” en una vacante.
Criterios de aceptación:

Dado que he definido requisitos críticos para un cargo,
cuando un candidato coincida en un 100% con esos requisitos,
entonces debo recibir una alerta por correo o dentro del sistema.

4. Carga masiva y resumen automático
Historia de usuario:
Como reclutador multitarea, quiero poder cargar varios CVs a la vez y recibir resúmenes automáticos, para no perder tiempo en tareas repetitivas.
Descripción:
El sistema debe permitir la carga múltiple de archivos y procesarlos en lote generando insights por cada uno.
Criterios de aceptación:

Dado que he cargado múltiples CVs,
cuando finalice el análisis,
entonces debo ver una tabla con los resúmenes clave (habilidades, años de experiencia, nivel de afinidad).

5. Recomendaciones de carga
Historia de usuario:
Como usuario nuevo, quiero que el sistema me dé ejemplos o recomendaciones sobre cómo subir CVs para asegurar mejores resultados de análisis.
Descripción:
Se debe mostrar una guía visual o mensajes contextuales que ayuden al usuario a subir documentos en formatos óptimos.
Criterios de aceptación:

Dado que intento subir un CV,
cuando el archivo no cumpla condiciones óptimas (formato incorrecto, ilegible),
entonces el sistema debe recomendar cómo mejorarlo o mostrar ejemplos aceptables.

🤖 MATCHING INTELIGENTE
1. Ranking automático de afinidad
Historia de usuario:
Como reclutador sin equipo grande, quiero que el sistema me muestre un ranking automático de los candidatos más afines al perfil, para enfocarme en los mejores.
Descripción:
El sistema debe calcular un puntaje de afinidad para cada candidato respecto a la vacante y ordenarlos en un listado.
Criterios de aceptación:
Dado que he creado una vacante,
cuando el sistema analice los candidatos disponibles,
entonces debo ver una lista ordenada de mayor a menor afinidad.

2. Transparencia del algoritmo
Historia de usuario:
Como startup en crecimiento, quiero entender por qué el sistema sugiere ciertos candidatos, para confiar en la IA.
Descripción:
Cada resultado del ranking debe incluir una explicación textual sobre los factores que influyeron en la puntuación.
Criterios de aceptación:
Dado que reviso el ranking de afinidad,
cuando consulte un candidato,
entonces debo ver un resumen de los criterios clave que contribuyeron a su posición.

3. Filtro por afinidad
Historia de usuario:
Como reclutador, quiero filtrar candidatos por nivel de afinidad al perfil deseado, para agilizar la revisión.
Descripción:
El sistema debe permitir aplicar filtros dinámicos al listado de candidatos según su puntuación de match.
Criterios de aceptación:
Dado que estoy visualizando la lista de candidatos,
cuando seleccione un filtro de afinidad (ej. 80%+),
entonces el sistema solo debe mostrarme candidatos que cumplan esa condición.

4. Comparación entre perfiles
Historia de usuario:
Como fundador, quiero poder comparar entre candidatos similares para tomar decisiones rápidas y basadas en datos.
Descripción:
El sistema debe permitir seleccionar múltiples perfiles para mostrar diferencias y similitudes clave.
Criterios de aceptación:
Dado que selecciono dos o más candidatos,
cuando pulse “Comparar”,
entonces el sistema debe mostrar sus competencias, experiencias y afinidades lado a lado.

5. Indicador visual de coincidencia
Historia de usuario:
Como reclutador junior, quiero una guía visual de "match" que me permita ver rápidamente qué candidatos cumplen más del 80% de los requisitos.
Descripción:
El sistema debe mostrar un ícono o barra de color indicando niveles de coincidencia, sin necesidad de leer toda la ficha.
Criterios de aceptación:
Dado que veo una lista de candidatos,
cuando uno tenga más del 80% de match,
entonces debo ver un ícono verde o barra destacada que lo indique.

# 1.2. PROBLEMAS COMUNES

1. Problema: Falta de confianza en los resultados del algoritmo de IA
Contexto: El sistema realiza análisis de CV, matching, evaluación de soft skills y predicciones automáticas. Pero el usuario (sobre todo no técnico) puede desconfiar del “por qué” detrás de cada decisión del sistema.
Impacto: Reduce la adopción, genera fricción o decisiones manuales duplicadas.

Mejora sugerida:

Incluir explicaciones visuales (“IA explicable”) en cada puntuación o sugerencia.

Incorporar gráficos de afinidad, etiquetas de criterios cumplidos y “consejo de IA” en lenguaje natural (ej: “Este candidato destaca por su experiencia en startups similares”).

Opción de “ver más/menos detalles” para usuarios técnicos y no técnicos.

2. Problema: Saturación de información en las primeras etapas
Contexto: Múltiples funcionalidades como extracción de datos, matching, evaluación de soft skills y predicción de éxito se presentan juntas tras la carga del CV.
Impacto: El usuario puede sentirse abrumado por la cantidad de datos al momento de tomar decisiones.

Mejora sugerida:

Implementar una vista por etapas (“Embudo de selección”) donde la información se revela progresivamente.

Usar tarjetas por bloque: “CV Básico”, “Afinidad Técnica”, “Soft Skills”, “Predicción de Éxito”.

Añadir un modo “Focus” que muestre solo los candidatos top 5 con más potencial en base al objetivo de la vacante.

3. Problema: Poca personalización de criterios para startups
Contexto: Las startups suelen valorar atributos como adaptabilidad, velocidad de aprendizaje o compatibilidad cultural por encima de la experiencia formal.
Impacto: El sistema podría subvalorar buenos candidatos por aplicar criterios más tradicionales.

Mejora sugerida:

Permitir al reclutador o founder personalizar el “peso” de los factores de selección.

Introducir plantillas de vacantes orientadas a startups (con enfoque en cultura, soft skills y potencial).

Entrenar modelos ML específicos para perfiles de startup con datos históricos segmentados.

4. Problema: Complejidad para usuarios nuevos o con poco tiempo
Contexto: Muchas startups no tienen equipos de RRHH formales; el mismo founder o PM realiza procesos de selección.
Impacto: La curva de aprendizaje puede frenar la adopción o provocar errores en configuraciones.

Mejora sugerida:

Activar un modo asistido o “IA Coach” para acompañar paso a paso en la creación de vacantes, análisis de candidatos y entrevistas.

Agregar recomendaciones contextuales en tiempo real (ej: “Te recomendamos revisar estos 3 perfiles por su afinidad alta con tu vacante”).

Ofrecer configuraciones rápidas: “¿Prefieres priorizar experiencia, cultura o potencial?”

5. Problema: Integración técnica limitada con herramientas internas
Contexto: Aunque el sistema tiene integración con Gmail, Google Drive y Office 365, puede haber fricción si los procesos de la startup se apoyan en Slack, Notion, Trello u otras herramientas comunes.
Impacto: Información desconectada o flujos poco naturales para el usuario.

Mejora sugerida:
Incluir integraciones nativas o vía Zapier/Make con herramientas populares de startups.

Agregar Webhooks personalizables para notificaciones o tareas (ej: “cuando se apruebe un candidato, crear una tarjeta en Trello”).

Ofrecer una API simplificada con documentación accesible para desarrolladores de la startup.

# 1.3. ASPECTOS TECNICOS ASOCIADOS

1. Requisitos de IA / Procesamiento Inteligente
a. Extracción automática de datos del CV
OCR avanzado (para PDFs escaneados).

Parser de CV multiformato (PDF, DOCX, HTML).

NER (Named Entity Recognition) entrenado en dominio laboral.

Clasificación semántica de secciones del CV (educación, experiencia, habilidades).

Normalización de skills con ontologías (ej: ESCO, O*NET, o propias).

b. Matching Inteligente
Motor de scoring basado en algoritmos ML (ej: Random Forest, XGBoost o NLP embedding con BERT).

Vectorización de perfil de vacante y perfil del candidato para cálculo de similitud.

Peso ajustable por feature (habilidades técnicas, años de experiencia, industria, cultura).

Módulo de explicabilidad (SHAP/LIME o reglas generadas para visualizar decisiones).

c. Evaluación de Soft Skills
Procesamiento de lenguaje natural para análisis de tono, estilo y vocabulario en CV o respuestas a preguntas abiertas.

Modelos entrenados para predecir rasgos de personalidad (basados en Big Five, DISC u otros).

Módulo de inferencia de “fit cultural” basado en valores organizacionales ingresados por la startup.

d. Predicción de Éxito
Modelos supervisados con entrenamiento sobre base histórica (éxito/fracaso laboral).

Features como movilidad laboral, seniority, tipo de empresa anterior, ciclo de vida startup.

Output de tipo clasificación binaria o regresión (porcentaje de éxito).

Registro de variables explicativas para transparencia.

🖥️ 2. Backend (Microservicios / Arquitectura LTI)
Servicios necesarios:
CV Parsing Service: Lectura, extracción y estructuración del contenido de CV.

Candidate Scoring Service: Calcula afinidad general por vacante.

Soft Skills Analysis Service: Ejecuta inferencias sobre atributos blandos.

Success Prediction Service: Evalúa probabilidad de éxito y genera recomendación.

Profile Comparison API: Compara múltiples candidatos entre sí.

Explainability Service: Expone el razonamiento detrás de los puntajes.

Infraestructura y APIs:
Node.js (según arquitectura LTI) para orquestar servicios.

Redis o MongoDB como caché de resultados IA (para evitar reprocesar).

PostgreSQL para almacenar perfiles estructurados.

RabbitMQ/Kafka para colas en análisis masivo o por lotes.

💻 3. Frontend (Web + Móvil)
Funcionalidades requeridas:
Componente de carga masiva de CVs con barra de progreso y validación de formato.

Panel de visualización de afinidad (ranking, etiquetas, barras de color).

Comparador visual entre candidatos.

Vista paso a paso (por secciones) del perfil enriquecido.

Dashboard para personalizar pesos de evaluación y prioridades (matching, cultura, etc.).

Módulo de configuración de alertas y criterios críticos.

🔗 4. Integraciones externas
Google Drive API para subir CVs desde el Drive.

Gmail API para enviar alertas de coincidencia crítica.

Slack Webhook (opcional para startups) para recibir notificaciones de IA.

Soporte para conectarse a un CRM de RRHH o Notion vía Zapier / Webhooks REST.

📈 5. Escalabilidad y Experiencia
Procesamiento en lote con tareas asíncronas.

UI/UX optimizado para simplificar visualizaciones complejas (dashboard simple con tooltips, ayuda en línea, modo asistente).

Control de versiones de modelos IA para trazabilidad.

Logs auditables de análisis y decisiones automáticas (para trazabilidad y control).


# 2.1 BACKLOG DEL PRODUCTO

| Historia de Usuario                         | Impacto / Valor | Urgencia | Complejidad Técnica | Riesgos / Dependencias                              |
| ------------------------------------------- | --------------- | -------- | ------------------- | --------------------------------------------------- |
| **Análisis de CV**                          |                 |          |                     |                                                     |
| Extracción automática de habilidades        | Alto            | Alta     | Alta                | Depende de NER, OCR, normalización de skills        |
| Visualización simplificada para no técnicos | Medio-Alto      | Alta     | Media               | Depende de resultados del parser y UI amigable      |
| Alertas de coincidencia crítica             | Alto            | Alta     | Media               | Requiere notificaciones + validación de reglas      |
| Carga masiva y resumen automático           | Alto            | Media    | Alta                | Procesamiento por lotes, arquitectura asíncrona     |
| Recomendaciones de carga                    | Medio           | Baja     | Media               | Afectado por validación de formatos y UX contextual |


| Matching Inteligente | | | | |
| Ranking automático de afinidad | Alto | Alta | Alta | Depende del motor de scoring y vectorización |
| Transparencia del algoritmo | Alto | Alta | Alta | Requiere módulo explainable AI (SHAP/LIME) |
| Filtro por afinidad | Medio | Media | Media | Requiere front dinámico + query optimizado |
| Comparación entre perfiles | Alto | Media | Alta | Requiere diseño de comparador + API de perfiles |
| Indicador visual de coincidencia | Medio-Alto | Alta | Media | Relacionado con resultado de matching |


# 3.1. TICKETS DE TRABAJO

| Nº  | Ticket Técnico                                                                 | Historia de Usuario Asociada                      | Prioridad | Tipo           | Criterios de Aceptación                                                                                               | Esfuerzo (pts) |
|-----|----------------------------------------------------------------------------------|---------------------------------------------------|-----------|----------------|------------------------------------------------------------------------------------------------------------------------|----------------|
| T1  | Crear parser de CV multiformato (PDF, DOCX, HTML) con OCR                       | Extracción automática de habilidades              | Alta      | Backend/IA     | Dado que he subido uno o más CVs, cuando el sistema procese los documentos, entonces debe leerlos y estructurarlos.   | 8              |
| T2  | Implementar modelo NER para extracción de entidades laborales                   | Extracción automática de habilidades              | Alta      | IA/ML          | Dado que se extrae texto del CV, cuando el modelo analice, entonces debe identificar skills, roles y experiencias.     | 13             |
| T3  | Construir microservicio `cv-parsing-service` y exponer vía API REST             | Extracción automática de habilidades              | Alta      | Backend        | Dado que se activa una carga de CV, cuando se llama al servicio, entonces debe devolver datos estructurados.          | 5              |
| T4  | Diseñar UI para visualización simplificada de competencias                      | Visualización simplificada para no técnicos       | Alta      | Frontend       | Dado que accedo al perfil de un candidato, cuando visualizo sus competencias, entonces deben estar organizadas y claras.| 3              |
| T5  | Implementar ranking automático de candidatos basado en afinidad vectorial       | Ranking automático de afinidad                    | Alta      | IA/ML          | Dado que he creado una vacante, cuando analice candidatos, entonces debe calcular y asignarles un puntaje de afinidad. | 13             |
| T6  | Crear microservicio `candidate-scoring-service`                                 | Ranking automático de afinidad                    | Alta      | Backend/IA     | Dado que se evalúa afinidad, cuando consulto un candidato, entonces el servicio debe devolver la puntuación correcta.  | 5              |
| T7  | Diseñar visualización del ranking + indicador visual (barra, color, badges)     | Indicador visual de coincidencia                  | Alta      | Frontend       | Dado que veo la lista de candidatos, cuando uno tenga más del 80% de match, entonces debe tener un indicador visual.   | 3              |
| T8  | Crear módulo de filtrado por afinidad (%) en listado de candidatos              | Filtro por afinidad                               | Alta      | Frontend       | Dado que estoy en la lista, cuando selecciono un filtro (ej. 80%+), entonces solo se muestran los candidatos relevantes.| 3              |
| T9  | Entrenar módulo de explicabilidad de IA (SHAP/LIME o reglas manuales)           | Transparencia del algoritmo                       | Alta      | IA/ML          | Dado que reviso el ranking, cuando consulto un candidato, entonces debo ver los factores clave que influyeron.         | 8              |
| T10 | Exponer explicaciones de IA en `explainability-service` vía API                 | Transparencia del algoritmo                       | Alta      | Backend/IA     | Dado que solicito detalles de afinidad, cuando accedo al API, entonces recibo un resumen explicativo del resultado.    | 3              |
| T11 | Agregar tooltip “¿por qué este candidato?” en UI de ranking                     | Transparencia del algoritmo                       | Alta      | Frontend       | Dado que veo un candidato, cuando paso el cursor o abro el detalle, entonces veo por qué fue recomendado.              | 2              |
| T12 | Crear sistema de alertas configurables por criterios críticos                   | Alertas de coincidencia crítica                   | Alta      | Backend        | Dado que defino criterios críticos, cuando un candidato los cumpla, entonces se activa una alerta.                     | 5              |
| T13 | Integrar alertas por email (Gmail API) y notificaciones en la app               | Alertas de coincidencia crítica                   | Alta      | Backend/Integr | Dado que se activa una alerta, cuando la condición se cumple, entonces recibo un email o notificación en la app.       | 5              |

| T14 | Implementar carga masiva de CVs con barra de progreso                           | Carga masiva y resumen automático                 | Media     | Frontend       | Dado que cargo varios CVs, cuando se complete la carga, entonces debo ver progreso y confirmación.                    | 5              |
| T15 | Procesamiento por lotes para CVs cargados masivamente                           | Carga masiva y resumen automático                 | Media     | Backend        | Dado que cargo múltiples CVs, cuando finaliza el proceso, entonces se generan los resúmenes por candidato.             | 8              |
| T16 | Diseñar y desarrollar módulo de comparación visual entre perfiles               | Comparación entre perfiles                        | Media     | Frontend       | Dado que selecciono dos candidatos, cuando pulso comparar, entonces veo sus diferencias clave lado a lado.             | 5              |
| T17 | Crear panel de configuración de pesos de criterios de evaluación                | Personalización para startups (mejora sugerida)   | Media     | Frontend       | Dado que configuro una vacante, cuando ajusto los pesos, entonces se aplican al matching de afinidad.                  | 5              |

| T18 | Validación y guía para carga de CVs incorrectos (formato, legibilidad)          | Recomendaciones de carga                          | Baja      | Frontend       | Dado que subo un CV malformado, cuando sea rechazado, entonces debo ver una recomendación de formato o ejemplo.        | 3              |
| T19 | Documentar API simplificada para integraciones (Zapier, Slack, etc.)            | Integración técnica limitada (problema común)     | Baja      | Integración    | Dado que accedo a la documentación, cuando necesito integrar, entonces encuentro endpoints y ejemplos claros.          | 3              |


# 4. ESTIMAR ESFUERZO

| Nº  | Ticket Técnico                                                                 | Pts (Fibonacci) | Estimación (hrs) | Comentario                                                                                                                                      |
|-----|----------------------------------------------------------------------------------|------------------|-------------------|-------------------------------------------------------------------------------------------------------------------------------------------------|
| T1  | Crear parser de CV multiformato con OCR                                         | 8                | 16–24 h            | Requiere lectura de múltiples formatos, OCR y parsing estructurado.                                                                             |
| T2  | Modelo NER para extracción de entidades laborales                               | 13               | 24–40 h            | Incluye entrenamiento, testing y evaluación con dataset laboral.                                                                                |
| T3  | Microservicio `cv-parsing-service`                                              | 5                | 10–16 h            | Servicio RESTful para consumir el parser y entregar resultados.                                                                                 |
| T4  | UI visualización de competencias (no técnicas)                                  | 3                | 6–10 h             | Interfaz amigable para usuarios no técnicos, uso de badges o etiquetas.                                                                         |
| T5  | Ranking automático de afinidad (vectorial)                                      | 13               | 24–40 h            | Matching semántico basado en embeddings, pesos y normalización.                                                                                 |
| T6  | Microservicio `candidate-scoring-service`                                       | 5                | 10–16 h            | Encapsula la lógica de afinidad y facilita integración con frontend.                                                                            |
| T7  | Visualización del ranking + indicadores visuales                                | 3                | 6–10 h             | Barras de color, íconos de coincidencia y elementos visuales UX.                                                                                |
| T8  | Filtro por afinidad (%)                                                         | 3                | 6–10 h             | Filtro dinámico en listado de candidatos con respuesta inmediata.                                                                               |
| T9  | Módulo de explicabilidad de IA (SHAP/LIME o reglas manuales)                   | 8                | 16–24 h            | Explicabilidad orientada a confianza del usuario en IA.                                                                                         |
| T10 | API `explainability-service`                                                    | 3                | 6–10 h             | Expone explicación del score de afinidad por candidato.                                                                                         |
| T11 | Tooltip “¿por qué este candidato?”                                              | 2                | 4–6 h              | Requiere consumo del `explainability-service` y visualización sencilla.                                                                        |
| T12 | Sistema de alertas configurables por criterios críticos                         | 5                | 10–16 h            | Alerta interna basada en reglas, configurable por el usuario.                                                                                   |
| T13 | Integración con Gmail API para alertas                                          | 5                | 10–16 h            | Integración con API externa, requiere autenticación y envío.                                                                                    |
| T14 | Carga masiva de CVs con barra de progreso                                       | 5                | 10–16 h            | Validación, progreso, feedback en UI y manejo de errores.                                                                                       |
| T15 | Procesamiento por lotes para CVs cargados                                       | 8                | 16–24 h            | Procesamiento asíncrono con colas y consolidación de resultados.                                                                                |
| T16 | Comparación visual entre perfiles                                               | 5                | 10–16 h            | Componente UI para comparar competencias, skills y experiencia lado a lado.                                                                    |
| T17 | Panel de configuración de pesos de criterios                                    | 5                | 10–16 h            | Permite modificar importancia de criterios para el matching (por vacante).                                                                     |
| T18 | Validación y guía para carga de CVs incorrectos                                 | 3                | 6–10 h             | Mensajes contextuales y ejemplos de formatos aceptados.                                                                                         |
| T19 | Documentar API simplificada para integraciones externas                         | 3                | 6–10 h             | Guía técnica con ejemplos para desarrolladores externos (Zapier, Slack, etc.).                                                                  |


# 4.2. PRIORIZACION

Criterios de priorización usados:
Problemas comunes identificados previamente, como:
Falta de confianza en IA → requiere explicabilidad.
Complejidad para usuarios nuevos → requiere buena visualización.
Poca personalización → requiere panel de configuración.
Saturación de información → requiere procesamiento por etapas.
Necesidad de automatizar matching → requiere parser + afinidad.

Requisitos técnicos clave, como:
Parser y NER son prerequisitos para todo el flujo IA.
Matching depende del parsing y el modelo de afinidad.
Visualizaciones deben venir después de la lógica IA.
Alerta crítica y explicabilidad aumentan confianza de usuario.


| Nº  | Ticket Técnico                                                                 | Historia de Usuario Asociada                  | Prioridad | Pts | Estimación (hrs) | Comentario                                                                                      |
|-----|----------------------------------------------------------------------------------|-----------------------------------------------|-----------|-----|-------------------|-------------------------------------------------------------------------------------------------|
| T1  | Crear parser de CV multiformato con OCR                                         | Extracción automática de habilidades          | ⭐️Alta   | 8   | 16–24 h            | Base para extracción y matching; dependencia crítica.                                           |
| T2  | Modelo NER para extracción de entidades laborales                               | Extracción automática de habilidades          | ⭐️Alta   | 13  | 24–40 h            | Extrae competencias y datos clave para matching y evaluación.                                   |
| T3  | Microservicio `cv-parsing-service`                                              | Extracción automática de habilidades          | ⭐️Alta   | 5   | 10–16 h            | Encapsula el procesamiento de CVs para otros servicios.                                         |
| T5  | Ranking automático de afinidad (vectorial)                                      | Matching inteligente                          | ⭐️Alta   | 13  | 24–40 h            | Core del sistema de selección basado en IA.                                                     |
| T6  | Microservicio `candidate-scoring-service`                                       | Matching inteligente                          | ⭐️Alta   | 5   | 10–16 h            | Servicio REST para puntaje de afinidad con candidatos.                                          |
| T9  | Módulo de explicabilidad de IA (SHAP/LIME o reglas manuales)                   | Transparencia del algoritmo                   | ⭐️Alta   | 8   | 16–24 h            | Permite entender por qué un candidato es sugerido por IA.                                       |
| T10 | API `explainability-service`                                                    | Transparencia del algoritmo                   | ⭐️Alta   | 3   | 6–10 h             | Expone las razones del score para el frontend.                                                  |
| T11 | Tooltip “¿por qué este candidato?”                                              | Transparencia del algoritmo                   | ⭐️Alta   | 2   | 4–6 h              | Información visual directa sobre la decisión del sistema.                                       |
| T12 | Sistema de alertas configurables por criterios críticos                         | Alertas de coincidencia crítica               | ⭐️Alta   | 5   | 10–16 h            | Disparador clave para candidatos estratégicos.                                                  |
| T13 | Integración con Gmail API para alertas                                          | Alertas de coincidencia crítica               | ⭐️Alta   | 5   | 10–16 h            | Para notificaciones inmediatas al reclutador/founder.                                           |
| T4  | UI visualización de competencias (no técnicas)                                  | Visualización simplificada                    | ⭐️Alta   | 3   | 6–10 h             | Mejora de experiencia para perfiles no técnicos.                                                |
| T7  | Visualización del ranking + indicadores visuales                                | Indicador visual de coincidencia              | ⭐️Alta   | 3   | 6–10 h             | Mejora la priorización visual de perfiles afines.                                               |
| T8  | Filtro por afinidad (%)                                                         | Filtro por afinidad                           | ⭐️Alta   | 3   | 6–10 h             | Funcionalidad esencial para reducir volumen de revisión.                                        |

| T15 | Procesamiento por lotes para CVs cargados                                       | Carga masiva y resumen automático             | 🟡Media  | 8   | 16–24 h            | Permite análisis en masa de CVs (para startups con alta demanda).                               |
| T14 | Carga masiva de CVs con barra de progreso                                       | Carga masiva y resumen automático             | 🟡Media  | 5   | 10–16 h            | Mejora UX para reclutadores multitarea.                                                         |
| T16 | Comparación visual entre perfiles                                               | Comparación entre candidatos                  | 🟡Media  | 5   | 10–16 h            | Para análisis de decisión en etapas finales del funnel.                                         |
| T17 | Panel de configuración de pesos de criterios                                    | Personalización de evaluación (mejora)        | 🟡Media  | 5   | 10–16 h            | Para startups que priorizan cultura o potencial por encima de experiencia.                      |

| T18 | Validación y guía para carga de CVs incorrectos                                 | Recomendaciones de carga                      | 🔽Baja   | 3   | 6–10 h             | Mejora onboarding de nuevos usuarios, no bloqueante.                                             |
| T19 | Documentar API simplificada para integraciones externas                         | Integración con herramientas (problema común) | 🔽Baja   | 3   | 6–10 h             | Para extensibilidad del sistema con herramientas de startup.                                    |

RESUMEN POR PRIORIDAD

| Prioridad | Tickets incluidos | Puntos Totales | Horas Aproximadas |
| --------- | ----------------- | -------------- | ----------------- |
| Alta      | T1–T13            | 75             | 150–260 h         |
| Media     | T14–T17           | 23             | 46–66 h           |
| Baja      | T18–T19           | 6              | 12–20 h           |


  
  

