---
name: prompt-engineering
description: "Técnicas de ingeniería de prompts (dar instrucciones claras, role prompting, few-shot, cadena de pensamiento, autoconsistencia) para obtener mejores resultados de un modelo de lenguaje. Usar cuando se necesite: redactar o mejorar un prompt para una tarea específica, decidir entre pedir un ejemplo (few-shot) o dejar que el modelo razone paso a paso (cadena de pensamiento), estructurar un prompt complejo en partes, o diagnosticar por qué un prompt no está dando el resultado esperado. Basado en la certificación oficial Prompt Engineering Foundation (Certiprof, CPEFPC)."
---

# Ingeniería de prompts

Técnicas prácticas para comunicarse con un modelo de lenguaje de forma que dé mejores resultados, más allá de "preguntar y ver qué sale".

## Técnicas principales

1. **Dar instrucciones claras** — La calidad de la salida depende directamente de cuán específica es la instrucción: qué se quiere, en qué formato, con qué restricciones. Ambigüedad en el prompt = ambigüedad en la respuesta.

2. **Role prompting** — Pedirle al modelo que asuma un rol específico ("actúa como un editor técnico", "responde como un abogado") ayuda a fijar el tono, vocabulario y criterios de la respuesta.

3. **Few-shot prompting** — Dar 1 o más ejemplos del resultado esperado antes de pedir la tarea real. Útil cuando el formato de salida es específico y difícil de describir solo con instrucciones.

4. **Zero-shot prompting** — Pedir la tarea sin ejemplos previos, apoyándose solo en el conocimiento general del modelo. Funciona bien para tareas comunes; para tareas con formato muy específico, few-shot suele dar mejor resultado.

5. **Cadena de pensamiento (Chain of Thought)** — Pedir explícitamente que el modelo razone paso a paso antes de dar la respuesta final. Mejora la precisión en tareas que requieren varios pasos lógicos o matemáticos, y hace el razonamiento auditable.

6. **Autoconsistencia** — Para tareas donde la precisión importa mucho, generar varias respuestas independientes con cadena de pensamiento y quedarse con la más consistente/repetida entre ellas.

7. **Prompting de menos a más (least-to-most)** — Descomponer un problema complejo en subproblemas más simples y resolverlos en secuencia, en vez de pedir la solución completa de una vez.

8. **Combinar técnicas** — Role prompting + few-shot + cadena de pensamiento no son excluyentes; combinarlas suele dar mejores resultados que usar una sola.

## Aplicaciones prácticas comunes
Estructurar datos no estructurados, redactar correos/documentos con un estilo específico, resumir texto largo, asistencia de código, adaptar el mismo contenido a distintos estilos de escritura.

## Trampas comunes de los LLM a tener presente
- Pueden generar información plausible pero incorrecta si el prompt no da suficiente contexto (alucinación).
- Tienen límites de memoria de conversación — para tareas largas, resumir o reafirmar contexto clave periódicamente.
- Un prompt vago tiende a producir una respuesta genérica; ser específico sobre formato, longitud y criterios de éxito mejora notablemente el resultado.

## Cómo aplicar esto de forma general
Antes de escribir un prompt complejo, preguntar: ¿necesito que el modelo razone paso a paso (cadena de pensamiento) o solo que siga un formato (few-shot)? ¿Le estoy dando suficiente contexto de rol y restricciones, o estoy asumiendo que "va a entender lo que quiero"?

## Referencia
Ver `references/temario-oficial.md` para el temario completo por módulo si se necesita profundizar en una técnica puntual (formalización de prompts, manejo de contenido de formato largo, etc.).
