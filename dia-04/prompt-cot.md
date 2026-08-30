# Día 4 — Prompt completo (Chain of Thought)

Estructura: **PERSONA + CONTEXTO + PLAN ACTUAL + DILEMA + TAREA por pasos**.

```text
PAPEL (PERSONA):
[bloque completo de ../dia-02/persona-mentora.md — Renata Salas]

CONTEXTO:
[bloque completo de ../dia-01/perfil-base-contexto.md]

PLAN ACTUAL:
[la Semana 1 generada en ../dia-03/salida-semana-01.md]

MI DILEMA:
Mi Semana 1 arranca construyendo un flujo con IA, pero el ejercicio del Día 2 mostró
que la primera objeción de un comprador de PyME no es la automatización, sino qué pasa
con la información de su empresa cuando la mete en una IA. Con 30 minutos al día no
puedo hacer las dos cosas a la vez. ¿Construyo primero el flujo, o empaqueto primero
la política de manejo de información que ya prometí en la versión 1.2 de mi oferta?

TAREA:
[la secuencia de seis pasos de secuencia-cot.md]
```

## De dónde salió este dilema

No lo inventé para el ejercicio. Apareció solo, al poner uno junto a otro dos archivos
de este mismo repositorio:

- El **Día 2** dijo que el comprador pone la seguridad de la información en primer lugar
  y la automatización en tercero.
- El **Día 3** armó la Semana 1 empezando por la automatización.

Y en medio, `mi_oferta.md` v1.2 ya promete por escrito una política de manejo de
información que todavía no existe. Ese es el dilema real: dos días seguidos dieron
respuestas coherentes entre sí y contradictorias en el orden.

## Cuatro días, cuatro capas

| Día | Qué agregó al prompt | Qué produce |
|---|---|---|
| 1 | Papel, Tarea, Contexto | Un diagnóstico específico |
| 2 | Persona en cuatro capas | Un plan con criterio propio |
| 3 | Ejemplos de entrada y salida | Un formato repetible |
| 4 | Pasos de razonamiento | Una decisión auditable |

El Día 4 es el primero que no produce contenido nuevo, sino que **ordena** el que ya
tenía. Es también el primero que se puede revisar paso por paso cuando la conclusión no
convence.
