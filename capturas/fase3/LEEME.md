# Capturas de la Fase 3 — Operación y gobierno

45 capturas tomadas en el entorno real. Todas están recortadas sin pestañas, marcadores ni datos de la cuenta, y los correos que aparecían en pantalla están tachados. No aparece ningún secreto.

## Seguridad: Key Vault, entidad de servicio y RBAC

| Nº | Archivo | Contenido |
|---|---|---|
| 17 | `17_entra_app_registro.png` | Registro de aplicación `app-audiovital-flujos` en Entra ID |
| 18 | `18_keyvault_configuracion.png` | Creación del Key Vault: plan Estándar, modelo de permisos RBAC, retención de 7 días |
| 19 | `19_keyvault_rbac.png` | Roles: el autor gestiona secretos y la aplicación solo los lee |
| 20 | `20_search_claves_consulta.png` | Claves de Azure AI Search, ocultas; se usa la de consulta |
| 21 | `21_keyvault_secreto.png` | Secreto `search-query-key` creado |
| 22 | `22_flujo2_conexion_keyvault.png` | Conexión con autenticación de entidad de servicio, secreto oculto |
| 23 | `23_flujo2_http_secreto_keyvault.png` | Cabecera `api-key` = valor del secreto |
| 24 | `24_conexiones_keyvault_conectada.png` | Conexiones en verde |
| 25 | `25_flujo2_ejecucion_keyvault.png` | Ejecución correcta con «Obtener secreto» |
| 26 | `26_teams_respuesta_tras_keyvault.png` | El asistente responde con la clave leída de Key Vault |
| 28 | `28_flujo2_salidas_seguras.png` | Entradas y salidas seguras: el secreto no aparece en el historial |

## Incidente: errores 429 y bucle de autodisparo del Flujo 2

| Nº | Archivo | Contenido |
|---|---|---|
| 27 | `27_flujo2_openai_5min.png` | El paso de Azure OpenAI tarda 5 min 6 s |
| 29 | `29_flujo2_reintento_429.png` | El paso de Azure OpenAI con un reintento tras el 429 |
| 30 | `30_openai_limite_tpm.png` | Límites del despliegue: 100.000 TPM y 100 RPM (modelo Legacy) |
| 31 | `31_bucle_from_bot_workflows.png` | El mensaje que dispara el flujo lo envía el bot Workflows (`from.user = null`) |
| 32 | `32_flujo2_condicion_antibucle.png` | Condición antibucle → Finalizar |
| 33 | `33_historial_bucle_cortado.png` | Historial tras la corrección: sin ejecuciones fantasma |
| 34 | `34_teams_respuesta_unica.png` | Una sola respuesta por pregunta |
| 35 | `35_flujo2_enumerar_filas_filtrado.png` | Enumerar filas: 12 columnas, orden por fecha y 50 filas |
| 36 | `36_enumerar_filas_48KB.png` | Respuesta reducida a 48.387 bytes (−80 %) |
| 37 | `37_teams_respuesta_filtrada.png` | Respuesta con la lista de incidencias recientes |
| 38 | `38_teams_agente_creadopor.png` | El asistente identifica al autor real («Usuario 747») |

## Observabilidad y control de costes

| Nº | Archivo | Contenido |
|---|---|---|
| 39 | `39_costes_por_recurso.png` | Coste de octubre por recurso: 19,55 €, casi todo Azure OpenAI |
| 40 | `40_metricas_tokens_bucle.png` | Tokens procesados: 36,53 M en 24 h, meseta del bucle y caída |
| 41 | `41_presupuesto_creado.png` | Presupuesto de 25 €/mes con alertas |
| 42 | `42_diagnostico_openai_loganalytics.png` | Diagnóstico `diag-openai` hacia Log Analytics |
| 43 | `43_loganalytics_llamadas.png` | Consulta KQL: embeddings y chat completions, código 200 |

## Ciclo de vida de la incidencia

| Nº | Archivo | Contenido |
|---|---|---|
| 44 | `44_formulario_resolucion.png` | Formulario con Autor (solo lectura) y Resolución |
| 45 | `45_app_ficha_autor_resolucion.png` | Ficha de INC-0086 en la app |
| 54 | `54_flujo1_fecha_alta.png` | Flujo 1: Fecha_Alta escrita a partir de la fecha de creación |
| 55 | `55_INC0087_fecha_alta_automatica.png` | Incidencia nueva con Fecha_Alta automática y clasificación de la IA |

## Flujo 3 — Cierre con resolución obligatoria

| Nº | Archivo | Contenido |
|---|---|---|
| 46 | `46_flujo3_mensaje_teams.png` | Aviso de Teams al autor con código y resolución |
| 47 | `47_flujo3_historial_prueba1.png` | Primera prueba correcta |
| 48 | `48_flujo3_ejecucion_sin_resolucion.png` | Sin resolución: la condición devuelve la incidencia a En curso |
| 49 | `49_ficha_vuelve_en_curso.png` | INC-0086 vuelve a En curso |
| 50 | `50_flujo3_historial_dos_ejecuciones.png` | Dos ejecuciones correctas |
| 51 | `51_flujo3_ejecucion_con_resolucion.png` | Con resolución: Fecha_Cierre, lectura del autor y aviso |
| 52 | `52_teams_aviso_escalado_y_cierre_INC0086.png` | Ciclo completo en Teams: escalado y cierre |
| 53 | `53_ficha_cerrada_fecha_resolucion.png` | Ficha cerrada con fecha y resolución |

## Flujo 4 — Asignación «Me encargo»

| Nº | Archivo | Contenido |
|---|---|---|
| 56 | `56_flujo4_actualizar_propietario.png` | Actualizar una fila: Estado En curso y Propietario |
| 57 | `57_teams_tarjeta_me_encargo.png` | Tarjeta adaptable con el botón «Me encargo» |
| 58 | `58_teams_tarjeta_asignada.png` | Tarjeta sustituida por «Asignada. Gestión en curso» |
| 59 | `59_flujo4_error_systemusers_vacio.png` | Error diagnosticado: la búsqueda por correo no encontraba al usuario |
| 60 | `60_flujo4_ejecucion_correcta.png` | Ejecución correcta tras buscar por UPN |
| 61 | `61_INC0087_en_curso_tras_me_encargo.png` | INC-0087 pasa de Escalada a En curso |
