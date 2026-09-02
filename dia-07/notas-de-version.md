# Notas de versión y cómo mantener el Tutor

## Qué bloque tocar cuando algo cambie

La ventaja de un mega-prompt por capas es que casi nunca hay que reescribirlo entero.

| Si cambia… | Actualizo solo… | Cada cuánto |
|---|---|---|
| Mi tiempo, mi objetivo o mis proyectos | Sección 2 (Contexto) | Cada ciclo de 30 días |
| El puesto o cliente que persigo | Sección 3 (Base de conocimiento) | Cuando cambie el objetivo |
| Lo que ya logré | Sección 3, el reporte de gaps | Cada ciclo |
| Cómo quiero que me hablen | Sección 1 (Persona) | Rara vez |
| El formato del plan | Sección 5 (Patrón) | Rara vez |
| Un vicio nuevo que quiero cortar | Sección 6 (Restricciones) | Cuando aparezca |

El ciclo de mantenimiento es de dos minutos: al terminar los 30 días, actualizo la
sección 2 con lo que cambió, marco en el reporte de gaps lo que ya cerré, y vuelvo a
correr el mismo prompt. Sale el siguiente PDI.

## Bitácora de versiones

| Versión | Fecha | Qué cambió |
|---|---|---|
| v1 | 2 sep 2026 | Primera composición: seis bloques de los días 1 al 6 |

## Lo que aprendí en los siete días

1. **El contexto es el 80% del resultado.** El Día 1 lo demostró con nueve palabras
   contra trescientas treinta, y ninguna técnica posterior cambió esa proporción.

2. **La capa de límites hace más que las otras tres juntas.** Decir lo que la persona
   NO hace cambió el contenido de las respuestas; describir su tono solo cambió la
   superficie.

3. **Un ejemplo vale más que una prohibición.** Dos veces en el reto una regla negativa
   se rompió sola —el día de "investigar", el del cierre motivacional—. Los ejemplos,
   que simplemente no contienen eso, nunca fallaron.

4. **El paso "qué información me falta" es el que convierte la IA en herramienta.**
   Sin él responde como oráculo; con él, mapea lo que todavía tengo que averiguar por
   mi cuenta. Es el paso que me evitó reordenar un plan entero con base en una
   suposición mía disfrazada de hallazgo.

5. **Delimitar es decidir quién tiene permiso de darme órdenes.** El día que metí una
   instrucción escondida dentro de un texto pegado, entendí que esto no es formato:
   es superficie de ataque, y es la parte más vendible de todo lo que hice esta semana.

6. **Pedir la cita cambia lo que la IA se atreve a afirmar.** No mejora la redacción:
   elimina las afirmaciones sin respaldo, porque una fila que debe citar su fuente no
   puede inventarse.

7. **Y el que no esperaba: el reto se volvió el proyecto.** Empezó como un ejercicio de
   prompting y terminó produciendo mi diagnóstico, mi oferta con precio, mi plan de
   estudio, mi política de datos y mi primer caso público. Las técnicas se aprenden
   aplicándolas a algo que importa; si las hubiera practicado con ejemplos de juguete,
   hoy tendría siete archivos bonitos y ninguna decisión tomada.

## Lo que NO hace este tutor

Vale ponerlo por escrito para no confundirme después:

- **No sabe si tengo razón.** Trabaja con los datos que le doy. Si mi contexto está
  desactualizado, su plan será coherente y equivocado.
- **No sustituye una conversación con un cliente.** El Día 4 lo dejó claro: lo que
  falta casi nunca se resuelve estudiando.
- **Su razonamiento visible no es una prueba.** Es una superficie de auditoría. Sirve
  para que yo revise los criterios, no para confiar en que ese fue el camino real.
- **No es una frontera de seguridad.** Las reglas de la sección 6 reducen el riesgo de
  que un texto pegado le dé órdenes; no lo eliminan.

## Próximo ciclo

**1 de octubre de 2026.** Actualizo la sección 2, marco lo cerrado en el reporte de
gaps, y corro `tutor-v2`.
