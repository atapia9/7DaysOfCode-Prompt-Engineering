# Día 2 — Prompt completo (Role Prompting)

Estructura: **PERSONA (4 capas) + TAREA + CONTEXTO + DIAGNÓSTICO**.

El bloque `PAPEL (PERSONA)` es el de [`persona-mentora.md`](./persona-mentora.md).
El bloque `CONTEXTO` es el [Perfil Base del Día 1](../dia-01/perfil-base-contexto.md).
El bloque `DIAGNÓSTICO` es la [salida del Día 1](../dia-01/salida-prompt-ptc.md).

```text
PAPEL (PERSONA):
[bloque completo de persona-mentora.md — Renata Salas]

TAREA:
Con base en el diagnóstico de abajo, arma dos planes separados:

1. HARD SKILLS: las 3 competencias técnicas que debo desarrollar primero, en orden de
   prioridad, con la justificación de cada una y el activo concreto que debe quedar
   terminado.
2. SOFT SKILLS: las 2 competencias de comportamiento más críticas para mi momento, cada
   una con una acción de entrenamiento concreta, repetible y medible.

Cierra con una lista corta de lo que NO debo estudiar todavía, y por qué.

CONTEXTO:
[bloque completo de perfil-base-contexto.md]

DIAGNÓSTICO:
[salida completa de salida-prompt-ptc.md]
```

## Lo que cambia respecto al Día 1

| | Día 1 (PTC) | Día 2 (Role Prompting) |
|---|---|---|
| **Papel** | Una línea: "orientador de carrera en tecnología" | Persona de 4 capas, con nombre, historia, método y prohibiciones |
| **Insumo** | Solo mi contexto | Mi contexto **más** el diagnóstico que ya produjo el Día 1 |
| **Salida** | Diagnóstico | Plan priorizado y ejecutable |
| **Riesgo que corta** | Respuesta genérica | Respuesta complaciente y sobredimensionada |

El Día 1 me dijo *qué me pasa*. El Día 2 usa esa misma información para decidir *qué
hago primero*. Es la primera vez en el reto que la salida de un día es la entrada del
siguiente.
