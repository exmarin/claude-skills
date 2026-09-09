---
name: business-intelligence
description: "Principios de Business Intelligence: extracción, transformación, modelado y visualización de datos para la toma de decisiones, incluyendo el uso de Power BI y Qlik Sense. Usar cuando se necesite: limpiar/transformar datos antes de analizarlos, definir cómo se relacionan dos o más tablas (modelo de datos), elegir el tipo de visualización adecuado para comunicar un hallazgo, o trabajar específicamente con Power BI (Power Query, DAX) o Qlik Sense (scripting, Joins). Basado en la certificación oficial Business Intelligence Analyst (Certiprof, BIAPC)."
---

# Business Intelligence

Marco de extracción, transformación y visualización de datos (ETL) para convertir datos crudos en información útil para decidir.

## Conceptos ETL

1. **Extracción y carga** — Identificar qué fuentes/columnas son relevantes para la pregunta que se está respondiendo. No cargar todo a ciegas.

2. **Transformación** (equivalente a Power Query en Power BI, o scripting en Qlik Sense):
   - Eliminar filas/columnas vacías o de encabezado antes de calcular nada.
   - Verificar el tipo de dato por columna (numérico, texto, fecha) antes de agregar — un error de formato aquí invalida cualquier análisis posterior.
   - Cruzar tablas (Join/Merge) requiere una llave común real (mismo campo/nombre) entre ambas.

3. **Modelo de datos** — Cuando hay más de una tabla involucrada, dejar explícita la relación (uno a muchos, llave común) antes de calcular métricas cruzadas.

4. **Visualización** — Elegir el tipo de gráfico según lo que se quiere comunicar:
   - Comparar categorías → barra.
   - Evolución en el tiempo → línea.
   - Composición de un total → evitar sobrecargar con torta si hay muchas categorías; considerar tabla ordenada.
   - Priorizar que la audiencia entienda el hallazgo rápido, no que el gráfico se vea sofisticado.

## Herramientas específicas del curso original

- **Power BI**: Power Query (transformación, lenguaje M), modelo de relaciones (Relationship/Data View), Report View para visualización, medidas y columnas calculadas en DAX.
- **Qlik Sense**: scripting y modelo de datos, comandos Join/Concatenate, funciones para visualizaciones, archivos .qvd/.qvf.

## Cómo aplicar esto de forma general
- Los principios de ETL y modelado aplican independiente de la herramienta (Excel, Power BI, Qlik, SQL, Python/pandas) — lo importante es el orden: extraer → limpiar/transformar → modelar relaciones → recién ahí visualizar.
- Nunca reportar una estadística sin haber verificado que la columna es realmente del tipo esperado y sin outliers evidentes que la distorsionen.

## Referencia
Ver `references/conceptos-transferibles.md` para más detalle sobre el temario específico de Power BI y Qlik Sense si el trabajo requiere usar esas herramientas puntualmente.
