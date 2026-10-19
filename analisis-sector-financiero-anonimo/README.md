# Análisis de Cumplimiento — Sector Financiero (Caso Anónimo)

> Ejercicio profesional de evaluación de controles de seguridad, gobierno de TI y gestión de riesgos en una institución financiera en proceso de transformación digital.

---

## Contexto del Caso

- **Tipo de entidad:** Institución financiera de importancia sistémica
- **Proceso evaluado:** Migración de sistema legado hacia plataforma integral
- **Situación:** Crecimiento acelerado sin actualización proporcional de infraestructura tecnológica
- **Regulación aplicable:** Sector bancario nacional

> **Nota:** Todos los datos han sido anonimizados. No se incluye información confidencial ni identificable de ninguna institución real.

---

## Metodología Aplicada

| Marco | Propósito en el Análisis |
|-------|--------------------------|
| **ISO/IEC 27001** | Identificación de brechas en controles de seguridad |
| **NIST CSF** | Evaluación de capacidades funcionales (Identify, Protect, Detect, Respond, Recover) |
| **COBIT 2019** | Evaluación de madurez de gobierno de TI |

### Dominios Evaluados (7)

1. Gobierno de TI
2. Gestión de Proveedores
3. Seguridad de la Información
4. Auditoría
5. Gestión de Riesgos
6. Gestión de Proyectos
7. Continuidad del Negocio

---

## Hallazgos por Dominio

### 1 Gobierno de TI

| Tipo | Hallazgo | Referencia |
|------|----------|------------|
| ✅ **Fortaleza** | Apoyo explícito y documentado de la Junta Directiva al proyecto | ISO 27001 — A.5.1 |
| ✅ **Fortaleza** | Comité de administración de proyectos con reglamento aprobado | COBIT — BAI01 |
| ⚠️ **Debilidad** | Ausencia de rol o comité formal de Gobierno de TI en el organigrama | ISO 27001 — A.5.1 / A.5.2 |
| ⚠️ **Debilidad** | Gerencia de Riesgos excluida del comité de proyectos (sin voz ni voto) | ISO 27001 — A.5.3 (Segregación de funciones) |
| ⚠️ **Debilidad** | Sistema legado sin código fuente — dependencia total del proveedor | ISO 27001 — A.8.27 / A.8.4 |

**Recomendación:** Crear un comité de Gobierno de TI que reporte directamente a la Junta Directiva, con participación obligatoria de la Gerencia de Riesgos en decisiones de proyectos críticos.

---

### 2️ Gestión de Proveedores

| Tipo | Hallazgo | Referencia |
|------|----------|------------|
| ✅ **Fortaleza** | Políticas y procedimientos formales para gestión de contratos | ISO 27001 — A.5.19 |
| ⚠️ **Debilidad** | Proveedor crítico sin capacidad de recuperación en tiempos requeridos | ISO 27001 — A.5.22 |
| ⚠️ **Debilidad** | Almacenamiento de datos en servidor en el extranjero (Marruecos) | ISO 27001 — A.5.34 / A.5.23 |
| ⚠️ **Debilidad** | Incompatibilidad técnica entre dos proveedores contratados | ISO 27001 — A.5.21 |

**Recomendación:** Renegociar contratos incluyendo SLAs con penalizaciones, cláusulas de recuperación ante desastres, y requisitos de cumplimiento normativo para datos transfronterizos.

---

### 3️ Seguridad de la Información

| Tipo | Hallazgo | Referencia |
|------|----------|------------|
| ✅ **Fortaleza** | Director de Seguridad con CISSP, CISM, CEH y 15 años de experiencia | — |
| ✅ **Fortaleza** | Políticas de seguridad documentadas y actualizadas | ISO 27001 — A.5.1 |
| ⚠️ **Debilidad** | Permisos de administrador otorgados en servidores de prueba/desarrollo | ISO 27001 — A.8.2 |
| ⚠️ **Debilidad** | Equipo de seguridad NO participó en la migración de datos a la nube | ISO 27001 — A.5.23 |

**Recomendación:** Aplicar principio de menor privilegio en todos los entornos; participación obligatoria del equipo de seguridad en procesos de migración de datos.

---

### 4️ Auditoría

| Tipo | Hallazgo | Referencia |
|------|----------|------------|
| ✅ **Fortaleza** | Personal certificado (CISM, CISA) con plan de capacitación continua | — |
| ✅ **Fortaleza** | Auditoría externa anual contratada para revisión de ciberseguridad | ISO 27001 — A.5.35 |
| ⚠️ **Debilidad** | Revisión del proyecto crítico postergada hasta salida a producción | ISO 27001 — A.8.32 (Gestión de cambios) |
| ⚠️ **Debilidad** | Hallazgos filtrados por el Jefe de Auditoría antes de presentar a la Alta Dirección | ISO 27001 — A.5.35 (Independencia) |

**Recomendación:** Incorporar auditoría continua durante el ciclo de vida del proyecto, no solo post-implementación. Garantizar independencia total en el reporte de hallazgos.

---

### 5️ Gestión de Riesgos

| Tipo | Hallazgo | Referencia |
|------|----------|------------|
| ✅ **Fortaleza** | Gerencia de Riesgos constituida con línea directa a Junta Directiva | ISO 27001 — A.5.1 |
| ✅ **Fortaleza** | Oficial de riesgo tecnológico con autoridad de reporte independiente | — |
| ⚠️ **Debilidad** | Dependencia exclusiva de matrices de riesgo elaboradas por proveedores | NIST CSF — ID.RA |
| ⚠️ **Debilidad** | Metodología basada en listado de controles, no en identificación de amenazas | ISO 27001 — A.5.7 / Clause 6.1 |

**Recomendación:** Desarrollar evaluación de riesgos propia e independiente. Validar las matrices de proveedores contra el contexto real de la organización.

---

### 6️ Gestión de Proyectos

| Tipo | Hallazgo | Referencia |
|------|----------|------------|
| ✅ **Fortaleza** | Metodología empírica de 30 áreas de conocimiento aprobada por Junta | COBIT — BAI01 |
| ⚠️ **Debilidad** | Ausencia de PMO formal definida | COBIT — BAI01 |
| ⚠️ **Debilidad** | Ampliación de alcance sin ajuste de costos, tiempo ni personal | ISO 27001 — A.5.8 |
| ⚠️ **Debilidad** | Gerente de proyecto y líderes funcionales sin dedicación de tiempo completo | — |

**Recomendación:** Formalizar y estandarizar la metodología existente. Establecer control de cambios obligatorio para cualquier modificación de alcance.

---

### 7️ Continuidad del Negocio

| Tipo | Hallazgo | Referencia |
|------|----------|------------|
| ✅ **Fortaleza** | Comité de Continuidad de Negocio constituido por exigencia regulatoria | ISO 27001 — A.5.29 |
| ✅ **Fortaleza** | Representación de Operaciones, Riesgos, Tecnología y Negocios | — |
| ⚠️ **Debilidad** | Frecuencia de reuniones anual — insuficiente para banca | ISO 27001 — A.5.30 |
| ⚠️ **Debilidad** | Definición de RPO/RTO delegada a una sola persona | ISO 27001 — A.5.29 / A.5.30 |

**Recomendación:** Incrementar frecuencia de reuniones a trimestral como mínimo. Definir RPO/RTO de forma multisectorial, involucrando a los dueños de cada proceso crítico.

---

## Conclusión Ejecutiva

El caso ilustra desafíos recurrentes en instituciones financieras en transformación digital:

1. **Dependencia crítica de terceros** sin control directo sobre la continuidad operativa
2. **Gobernanza fragmentada** — ausencia de comité formal de Gobierno de TI
3. **Auditoría reactiva** en lugar de preventiva durante el ciclo de vida del proyecto
4. **Datos transfronterizos** sin supervisión directa del equipo de seguridad
5. **Gestión de riesgos delegada** a los proveedores en lugar de asumida internamente

### Competencias Demostradas

- Lectura crítica y análisis de documentación compleja
- Mapeo de hallazgos a marcos normativos internacionales
- Priorización basada en impacto empresarial
- Redacción de recomendaciones accionables
- Comunicación de conceptos técnicos a audiencias ejecutivas

---

## Nota de Atribución

Análisis desarrollado por **Jay Romero Amaya** como ejercicio profesional de evaluación de competencias. El escenario fue proporcionado como caso de estudio; la interpretación, mapeo a marcos normativos, hallazgos y recomendaciones son de elaboración propia.

Todos los datos institucionales han sido anonimizados para proteger la confidencialidad.

---

*Última actualización: Octubre 2025*
