# Capturas de la Fase 2

Evidencias del entorno real. Recortadas para no mostrar pestañas ni marcadores del navegador; la clave de API aparece tapada en `09a`.

| Archivo | Contenido |
|---|---|
| `01_recursos_azure.png` | Recursos de la Fase 2 en el grupo `rg-incidencias-audiovital` |
| `02_storage_contenedor.png` | Contenedor `base-documental` con los 6 PDFs |
| `02b_storage_overview_LRS.png` | Cuenta de almacenamiento con redundancia local (LRS) |
| `03_search_overview_plan_gratis.png` | Servicio Azure AI Search en plan Gratis |
| `04_indice_audiovital_rag.png` | Índice: 11 fragmentos, 248 KB, 200 KB de vectores |
| `05_configuracion_semantica.png` | Configuración semántica (`title` / `chunk`) |
| `06a_busqueda_semantica_original.png` | Búsqueda semántica: protocolo de escalado en primer lugar (0,979) |
| `06b_cuota_semantica_agotada.png` | Error de cuota semántica agotada |
| `06c_opciones_consulta.png` | Opciones de consulta sin clasificador semántico |
| `06d_busqueda_hibrida_resultados.png` | Resultados de la búsqueda híbrida |
| `06e_busqueda_hibrida_escalado_7o.png` | Protocolo de escalado en séptima posición sin reordenación |
| `07_indexacion_creada.png` | Creación del índice completada |
| `07b_indexador_historial.png` | Indexador: 6 documentos, 0 errores |
| `08_implementaciones_modelos.png` | Modelos desplegados: `gpt-4.1-mini` y `text-embedding-3-small` |
| `08b_openai_overview.png` | Recurso de Azure OpenAI |
| `09a_flujo2_http_headers.png` | Flujo 2: cabeceras del paso HTTP (clave tapada) |
| `09b_flujo2_http_body_hibrido.png` | Flujo 2: cuerpo de la búsqueda híbrida |
| `10_flujo1_rama_error.png` | Flujo 1: configuración "Ejecutar después de" de la rama de error |
| `10b_flujo1_vista_general.png` | Flujo 1 completo |
| `11_flujo1_estado_expresion.png` | Expresión que escribe el Estado |
| `12a_flujo1_temperatura.png` | Temperatura 0 |
| `12b_flujo1_json_object.png` | `response_format = json_object` |
| `13_teams_respuesta_rag.png` | Respuesta fundamentada en el protocolo de escalado |
| `13b_teams_respuesta_rag_hibrida.png` | Respuesta tras pasar a búsqueda híbrida |
| `13c_teams_garantia.png` | Pregunta sobre garantías |
| `13d_teams_cambio_cita.png` | Pregunta sobre cambio de cita |
| `14_teams_pregunta_sin_respuesta.png` | Pregunta sin respaldo documental: el asistente no inventa |
| `15_teams_aviso_fallo.png` | Aviso de clasificación fallida (prueba de fallo forzado) |
| `16_dataverse_escaladas.png` | Incidencias Alta con Estado *Escalada* |
