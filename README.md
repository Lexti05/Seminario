# SIPREC (Sistema Inteligente de Prevención de Fallas en Equipos de Cómputo)

# Investigación previa

**1. Problema**

¿Qué situación, necesidad o problema quieren atender?

El problema central es la falta de monitoreo preventivo accesible en los equipos de cómputo, lo que provoca que los problemas se atiendan únicamente cuando ya afectan su funcionamiento. Aunque el hardware genera información sobre su estado, esta no es comprensible para el usuario promedio. Como consecuencia, no se detectan a tiempo señales de desgaste, lo que deriva en interrupciones en las actividades, costos no planificados, deterioro progresivo del equipo y posible pérdida de información.

**2. Objetivo general y objetivos particulares (máximo 4)**

Transformar el mantenimiento de equipos de cómputo de un modelo reactivo a uno preventivo: en el que el propio sistema detecte el desgaste o mal funcionamiento del hardware con anticipación y lo comunique al usuario en un lenguaje claro, sin que este necesite conocimientos técnicos para actuar a tiempo.

- Detectar comportamientos anómalos en el hardware que puedan indicar una posible falla.
- Traducir esas señales técnicas en alertas y recomendaciones comprensibles para cualquier usuario.
- Reducir interrupciones, costos de reparación no planificados y pérdida de vida útil de los equipos que se derivan de no detectar a tiempo las señales de desgaste.

**3. Alcance**

¿Qué sí contempla el proyecto?

- Agente cliente que recolecta métricas de hardware (CPU, RAM, temperatura, almacenamiento/SMART) en equipos con Windows.
- Servidor central con base de datos PostgreSQL para almacenar la telemetría.
- Modelo de IA capaz de analizar las métricas recopiladas y detectar comportamientos anómalos que puedan indicar una posible falla.
- Generación de diagnósticos y recomendaciones preventivas comprensibles para el usuario.
- Dashboard web para visualizar el estado de los equipos y las alertas.
- Scripts de mantenimiento preventivo, ejecutables solo con autorización previa del usuario.

**4. Fuera de alcance**

¿Qué cosas deliberadamente no realizará el proyecto?

- Ejecución automática de acciones correctivas sin aprobación previa del usuario.
- Soporte para sistemas operativos distintos a Windows en esta primera fase.
- Reparación física o soporte técnico presencial de los equipos.
- Predicción de cualquier tipo de falla o diagnóstico definitivo del componente afectado.

**5. MVP (Minimum Viable Product)**

¿Cuál es la versión mínima del proyecto que permitiría demostrar que la propuesta funciona?

La versión mínima del proyecto será un sistema capaz de monitorear las métricas básicas de un equipo con Windows, analizarlas mediante un modelo de IA básico, detectar comportamientos inusuales y alertar al usuario.

El MVP incluirá:

- Recolección de métricas básicas de CPU, RAM, temperatura y almacenamiento.
- Envío de las métricas para su análisis.
- Análisis mediante un modelo de IA básico para identificar comportamientos anómalos.
- Generación de alertas cuando se detecte una posible señal de desgaste o mal funcionamiento.
- Recomendaciones básicas de mantenimiento para el usuario.
