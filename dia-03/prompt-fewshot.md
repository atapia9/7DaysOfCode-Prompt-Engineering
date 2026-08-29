# Día 3 — Prompt completo (Few-Shot)

Estructura: **PERSONA + TAREA con ejemplos + ENTRADA + CONTEXTO**.

```text
PAPEL (PERSONA):
[bloque completo de ../dia-02/persona-mentora.md — Renata Salas]

TAREA:
Abajo hay dos ejemplos de cómo quiero que se escriba un plan de estudio semanal.
Aprende el PATRÓN —estructura, extensión y tono—, no el contenido.
Después arma mi próxima semana siguiendo exactamente ese patrón: nueve líneas,
meta arriba, entregable y destinatario abajo.

EXEMPLO 1
[ejemplo de fotografía de producto — ver formato-plan-semanal.md]

EXEMPLO 2
[ejemplo de examen teórico de manejo — ver formato-plan-semanal.md]

AHORA ES MI TURNO:
Entrada: prioridad 1 de mi lista de hard skills del Día 2 — construir flujos de
trabajo con IA en una sola herramienta de automatización (n8n o Make), con el
objetivo de poder entregar el Nivel 3 de mi oferta ("AI Workflow Sprint").
Contexto: [bloque completo de ../dia-01/perfil-base-contexto.md]
Salida:
```

## La línea de rescate

Si en las siguientes semanas el formato empieza a resbalarse —párrafos que crecen,
días que se convierten en tres subtareas—, se agrega esta línea al final de la TAREA:

> Mantén exactamente la estructura de los ejemplos, incluido el número de líneas.

## Zero-shot vs Few-shot, en una tabla

| | Zero-shot | Few-shot |
|---|---|---|
| **Qué le doy** | La tarea descrita con palabras | 2–4 pares de entrada/salida |
| **Qué adivina el modelo** | Estructura, extensión, tono | Solo el contenido |
| **Cuándo conviene** | Tarea común, formato indiferente | Cuando necesito el **mismo** formato cada vez |
| **Riesgo** | Cada corrida sale distinta | Si los ejemplos son de mi tema, copia el contenido |

Los días 1 y 2 fueron zero-shot y funcionaron: eran tareas de una sola vez. El Día 3
cambia el juego porque el Tutor del Día 7 tiene que entregar un plan **cada semana**, y
ahí la consistencia deja de ser estética y se vuelve funcional.
