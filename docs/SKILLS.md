# Documentación de las skills

Cada skill se activa sola cuando el contexto de la conversación coincide con su `description` (frontmatter del `SKILL.md`) — no hay que invocarlas por nombre.

---

## design-thinking
**Qué es:** framework de descubrimiento centrado en las personas — evita diseñar una solución antes de entender bien el problema.
**Se activa cuando:** hay que preparar preguntas para entender la necesidad de un usuario/cliente, separar el síntoma reportado del problema real, generar varias ideas sin cerrarse a la primera obvia, o armar un prototipo/mockup antes de construir la versión completa.
**Conceptos clave:** las 5 fases — Empatizar (mapa de empatía, journey map), Definir (Point of View, "¿Cómo podríamos...?"), Idear (brainstorming, SCAMPER), Prototipar (baja fidelidad, bajo costo), Evaluar (validar con la persona real, no solo revisión interna).
**Aporte diferencial:** separar explícitamente "lo que la persona dijo que era el problema" del "problema real identificado".

## lean-six-sigma
**Qué es:** metodología DMAIC para llegar de "algo anda mal" a una causa raíz identificada y una mejora medible.
**Se activa cuando:** hay que encontrar causa raíz (no solo el síntoma), reducir desperdicio o variabilidad en un proceso, estructurar un análisis de datos para encontrar cuellos de botella, o justificar una mejora con ROI.
**Conceptos clave:** Definir (Project Charter, SIPOC), Medir (tendencia central, dispersión, confiabilidad de la medición), Analizar (Ishikawa, Pareto 80/20, AMEF/FMEA), Mejorar (desperdicio Lean vs. variabilidad Six Sigma), Controlar (estandarizar, documentar, monitorear).
**Aporte diferencial:** no saltar de "hay un problema" a "la solución es X" sin pasar por Medir y Analizar.

## business-intelligence
**Qué es:** framework de extracción, transformación y visualización de datos (ETL) para convertir datos crudos en información útil para decidir.
**Se activa cuando:** hay que limpiar/transformar datos antes de analizarlos, definir cómo se relacionan dos o más tablas, elegir el tipo de visualización adecuado, o trabajar puntualmente con Power BI (Power Query, DAX) o Qlik Sense (scripting, Joins).
**Conceptos clave:** orden ETL (extraer → limpiar/transformar → modelar relaciones → visualizar), validación de tipo de dato por columna antes de agregar, elección de gráfico según el mensaje (barra para comparar, línea para evolución, evitar torta con muchas categorías).
**Aporte diferencial:** nunca reportar una estadística sin haber verificado tipo de dato y outliers.

## data-storytelling
**Qué es:** framework para convertir un hallazgo de datos en algo que la audiencia entienda, recuerde y sobre lo que actúe.
**Se activa cuando:** hay que presentar un hallazgo a audiencia no técnica, estructurar la narrativa alrededor de un insight, decidir entre enfoque exploratorio (dashboard) o explicativo (conclusión guiada), o mejorar una comunicación que solo reporta números.
**Conceptos clave:** Explicar / Iluminar / Comprometer; explicativo vs. exploratorio; empezar por el insight (no por el proceso de análisis) y cerrar con la acción sugerida.
**Aporte diferencial:** distinguir informar el dato de explicar qué implica y qué se debería hacer al respecto.
**Se conecta con:** `business-intelligence` (de dónde viene el dato que se está narrando).

## innovation-management
**Qué es:** framework para que una propuesta de mejora no se quede solo en optimizar lo existente, y para no recomendar apuestas grandes sin validarlas.
**Se activa cuando:** hay que clasificar si una idea es mejora incremental o cambio de modelo de negocio, pasar de una queja general a un problema bien definido, validar una idea riesgosa con bajo costo, o argumentar diferenciación frente a la competencia.
**Conceptos clave:** tipos de innovación (incremental / radical / transformacional), árbol de problemas (tema → problema medible → proyecto), Lean Startup (Crear-Medir-Aprender), modelo de negocio, los 10 tipos de innovación como mapa de dónde buscar oportunidades.
**Aporte diferencial:** si la propuesta es una apuesta no probada, decirlo explícitamente y sugerir una forma barata de validarla primero.

## project-management-pm2
**Qué es:** metodología PM² (Comisión Europea, CC BY 4.0) para planificar y ejecutar un proyecto de forma simple, sin requerir formación previa.
**Se activa cuando:** hay que armar un cronograma o EDT/WBS, definir roles y responsabilidades, identificar interesados, estructurar el ciclo de vida de una iniciativa, o cerrar un proyecto con informe final y lecciones aprendidas.
**Conceptos clave:** ciclo de vida en 4 fases (Inicio, Planificación, Ejecución, Cierre) + monitoreo transversal; EDT/WBS, matriz de interesados, análisis básico de riesgos; roles típicos (Comité de Dirección, Director de Proyecto, equipo).
**Aporte diferencial:** el cierre siempre debe incluir cómo el resultado se sostiene solo, no solo un reporte de lo hecho.

## prompt-engineering
**Qué es:** técnicas prácticas para comunicarse con un modelo de lenguaje y obtener mejores resultados, más allá de "preguntar y ver qué sale".
**Se activa cuando:** hay que redactar o mejorar un prompt, decidir entre few-shot o cadena de pensamiento, estructurar un prompt complejo en partes, o diagnosticar por qué un prompt no está funcionando.
**Conceptos clave:** instrucciones claras, role prompting, few-shot vs. zero-shot, cadena de pensamiento (Chain of Thought), autoconsistencia, descomposición least-to-most, combinación de técnicas.
**Aporte diferencial:** distinguir si el problema del prompt es de contexto/rol insuficiente o de falta de razonamiento paso a paso.

## ai-literacy
**Qué es:** marco conceptual no técnico para explicar y razonar sobre IA con alguien que no programa ni entrena modelos.
**Se activa cuando:** hay que explicar IA a alguien sin formación técnica, desmentir un mito común, evaluar en términos generales si una tarea es candidata a automatización con IA, o discutir riesgos/limitaciones de forma balanceada.
**Conceptos clave:** IA / ML / Deep Learning / Big Data (relación entre los cuatro), mitos comunes (reemplazo total de empleos, infalibilidad, complejidad inexplicable), sesgo algorítmico, privacidad de datos, impacto en el trabajo (automatización parcial vs. roles nuevos).
**Aporte diferencial:** al evaluar si una tarea es candidata a IA, preguntar por datos históricos representativos, tolerancia al error y necesidad de explicabilidad.

---

## Cómo se relacionan entre sí
`design-thinking` (entender el problema) y `lean-six-sigma` (encontrar causa raíz en un proceso) suelen combinarse en un mismo diagnóstico. `business-intelligence` prepara los datos que `data-storytelling` convierte en narrativa para decisión. `innovation-management` y `project-management-pm2` entran cuando el diagnóstico ya definió qué hacer y hay que fundamentar el nivel de riesgo o estructurar la ejecución. `prompt-engineering` y `ai-literacy` son transversales — aplican a cómo se usa Claude y a cómo se explica IA en cualquiera de los casos anteriores.
