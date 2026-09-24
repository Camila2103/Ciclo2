# Instrucciones para Claude — Repo Estadística 1

Este repositorio contiene el material del curso de Estadística 1 (universidad).
El objetivo es que Claude use este material para resolver tareas y prácticas,
generar resúmenes, crear preguntas tipo y exámenes de prueba, siempre alineado
con lo que se ha visto en clase.

## Regla de actualización (IMPORTANTE)

No leas el repo por iniciativa propia al empezar una conversación. Solo
accede a él cuando el usuario lo pida explícitamente. Cuando lo pidan,
trae los archivos desde cero en ese momento — no reutilices lecturas de
conversaciones anteriores, incluso si son sobre el mismo tema.

## Estructura del repo

- `STATUS.md` → en qué unidad va el curso, qué está pendiente
- `SYLLABUS.md` → temario oficial completo del curso
- `formulario.md` → notación y fórmulas oficiales que usa el profesor
- `clases/unidad-XX.md` → apuntes de cada unidad (uno por archivo)
- `libros/` → PDFs de los libros de texto
- `tareas/tarea-XX.md` → cada archivo contiene enunciado + solución + notas
- `practicas/practica-XX.md` → mismo formato que tareas
- `generado/resumenes/`, `generado/examenes/`, `generado/preguntas/` →
  contenido que tú (Claude) generas

## Cómo trabajar

1. **Antes de resolver algo**, revisa `formulario.md` y el apunte de la unidad
   correspondiente en `clases/`. No uses notación distinta a la del formulario.
2. **No uses métodos ni temas que no aparezcan aún cubiertos según STATUS.md**,
   aunque técnicamente pertenezcan al temario de SYLLABUS.md — el curso avanza
   progresivamente y las soluciones deben usar solo lo ya visto.
3. **Muestra el procedimiento paso a paso**, no solo el resultado final. Es
   material de estudio, no solo una respuesta.
4. **Al resolver una tarea o práctica**, escribe la solución dentro del mismo
   archivo (`tarea-XX.md` o `practica-XX.md`), debajo del enunciado, en una
   sección `## Solución`. No crees archivos nuevos para esto.
5. **Al generar resúmenes, exámenes o bancos de preguntas**, guárdalos en la
   subcarpeta correspondiente dentro de `generado/`, y dime el nombre de
   archivo sugerido para que yo lo confirme antes de crearlo.
6. Si un enunciado de tarea/práctica hace referencia a una unidad que no está
   documentada todavía en `clases/`, avísame en vez de asumir el contenido.

## Formato de tareas y prácticas

Cada archivo de tarea o práctica sigue esta estructura interna:

```markdown
# Tarea 01

## Enunciado
...

## Solución
...

## Notas / dudas
...
```

## Estilo de respuesta

- Explicaciones claras, a nivel de estudiante universitario que está
  aprendiendo el tema por primera vez.
- Usa LaTeX inline o en bloque para fórmulas cuando el formato lo soporte.
- Si hay varias formas de resolver un problema, prioriza el método que
  aparece en `formulario.md` o en los apuntes de clase, y menciona
  brevemente si existe una alternativa.
