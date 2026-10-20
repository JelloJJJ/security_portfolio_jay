# Checklist de Auditoría — ISO/IEC 27001 (Base 2013 + Referencia 2022)

Herramienta de verificación para evaluar la implementación de controles de
seguridad de la información.

**Estructura de referencia:** el checklist usa como base los controles del
**Anexo A de ISO/IEC 27001:2013** (edición a la que tengo acceso y que apliqué
en mi análisis de casos), e incluye la columna de equivalencia aproximada a
la **edición 2022** según material de mapeo oficial de transición.

---

## 📖 Cómo Usarlo

1. Seleccionar los controles aplicables a la organización
2. Verificar cada control contra evidencia documental
3. Registrar cumplimiento: `✓` = cumple · `✗` = no cumple · `P` = parcial · `N/A` = no aplica
4. Documentar observaciones y acciones correctivas

---

## ✅ Controles Utilizados en Mi Análisis de Caso

Estos son los controles que apliqué directamente en mi evaluación del caso
del sector financiero. Cada uno fue consultado en el Anexo A 2013 durante
el trabajo analítico.

| Control 2013 | Equivalente 2022 (aprox.) | Nombre del Control | Pregunta de Auditoría | Evidencia Esperada | Cumple |
|---|---|---|---|---|---|
| A.14.2.5 | 8.27 | Principios de ingeniería de sistemas seguros | ¿Los sistemas críticos se desarrollan bajo principios de ingeniería segura? | Arquitectura documentada, acceso al código fuente | |
| A.6.1.1 | 5.2 | Roles y responsabilidades de seguridad | ¿Existen roles de seguridad formalmente asignados y reportando al nivel directivo? | Descripciones de puesto, organigrama, comités | |
| A.5.1.1 | 5.1 | Políticas de seguridad de la información | ¿Existe política aprobada por la dirección y revisada periódicamente? | Política firmada + registro de revisiones | |
| A.9.2.3 | 8.2 | Gestión de derechos de acceso privilegiado | ¿Los accesos administrativos están restringidos, controlados y revisados? | Registro de cuentas admin + revisiones periódicas | |
| A.14.2.1 | 8.25 | Política de desarrollo seguro | ¿Se aplican controles de seguridad durante el desarrollo de sistemas? | Metodología de desarrollo seguro documentada | |
| A.14.2.2 | 8.32 | Gestión de cambios en sistemas | ¿Los cambios en sistemas de producción siguen un control formal? | Registros de solicitudes de cambio aprobadas | |
| A.15.1.1 | 5.19 | Seguridad en relaciones con proveedores | ¿Existe política que regule la seguridad con terceros? | Política de proveedores + contratos con cláusulas | |
| A.15.1.2 | 5.20 | Seguridad en acuerdos con proveedores | ¿Los contratos incluyen SLAs y requisitos de seguridad verificables? | Contratos vigentes + reportes de cumplimiento | |
| A.18.1.4 | 5.34 | Privacidad y protección de datos personales | ¿Se garantiza la protección de datos almacenados fuera de la jurisdicción local? | Análisis legal de transferencia internacional | |
| A.17.1.1 | 5.29 | Planificación de continuidad de seguridad | ¿Existe plan de continuidad probado y actualizado? | BCP documentado + resultados de pruebas | |
| A.8.1.3 | 5.10 | Uso aceptable de activos | ¿Se gestionan los activos según reglas de uso aceptable? | Inventario de activos + reglas de uso | |

---

## 📋 Controles Complementarios (Del Mapeo de Transición)

Controles adicionales relevantes para una evaluación integral, incluidos a partir
del material de mapeo entre ediciones. Marcan áreas típicas de revisión que
complementan los controles anteriores.

| Control 2013 | Equivalente 2022 (aprox.) | Nombre del Control | Pregunta de Auditoría | Evidencia Esperada | Cumple |
|---|---|---|---|---|---|
| A.9.1.1 / 9.1.2 | 5.15 | Política de control de acceso | ¿El acceso se otorga según necesidad de conocer? | Matriz de accesos por rol | |
| A.9.4.2 | 8.5 | Procedimientos de inicio de sesión seguro | ¿Se usan mecanismos de autenticación robustos? | Configuración MFA + política de contraseñas | |
| A.12.1.2 | 8.32 | Gestión de cambios | ¿Existe procedimiento formal de cambios en operación? | Registros de control de cambios | |
| A.12.3.1 | 8.13 | Copias de seguridad | ¿Se realizan y prueban respaldos? | Registros de backup + pruebas de restauración | |
| A.12.6.1 | 8.8 | Gestión de vulnerabilidades técnicas | ¿Se realizan escaneos periódicos? | Reportes de escaneo + plan de remediación | |
| A.12.4.1 | 8.15 | Registro de eventos | ¿Se registran eventos de seguridad relevantes? | Configuración de logs + retención | |
| A.15.2.1 | 5.22 | Monitoreo de servicios de proveedores | ¿Se monitorea el cumplimiento de los proveedores? | Reportes de SLA + actas de revisión | |
| A.14.2.8 / 14.2.9 | 8.29 | Pruebas de seguridad en desarrollo | ¿Se prueban sistemas antes de pasar a producción? | Informes de pruebas + resultados | |
| A.14.2.6 / 12.1.4 | 8.31 | Separación de ambientes (dev/test/prod) | ¿Los ambientes están separados? | Diagrama de arquitectura | |
| A.18.2.1 | 5.35 | Revisión independiente de seguridad | ¿Se realiza auditoría externa periódica? | Informe de firma auditora externa | |

---

## 📌 Leyenda

| Símbolo | Significado |
|---------|-------------|
| `✓` | Cumple |
| `✗` | No cumple |
| `P` | Cumplimiento parcial |
| `N/A` | No aplica (requiere justificación documentada) |

---

## 🔗 Nota sobre las Fuentes de Este Checklist

- **Columna de controles 2013:** base del checklist, correspondiente a los
  controles aplicados en mi análisis de casos y material de estudio disponible.
- **Columna de equivalencia 2022:** derivada de material de mapeo de transición
  entre ediciones del estándar. Las equivalencias son orientativas; varios
  controles de 2013 se fusionaron o reorganizaron en 2022, por lo que una
  correspondencia no siempre es uno a uno.
- Para mapeo oficial y texto íntegro de los controles, consultar la documentación
  publicada por ISO en [iso.org](https://www.iso.org).

**Referencias:**
- ISO/IEC 27001:2013 — Requisitos del SGSI (Anexo A: 114 controles)
- ISO/IEC 27001:2022 — Edición vigente (Anexo A: 93 controles)
- ISO/IEC 27002 — Guía de implementación de controles

---

*Plantilla de trabajo elaborada por Jay Romero Amaya — Octubre 2025*
