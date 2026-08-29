# 7 Days of Code — Prompt Engineering (Alura)

Reto **#7DaysOfCode** de Prompt Engineering de [Alura Latam](https://www.alura.com.br/), por Fabrício Carraro.
Una técnica por día durante 7 días; cada desafío es una pieza del proyecto final: un **Tutor Personal de Carrera Tech**, un mega-prompt a la medida que analiza mi momento y arma mi plan de estudios.

**Autor:** Jesús Armando Tapia Gallegos — [@atapia9](https://github.com/atapia9)

---

## Progreso

| Día | Técnica | Estado |
|---|---|---|
| [1](./dia-01) | Estructura **PTC**: Papel · Tarea · Contexto | ✅ Completado |
| [2](./dia-02) | **Role Prompting**: persona en 4 capas (identidad · tono · método · límites) | ✅ Completado |
| [3](./dia-03) | **Zero-shot y Few-shot**: enseñar el formato con ejemplos | ✅ Completado |
| 4 | — | ⏳ |
| 5 | — | ⏳ |
| 6 | — | ⏳ |
| 7 | Mega-Prompt: Tutor Personal de Carrera Tech | ⏳ |

---

## Día 1 — Papel, Tarea y Contexto

Un buen prompt tiene tres partes:

- **P — Papel:** quién debe ser la IA. Ajusta nivel técnico, vocabulario y tono.
- **T — Tarea:** qué hay que hacer exactamente, con verbos de comando y cantidades.
- **C — Contexto:** el escenario. Quién soy, de dónde parto, qué restricciones tengo.

Archivos:

- [`perfil-base-contexto.md`](./dia-01/perfil-base-contexto.md) — mi **Perfil Base de Contexto**, el bloque que se reutiliza los 7 días.
- [`prompt-ptc.md`](./dia-01/prompt-ptc.md) — el prompt completo del Día 1.
- [`salida-prompt-ptc.md`](./dia-01/salida-prompt-ptc.md) — el diagnóstico obtenido.
- [`salida-prompt-corto.md`](./dia-01/salida-prompt-corto.md) — la respuesta al prompt vago, para comparar.
- [`comparacion.md`](./dia-01/comparacion.md) — comparación lado a lado y aprendizajes.
- [`mi_oferta.md`](./dia-01/mi_oferta.md) — documento maestro de oferta: la acción de 30 minutos que pidió el diagnóstico, convertida en hipótesis comercial v1.0 y en el eje de los Días 2 a 7.

**Conclusión del día:** el contexto vago genera respuestas vagas. La diferencia entre las dos salidas no vino de un modelo distinto, sino de nueve palabras contra trescientas treinta.

---

## Día 2 — Role Prompting

Un papel de una línea ("orientador de carrera") ya mejora la respuesta, pero deja todo lo demás en manos del modelo. Role Prompting describe a la persona en cuatro capas:

- **Identidad y experiencia:** el repertorio del que la IA va a tirar.
- **Tono de voz:** cómo llega el mensaje.
- **Método:** cómo razona y en qué orden.
- **Límites:** lo que NO hace. Es la capa que más cambia el resultado y la que casi nadie escribe.

Archivos:

- [`persona-mentora.md`](./dia-02/persona-mentora.md) — la persona de Renata Salas, activo reutilizable para los días 3 a 7.
- [`prompt-role.md`](./dia-02/prompt-role.md) — el prompt completo del Día 2.
- [`salida-plan-mentora.md`](./dia-02/salida-plan-mentora.md) — 3 hard skills priorizadas y 2 soft skills con acción de entrenamiento.
- [`salida-persona-comprador.md`](./dia-02/salida-persona-comprador.md) — el mismo prompt visto por un comprador escéptico.
- [`comparacion-personas.md`](./dia-02/comparacion-personas.md) — qué cambió al cambiar de persona y por qué.

**Conclusión del día:** la persona no es decoración, es un sesgo elegido. La mentora ni siquiera mencionó la seguridad de la información; el comprador la puso en primer lugar.

---

## Día 3 — Zero-shot y Few-shot

Pedir una respuesta "organizada" deja que el modelo decida qué significa eso. **Zero-shot** es describir la tarea con palabras; **few-shot** es mostrar de 2 a 4 pares de entrada y salida para que la IA copie el patrón. Se usa cuando lo que importa es la consistencia: misma estructura, misma extensión, mismo nivel de detalle, siempre.

Dos reglas: bastan de 2 a 4 ejemplos, y deben ser de **temas distintos al tuyo** — si son de tu mismo tema, la IA copia el contenido en vez del formato.

Archivos:

- [`formato-plan-semanal.md`](./dia-03/formato-plan-semanal.md) — la plantilla de nueve líneas y los dos ejemplos. Activo reutilizable para los días 4 a 7.
- [`prompt-fewshot.md`](./dia-03/prompt-fewshot.md) — el prompt completo del Día 3.
- [`salida-semana-01.md`](./dia-03/salida-semana-01.md) — mi Semana 1 sobre la prioridad 1 de hard skills del Día 2.
- [`zeroshot-vs-fewshot.md`](./dia-03/zeroshot-vs-fewshot.md) — la misma petición sin ejemplos, y los tres defectos que aparecieron.

**Conclusión del día:** un ejemplo vale más que una prohibición. La persona tenía escrito "no aceptas *investigar* como acción" y el zero-shot igual abrió con un día de comparar herramientas; los ejemplos, que simplemente no contienen días así, lo eliminaron sin decirlo.

---

## Licencia

Este repositorio está bajo [Creative Commons Atribución 4.0 Internacional (CC BY 4.0)](./LICENSE).

Puedes copiar, adaptar y reutilizar el contenido —incluido su uso como material de clase— siempre que des crédito. Atribución sugerida:

> Jesús Armando Tapia Gallegos, *7 Days of Code — Prompt Engineering* (2026). https://github.com/atapia9/7DaysOfCode-Prompt-Engineering — CC BY 4.0

---

`#7DaysOfCode` `#PromptEngineering` `#AluraLatam`
