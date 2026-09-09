---
name: ai-literacy
description: "Conceptos fundamentales de inteligencia artificial para audiencia no técnica: qué es IA, Machine Learning y Deep Learning, mitos comunes, oportunidades, riesgos de seguridad y sesgo, e impacto en el trabajo. Usar cuando se necesite explicar IA a alguien sin formación técnica, desmentir un mito común sobre IA, evaluar de forma general si una tarea es candidata a automatización con IA, o discutir riesgos/limitaciones de forma balanceada. Basado en la certificación oficial Generative AI Professional Certification (Certiprof, GAIPC)."
---

# Alfabetización en IA

Marco conceptual (no técnico) para explicar y razonar sobre IA con alguien que no programa ni entrena modelos — útil para comunicación, capacitación o toma de decisiones de negocio.

## Conceptos base

- **Inteligencia Artificial**: la capacidad de las máquinas para imitar comportamiento humano, aprender y mejorar con el tiempo, y razonar/tomar decisiones.
- **Machine Learning (ML)**: subconjunto de la IA que permite a las máquinas aprender de datos sin ser programadas explícitamente para cada caso.
- **Deep Learning**: subconjunto del ML que usa redes neuronales de varias capas; requiere más datos y cómputo pero maneja mejor problemas complejos (imagen, voz, lenguaje).
- **Big Data**: conjuntos de datos tan grandes y complejos que requieren métodos distintos a los tradicionales para procesarlos — es el "combustible" que hace posible el ML moderno.

## Mitos comunes a desmentir
- "La IA reemplazará todos los trabajos humanos" — en la práctica automatiza tareas, no roles completos; muchas tareas requieren habilidades creativas/sociales que aún no replica bien.
- "La IA siempre toma las decisiones correctas" / "es invulnerable a errores" — los modelos heredan sesgos de los datos con que se entrenaron y pueden fallar de forma no obvia.
- "La IA es demasiado compleja para que la gente común la entienda" — los conceptos de fondo (patrones en datos, predicción) son explicables sin matemáticas avanzadas.

## Oportunidades típicas
Detección temprana de problemas/anomalías a partir de datos, personalización de servicios, automatización de tareas rutinarias, apoyo a la toma de decisiones (no reemplazo de esta).

## Riesgos y seguridad a tener presentes
- **Sesgo algorítmico**: un modelo entrenado con datos no representativos reproduce y a veces amplifica ese sesgo. Mitigación: usar datos diversos, auditar resultados, no asumir neutralidad por defecto.
- **Privacidad de datos**: los sistemas de IA suelen depender de datos personales; hay que ser explícito sobre qué se usa y con qué fin.
- **Mal uso**: la misma capacidad que automatiza una tarea legítima puede usarse para desinformación, fraude, etc. — vale la pena nombrar el riesgo al proponer una solución con IA.

## Impacto en el trabajo
Algunos trabajos se automatizan parcialmente, se crean nuevos roles centrados en supervisar/dirigir sistemas de IA, y cambian las habilidades requeridas (menos tarea repetitiva, más criterio y verificación).

## Cómo aplicar esto de forma general
- Al explicar una solución con IA a alguien no técnico, distinguir claramente ML (aprende de datos) de Deep Learning (redes neuronales, más "caja negra") — ayuda a fijar expectativas de qué tan explicable es el sistema.
- Al evaluar si una tarea es candidata a IA: ¿hay suficientes datos históricos representativos? ¿el error tolerable es alto o bajo? ¿el resultado necesita ser explicable a un humano?

## Referencia
Ver `references/temario-oficial.md` para el temario completo por capítulo si se necesita profundizar en un tema puntual.
