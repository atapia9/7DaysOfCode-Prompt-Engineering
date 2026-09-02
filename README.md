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
| [4](./dia-04) | **Chain of Thought**: razonamiento por pasos definidos | ✅ Completado |
| [5](./dia-05) | **Delimitadores y restricciones**: separar instrucciones de datos | ✅ Completado |
| [6](./dia-06) | **Inyección de contexto largo**: fuentes etiquetadas y trazabilidad | ✅ Completado |
| [7](./dia-07) | **Composición**: Mega-Prompt — Tutor Personal de Carrera Tech | ✅ Completado |

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

## Día 4 — Chain of Thought

Ante una decisión con renuncia de por medio, la IA responde rápido, con seguridad y sin mostrar nada de su razonamiento. **Chain of Thought** es pedirle que exponga los pasos antes de concluir: descompone el problema, evalúa cada parte y solo entonces cierra una posición. Sirve para dos cosas: reduce conclusiones apresuradas, y deja una superficie que se puede auditar paso por paso.

"Piensa paso a paso" funciona; definir **cuáles** son los pasos funciona mucho mejor, porque ahí eliges tú los criterios que entran en la decisión.

Archivos:

- [`secuencia-cot.md`](./dia-04/secuencia-cot.md) — mi secuencia de seis pasos y por qué cambié dos criterios del ejemplo. Activo reutilizable.
- [`prompt-cot.md`](./dia-04/prompt-cot.md) — el prompt completo del Día 4.
- [`salida-cot.md`](./dia-04/salida-cot.md) — los seis bloques de razonamiento sobre un dilema real del proyecto.
- [`con-y-sin-cot.md`](./dia-04/con-y-sin-cot.md) — el mismo dilema sin pedir razonamiento, y qué escondía esa respuesta.

**Conclusión del día:** el paso 4 —"qué información me falta"— es el que paga el ejercicio. Reveló que estaba a punto de reordenar mi plan con base en una objeción que ninguna persona real me ha dicho todavía.

---

## Día 5 — Delimitadores y restricciones

**Delimitadores** (comillas triples, `---`, etiquetas) marcan dónde terminan mis instrucciones y empiezan mis datos: lo que va dentro es material a procesar, no una orden a obedecer. **Restricciones** son las reglas del juego, en tres clases: de formato, de extensión y negativas. Las negativas son las que más tiempo ahorran.

Archivos:

- [`bloque-reglas.md`](./dia-05/bloque-reglas.md) — el bloque de reglas y la regla anti-inyección que agregué. Activo reutilizable.
- [`prompt-extraccion.md`](./dia-05/prompt-extraccion.md) — el prompt completo del Día 5, sobre el temario real del curso "Git y GitHub" de REDEC-UNAM/FESC.
- [`salida-cronograma.md`](./dia-05/salida-cronograma.md) — la tabla, y nada más.
- [`sin-reglas-y-prueba-inyeccion.md`](./dia-05/sin-reglas-y-prueba-inyeccion.md) — la misma petición sin reglas negativas, y qué pasa cuando el texto pegado trae una orden escondida.

**Conclusión del día:** delimitar no es prolijidad, es decidir qué parte del texto tiene permiso de darme órdenes. Y "no informado" también es información: cinco celdas vacías me revelaron que mi propio temario no declara entregables por sesión, mientras la rúbrica califica 40% por ellos.

---

## Día 6 — Inyección de contexto largo

Los modelos aguantan textos extensos, pero su atención no es uniforme: lo que queda en medio de un bloque grande tiende a diluirse. Tres prácticas lo corrigen: **etiquetar cada fuente** en bloques con nombre, **poner la instrucción después de los datos** (y repetirla), y **exigir trazabilidad** — que cada conclusión cite el fragmento que la sostiene.

Archivos:

- [`vacante-objetivo.md`](./dia-06/vacante-objetivo.md) — la fuente: una vacante real de Change Consultant / AI Trainer, freelance y remota.
- [`prompt-gaps.md`](./dia-06/prompt-gaps.md) — el prompt completo del Día 6, con tres bloques etiquetados.
- [`reporte-gaps.md`](./dia-06/reporte-gaps.md) — el reporte: qué ya tengo, qué me bloquea y qué es bonus. Última pieza del Día 7.
- [`aprendizajes-contexto-largo.md`](./dia-06/aprendizajes-contexto-largo.md) — los dos errores que aparecieron sin etiquetas y cómo se corrigieron.

**Conclusión del día:** pedir la cita no mejora la redacción, cambia lo que la IA se atreve a afirmar. Sin etiquetas, un plan futuro del Día 2 apareció citado como capacidad presente; con las fuentes separadas por valor probatorio, ese error desapareció solo.

---

## Día 7 — Composición: el Mega-Prompt

Un mega-prompt es un prompt en capas, donde cada bloque cumple una función distinta y no pelea con los demás. El orden importa: **persona → contexto → base de conocimiento → razonamiento → patrón de salida → restricciones → tarea**. La tarea va al final para que sea lo último que el modelo lee.

Las seis piezas de los días 1 a 6 se ensamblan aquí en una sola herramienta reutilizable. Cuando algo cambia, se actualiza un bloque, no todo el prompt.

Archivos:

- [`tutor-v1.md`](./dia-07/tutor-v1.md) — **el Mega-Prompt completo**, autocontenido y listo para copiar y pegar.
- [`pdi-30-dias.md`](./dia-07/pdi-30-dias.md) — la salida: mi Plan de Desarrollo Individual de 30 días, con cuatro semanas ejecutables y cada bloque ligado a un gap real.
- [`notas-de-version.md`](./dia-07/notas-de-version.md) — qué bloque tocar cuando algo cambie, la bitácora de versiones, los siete aprendizajes del reto y lo que este tutor **no** hace.

**Conclusión del día:** lo primero que hizo el Tutor fue avisarme que mi tiempo no alcanza para la vacante que elegí, antes de presentar el plan. Un tutor que solo dice que sí no es un tutor: es un generador de listas.

---

## Cierre del reto

Siete días, siete técnicas, y un repositorio que dejó de ser un ejercicio de estudio para volverse el proyecto: diagnóstico, oferta con precio, plan de estudio, política de datos y el primer caso público. Las técnicas se aprenden aplicándolas a algo que importa.

---

## Licencia

Este repositorio está bajo [Creative Commons Atribución 4.0 Internacional (CC BY 4.0)](./LICENSE).

Puedes copiar, adaptar y reutilizar el contenido —incluido su uso como material de clase— siempre que des crédito. Atribución sugerida:

> Jesús Armando Tapia Gallegos, *7 Days of Code — Prompt Engineering* (2026). https://github.com/atapia9/7DaysOfCode-Prompt-Engineering — CC BY 4.0

---

`#7DaysOfCode` `#PromptEngineering` `#AluraLatam`
