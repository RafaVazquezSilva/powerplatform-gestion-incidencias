# Documentación

## Proyecto completo — Fases 1, 2 y 3

`Proyecto_Completo_Gestion_Incidencias_PowerPlatform_IA.pdf` — 49 páginas. Portada común, presentación del proyecto, índice general con marcadores y las dos memorias técnicas siguientes, sin cambios en su contenido.

## Memoria técnica — Fases 1 y 2

Documento de 21 páginas: solución base, evolución a la Fase 2, arquitectura, Dataverse, flujos, prompts y expresiones, base documental, **Azure AI Search y asistente con RAG**, clasificación robusta, evaluación (v1, v2 y validación independiente), incidente de la cuota semántica agotada, problemas resueltos y límites conocidos.

- `Memoria_Tecnica_Gestion_Incidencias_Fases1y2.pdf` — lectura y descarga
- `Memoria_Tecnica_Gestion_Incidencias_Fases1y2.docx` — editable

## Memoria técnica — Fase 3: operación y gobierno

Documento de 25 páginas:

- Modelo de uso: roles y responsabilidades
- Arquitectura final con los cuatro flujos
- **Azure Key Vault, entidad de servicio y RBAC** de mínimo privilegio
- **Observabilidad y coste:** métricas, presupuesto con alertas y diagnósticos en Log Analytics (KQL)
- Incidente del bucle de autodisparo y errores 429, diagnosticado y corregido
- Ciclo de vida de la incidencia: autor, propietario, estados y resolución
- Flujo 3 (cierre con resolución obligatoria) y Flujo 4 (asignación «Me encargo» con tarjeta adaptable)
- Lo que no se construyó, límites conocidos y **hoja de ruta para llevarlo a producción**

Archivo: `Memoria_Tecnica_Fase3_Operacion_y_Gobierno.pdf`

## Nota sobre la memoria original de la Fase 1

La memoria original de 16 páginas (solo Fase 1) queda sustituida por la de las Fases 1 y 2. Aquella afirmaba que la rama de escalado cambiaba el Estado a *Escalada*; la Fase 2 demostró que no era así y lo corrigió.
