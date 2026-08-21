# Auditoría y actualización de la agenda HTML

## Síntesis ejecutiva

Se comparó la planilla actualizada **CongresoREPORT2026-ok.xlsx** con la versión publicada en [REPORT 2026 | Programa, tarifas y contactos](https://condegraphics.github.io/report-2026-landing/). La página ya reflejaba la mayor parte de la agenda, pero presentaba **tres omisiones o desactualizaciones de contenido**: no mostraba el bloque “Libre” de Sala 2 del martes, no mostraba la actividad de Sala 1 del miércoles entre las 12:00 y las 13:00 y había omitido la condición arancelada del almuerzo de la industria. También incluía una nota pública que indicaba que no había actividad en ese horario del miércoles; esa nota quedó obsoleta y fue eliminada. La copia local del proyecto fue actualizada y validada sin modificar el sitio publicado ni realizar un push a GitHub.

## Alcance de la revisión

| Elemento | Resultado |
|---|---|
| Marca y canal | REPORT 2026, landing HTML en GitHub Pages |
| Fuente principal | Planilla entregada: `CongresoREPORT2026-ok.xlsx`, hoja `Copia de TecCom PM` |
| Fuente comparada | Repositorio `condegraphics/report-2026-landing`, rama `main` |
| Jornadas verificadas | Martes 1, miércoles 2 y jueves 3 de septiembre de 2026 |
| Salas verificadas | Sala 1 y Sala 2 para cada jornada |
| Actividades con horario | 41 en la planilla y 41 en la versión actualizada |
| Estado | **Cambio preparado y validado; no publicado** |

## Cambios realizados

| Prioridad | Ubicación | Situación detectada | Corrección aplicada |
|---|---|---|---|
| Alta | Martes 1 · Sala 2 · 13:00–14:30 | La planilla consignaba `Libre`, pero la landing no mostraba ese bloque. | Se agregó el bloque horario con la etiqueta **Libre** y estilo de intervalo. |
| Alta | Miércoles 2 · Sala 1 · 12:00–13:00 | La planilla repetía `Problemas Microbianos en Fábrica de Pinturas — F. Rossi (Surfactan)`; la landing omitía el segundo bloque. | Se agregó la actividad exactamente como figura en la fuente, sin corregirla por intuición. |
| Media | Martes 1 · Sala 1 · 13:00–14:30 | La landing mostraba el almuerzo, pero no indicaba que era una actividad arancelada. | Se incorporó `Actividad arancelada · junto a los auditorios.` |
| Media | Miércoles 2 · Sala 1 | La landing informaba que no había una actividad consignada entre 12:00 y 13:00. | Se eliminó la nota porque quedó contradicha por la planilla actualizada. |

## Interpretación de las diferencias

La diferencia más relevante es la incorporación de **dos bloques horarios que modifican la lectura operativa de la agenda**: una franja libre en Sala 2 durante el martes y una segunda actividad de Sala 1 durante el miércoles. La repetición de “Problemas Microbianos en Fábrica de Pinturas” entre las 11:00–12:00 y las 12:00–13:00 puede ser intencional o un duplicado de la planilla. Como la instrucción recibida fue trabajar sobre el listado actualizado y no existe una confirmación oficial alternativa en los materiales revisados, se conservó literalmente en la web, dejando señalada la necesidad de confirmación editorial por parte de ATIPAT antes de una publicación definitiva.

La planilla contiene además el texto **“Tercer día del Congreso Técnico - Jueves 1 de Septiembre”**, que contradice las fechas generales del evento y el calendario: el 1 de septiembre de 2026 corresponde a martes y el jueves es 3 de septiembre. La landing ya utilizaba “Jueves 3 de septiembre”, por lo que esa redacción se mantuvo. Se considera una corrección tipográfica evidente, pero conviene confirmarla con ATIPAT antes de publicar si el archivo XLSX se vuelve a distribuir como documento oficial.

## Validaciones técnicas

| Control | Resultado |
|---|---:|
| `<!doctype html>` | OK |
| `html lang="es"` | OK |
| Meta description y título | OK |
| Tres jornadas | OK |
| Seis salas | OK |
| 41 bloques con horario | OK |
| Bloque “Libre” del martes incorporado | OK |
| Actividad de miércoles 12:00–13:00 incorporada | OK |
| Condición arancelada del almuerzo visible | OK |
| Nota obsoleta eliminada | OK |
| Grilla de salas a una columna en mobile | OK |
| Vista previa visual de la agenda | OK |

## Archivos entregados

El archivo principal es `index.html`, listo para reemplazar el archivo equivalente del repositorio mediante una revisión humana. También se entrega un ZIP con el proyecto completo y una captura de la vista previa de la agenda. La versión fue preparada sobre una copia local; **no se modificó la rama `main`, no se creó un Pull Request y no se publicó en GitHub Pages**, respetando la regla de aprobación previa para cambios externos.

## Aprobación requerida

Antes de publicar, solicitar a ATIPAT confirmación de dos puntos: si la repetición de “Problemas Microbianos en Fábrica de Pinturas” en las dos franjas consecutivas del miércoles es correcta y si el encabezado del tercer día debe decir “Jueves 3 de septiembre”. Con esa confirmación, el archivo queda listo para subir mediante una rama y Pull Request.

## Referencias

[1]: https://condegraphics.github.io/report-2026-landing/ "Landing publicada de REPORT 2026"
[2]: https://recrecubrimientos.com/el-report-que-viene/ "REC Recubrimientos: Todo lo que hay que saber de REPORT"
[3]: https://pinturasynegocios.com.ar/report-2026-leer-el-presente-para-anticipar-el-futuro/ "Pinturas y Negocios: REPORT 2026"
