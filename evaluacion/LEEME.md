# Evaluación de la clasificación

Mide cómo clasifica el Flujo 1 (tipo y prioridad) incidencias cuyo resultado esperado se fijó **antes** de ejecutarlas, a partir de los criterios de la [base documental](../base-documental/).

| Archivo | Contenido |
|---|---|
| `Evaluacion_Clasificacion_AudioVital_v1_v2.xlsx` | 30 casos: resultados de la v2, hoja **Comparativa** v1 → v2 y **Resumen** con matrices de confusión |
| `Validacion_Clasificacion_AudioVital_resultados.xlsx` | 15 casos nuevos, no usados para ajustar el prompt: la cifra no sesgada |
| `eval_importar_incidencias.csv` | Las 30 descripciones, listas para *Importar desde CSV* en Dataverse |
| `val_importar_incidencias.csv` | Las 15 descripciones de validación |

## Resultados

| Pasada | Acierto estricto | Escalados perdidos |
|---|---|---|
| v1 (30 casos) | 27/30 (90 %) | 1 |
| v2 (mismos 30, tras corregir) | 29/30 · 0 regresiones | 0 |
| **Validación (15 nuevos)** | **12/15 (80 %)** | **0** |

Los casos se clasifican en *claros*, *de frontera* y *ambiguos*. Los dos últimos admiten una alternativa aceptable, y se mide el acierto estricto y el acierto con alternativas.

**Límite:** el resultado de la v2 es optimista, porque las reglas añadidas se escribieron viendo esos casos. La cifra a citar es la de la validación.
