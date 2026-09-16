<div align="center">

<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />

  <h1>Built with AI Studio</h2>

  <p>The fastest path from prompt to production with Gemini.</p>

  <a href="https://aistudio.google.com/apps">Start building</a>

</div>

## Prioridades y métricas

### Prioridad de funcionalidades

- **P1 - Clientes:** crear, editar y consultar clientes con nombre completo, documento/identificación, teléfono, email y domicilio; no se acepta guardar clientes sin nombre ni al menos un dato de contacto.
- **P1 - Expedientes:** crear expedientes vinculados a un cliente, con carátula/asunto, número interno, estado, responsable y fecha de alta; el listado debe permitir filtrar por cliente, estado y responsable.
- **P1 - Audiencias:** registrar audiencias con expediente asociado, fecha, hora, lugar/modalidad y responsable; el sistema debe mostrar avisos de audiencias próximas dentro de los siguientes 7 días.
- **P2 - Documentos:** adjuntar o registrar documentos por expediente con tipo, fecha, descripción y responsable de carga; cada documento debe quedar visible desde la ficha del expediente.
- **P2 - Tareas:** crear tareas asociadas a clientes o expedientes con responsable, fecha límite, estado y prioridad; el sistema debe distinguir tareas pendientes, completadas y vencidas.
- **P3 - Mejoras posteriores:** tableros avanzados, reportes exportables, automatizaciones y permisos granulares quedan fuera del MVP salvo que bloqueen la operación diaria validada con usuarios.

### Métricas iniciales medibles

- **Tiempo de alta de expediente:** medir desde el clic en “Nuevo expediente” hasta el guardado exitoso; meta MVP: el 80% de las altas completas se realizan en **menos de 3 minutos** durante pruebas con usuarios.
- **Cumplimiento de plazos:** porcentaje de audiencias y tareas con fecha límite revisadas antes de su vencimiento; meta MVP: al menos **90%** de eventos críticos aparecen en la vista de próximos vencimientos.
- **Tareas vencidas:** cantidad de tareas con fecha límite pasada y estado distinto de completada; meta MVP: el listado de tareas vencidas coincide con una revisión manual en **10 de 10 casos de prueba**.

### Criterios de aceptación del MVP

- Un abogado o auxiliar puede registrar un cliente y crear un expediente asociado sin asistencia técnica en una prueba supervisada.
- Cada expediente muestra cliente, estado, responsable, audiencias, documentos y tareas relacionadas desde una misma vista o flujo de navegación documentado.
- El sistema permite identificar en menos de 30 segundos las audiencias de los próximos 7 días y las tareas vencidas.
- Los campos obligatorios impiden guardar registros incompletos para clientes, expedientes, audiencias y tareas.
- Una carga de prueba con al menos 20 clientes, 30 expedientes, 15 audiencias, 25 documentos y 40 tareas se consulta sin errores funcionales bloqueantes.
- La primera versión se declara usable solo si no quedan defectos P1 abiertos relacionados con pérdida de datos, imposibilidad de crear expedientes o fallas al listar vencimientos.

### Checklist de validación con usuarios

- [ ] **Abogados:** confirmar que los datos obligatorios del expediente coinciden con la información usada en la práctica diaria.
- [ ] **Abogados:** crear 3 expedientes reales o simulados y registrar el tiempo de alta de cada uno.
- [ ] **Auxiliares:** cargar 5 documentos en expedientes distintos y verificar que cada documento pueda recuperarse desde la ficha correcta.
- [ ] **Auxiliares:** crear 5 tareas con distintas fechas límite y validar que las vencidas aparezcan en el listado correspondiente.
- [ ] **Abogados y auxiliares:** revisar la vista de audiencias próximas y confirmar que no falten eventos de los próximos 7 días.
- [ ] **Equipo de producto:** registrar observaciones con severidad P1/P2/P3 y convertir las P1 en correcciones obligatorias antes de la siguiente iteración.
