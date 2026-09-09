---
name: lean-six-sigma
description: "Metodología Lean Six Sigma / DMAIC (Definir-Medir-Analizar-Mejorar-Controlar) para diagnosticar y resolver problemas de calidad, eficiencia o variabilidad en un proceso. Usar cuando se necesite: identificar causa raíz de un problema (no solo el síntoma), reducir desperdicio o variabilidad en un proceso, estructurar un análisis de datos para encontrar cuellos de botella, o justificar formalmente una mejora con ROI. Basado en la certificación oficial Lean Six Sigma Green Belt (Certiprof, LSSGBPC)."
---

# Lean Six Sigma (DMAIC)

Marco para pasar de "algo anda mal" a una causa raíz identificada y una mejora medible, en vez de recomendar soluciones por intuición.

## Las 5 fases (DMAIC)

1. **Definir (Define)** — Delimitar el proceso antes de analizarlo:
   - **Project Charter** en pocas líneas: problema, objetivo medible, alcance.
   - **SIPOC** (Proveedor–Entrada–Proceso–Salida–Cliente) para tener el proceso completo en una vista.

2. **Medir (Measure)** — Caracterizar el proceso con datos, no con impresiones:
   - Medidas de tendencia central (promedio, mediana) y de dispersión (rango, varianza, desviación estándar) sobre los datos disponibles.
   - Si se está midiendo con un instrumento o criterio subjetivo, validar primero que la forma de medir es confiable (equivalente conceptual a un Gage R&R: ¿el mismo caso medido dos veces da el mismo resultado?).

3. **Analizar (Analyze)** — Buscar causa raíz, no síntomas:
   - **Diagrama de Ishikawa** (causa-efecto): agrupar posibles causas en categorías (personas, método, herramienta/sistema, insumo, medición, entorno).
   - **Pareto**: identificar el ~20% de causas que explican el ~80% del problema.
   - **AMEF/FMEA** cuando el análisis de riesgo lo amerita: priorizar por severidad × ocurrencia × detección (RPN).
   - No pasar a la fase de mejora sin haber nombrado explícitamente la causa raíz.

4. **Mejorar (Improve)** — La solución debe estar conectada a la causa identificada, no ser genérica:
   - Estimar el beneficio esperado (ahorro, tiempo, ROI) para priorizar entre alternativas.
   - Revisar si el problema es de **desperdicio** (Lean: sobreproducción, espera, transporte, sobreproceso, inventario, movimiento, defectos, talento no usado) o de **variabilidad** (Six Sigma), porque la palanca de mejora es distinta en cada caso.

5. **Controlar (Control)** — Sostener la mejora en el tiempo, sobre 3 pilares: estandarizar el proceso, documentarlo, y monitorear que no se degrade (ej. cartas de control simples: ¿el indicador se mantiene dentro de un rango esperado?).

## Cómo aplicar esto de forma general
- Cualquier problema recurrente puede pasar por este ciclo, aunque sea de forma liviana: definir bien qué se está resolviendo, medir con datos reales antes de opinar, buscar causa raíz antes de proponer solución, y no dar la mejora por sostenible sin un mecanismo de control.
- Evitar saltar directo de "hay un problema" a "la solución es X" sin pasar por Medir y Analizar — es el error más común y el que más le resta credibilidad a un diagnóstico.

## Referencia
Ver `references/temario-oficial.md` para el temario completo por unidad (Calidad, Medición, Análisis, Mejora) si se necesita profundizar en una herramienta puntual (AMEF completo, diseño de experimentos, cartas de control específicas, etc.).
