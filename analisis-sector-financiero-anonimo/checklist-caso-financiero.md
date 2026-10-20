# Checklist Aplicado — Caso Sector Financiero (Anónimo)

> Aplicación práctica del [checklist de auditoría ISO 27001](../plantillas-politicas-seguridad/checklist-auditoria-iso27001.md)
> al caso de estudio de institución financiera en transformación digital.

**Metodología:** Los hallazgos provienen del análisis documental del caso.
La evaluación se basa en la información descrita en el escenario, no en
una auditoría de campo real.

---

## Resultados de la Evaluación

### Controles de Gobierno de TI

| Control 2013 | Equiv. 2022 | Pregunta de Auditoría | Resultado | Justificación (del caso) |
|---|---|---|---|---|
| A.5.1.1 | 5.1 | ¿Existe política de seguridad aprobada y revisada por la dirección? | P | Existen políticas actualizadas, pero no hay comité formal de gobierno de TI reportando a la Junta |
| A.6.1.1 | 5.2 | ¿Existen roles de seguridad formalmente asignados y reportando al nivel directivo? | P | El Director de Seguridad existe, pero Riesgos queda excluido del Comité de Proyectos (sin voz ni voto) |
| A.8.4 | 8.4 | ¿Se controla el acceso al código fuente de los sistemas? | ✗ | El sistema AUD opera sin código fuente; dependencia total del proveedor para actualizaciones |

### Controles de Proveedores y Cloud

| Control 2013 | Equiv. 2022 | Pregunta de Auditoría | Resultado | Justificación (del caso) |
|---|---|---|---|---|
| A.15.1.1 | 5.19 | ¿Existe política que regule la seguridad con terceros? | ✓ | La institución tiene políticas y procedimientos para gestión de contratos con proveedores |
| A.15.1.2 | 5.20 | ¿Los contratos incluyen SLAs verificables? | ✗ | Proveedor crítico no responde oportunamente; su infraestructura no soporta los tiempos de recuperación requeridos |
| A.15.1.3 | 5.21 | ¿Se gestiona la cadena de suministro de TIC? | P | Problema de compatibilidad entre dos proveedores contratados (sistema vs base de datos) |
| A.5.23 | 5.23 | ¿Se evalúan riesgos antes de adoptar servicios cloud? | ✗ | El equipo de seguridad decidió NO participar en la migración de datos a la nube |
| A.18.1.4 | 5.34 | ¿Se protegen los datos almacenados fuera de la jurisdicción? | P | Datos en el extranjero (Marruecos) respaldados por normativa europea alegada por el proveedor, pero sin validación independiente |

### Controles de Acceso y Desarrollo

| Control 2013 | Equiv. 2022 | Pregunta de Auditoría | Resultado | Justificación (del caso) |
|---|---|---|---|---|
| A.9.2.3 | 8.2 | ¿Los accesos privilegiados están restringidos y revisados? | ✗ | Se otorgaron permisos de administrador en servidores de prueba/desarrollo para evitar retrasos, sin control ni revisión |
| A.14.2.1 | 8.25 | ¿Se aplican controles de seguridad durante el desarrollo? | P | Existe metodología de desarrollo aprobada por la Junta, pero es empírica y sin revisión de Riesgos/Auditoría hasta producción |
| A.14.2.2 | 8.32 | ¿Los cambios siguen control formal? | ✗ | Ampliación de alcance del proyecto sin ajustar costos, tiempo ni personal |

### Controles de Auditoría y Continuidad

| Control 2013 | Equiv. 2022 | Pregunta de Auditoría | Resultado | Justificación (del caso) |
|---|---|---|---|---|
| A.17.1.1 | 5.29 | ¿Existe plan de continuidad probado y actualizado? | P | Comité de continuidad existe, pero se reúne solo una vez al año y el BCP aún no define RPO/RTO |
| A.18.2.1 | 5.35 | ¿Se realiza revisión independiente periódica? | P | Auditoría externa anual existe, pero el Jefe de Auditoría filtra hallazgos antes de presentarlos a la dirección |

---

## Resumen de Resultados

| Resultado | Cantidad | Controles (A.9.2.3, A.15.1.2, A.5.23, A.14.2.2, A.8.4, A.5.1.1, A.15.1.3, etc.) |
|-----------|----------|--------------------------------------------------|
| ✓ Cumple | 1 | A.15.1.1 |
| P Parcial | 6 | A.5.1.1, A.6.1.1, A.15.1.3, A.18.1.4, A.14.2.1, A.17.1.1, A.18.2.1 |
| ✗ No cumple | 4 | A.9.2.3, A.15.1.2, A.5.23, A.14.2.2, A.8.4 |

---

## Conclusiones por Área

### 🔴 Crítico

| Área | Brecha Principal |
|------|------------------|
| **Acceso privilegiado** | Permisos admin en dev sin control |
| **Proveedores críticos** | Sin SLA de recuperación real |
| **Cloud** | Seguridad delegada totalmente |
| **Código fuente** | Sistema legacy sin acceso |

### 🟡 Medio

| Área | Brecha Principal |
|------|------------------|
| **Gobierno de TI** | Sin comité formal |
| **Auditoría** | Hallazgos filtrados antes de presentación |
| **Continuidad** | Frecuencia anual insuficiente |

### ✅ Fortalezas

| Área | Fortaleza |
|------|-----------|
| **Políticas** | Existen y se actualizan |
| **Director de Seguridad** | Certificado y experimentado |

---

*Aplicación elaborada por Jay Romero Amaya — Octubre 2025*
*Caso anonimizado. Los hallazgos son interpretación propia del escenario proporcionado.*
