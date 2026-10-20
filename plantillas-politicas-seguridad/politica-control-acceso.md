# Política de Control de Acceso

> **Documento de ejemplo** — Plantilla de trabajo elaborada como ejercicio de
> aplicación de ISO/IEC 27001. No corresponde a ninguna organización real.

| Campo | Valor |
|-------|-------|
| **Código** | POL-SEG-001 |
| **Versión** | 1.0 |
| **Clasificación** | Interna |
| **Propietario** | Dirección de Seguridad de la Información |
| **Aprobado por** | (Pendiente de aprobación) |
| **Fecha de vigencia** | (Pendiente) |
| **Próxima revisión** | 12 meses desde aprobación |

**Controles de referencia (ISO/IEC 27001:2013 → equivalente 2022):**

| Control 2013 | Equivalente 2022 | Tema |
|--------------|------------------|------|
| A.9.1.1 / A.9.1.2 | 5.15 | Política de control de acceso |
| A.9.2.1 | 5.16 | Registro y baja de usuarios |
| A.9.2.2 / A.9.2.5 / A.9.2.6 | 5.18 | Provisión, revisión y retiro de accesos |
| A.9.2.3 | 8.2 | Gestión de derechos de acceso privilegiado |
| A.9.2.4 / A.9.3.1 / A.9.4.3 | 5.17 | Gestión de credenciales de autenticación |
| A.9.4.1 | 8.3 | Restricción de acceso a la información |
| A.9.4.2 | 8.5 | Procedimientos de inicio de sesión seguro |
| A.9.4.4 | 8.18 | Uso de programas utilitarios privilegiados |
| A.9.4.5 | 8.4 | Control de acceso al código fuente |
| A.6.2.2 | 6.07 | Trabajo remoto (teletrabajo) |

---

## 1. Propósito

Establecer los lineamientos para la gestión de accesos a los sistemas de
información, garantizando que únicamente el personal autorizado acceda a los
recursos conforme a sus funciones y responsabilidades, protegiendo la
confidencialidad, integridad y disponibilidad de la información.

---

## 2. Alcance

Esta política aplica a:

- Todo el personal: empleados, contratistas, consultores y terceros
- Todas las aplicaciones, bases de datos, redes y sistemas corporativos
- Todos los dispositivos autorizados para conexión a la red institucional
- Todo tipo de acceso: presencial, remoto y móvil

---

## 3. Principios Rectores

### 3.1 Necesidad de conocer
El acceso se otorga únicamente cuando existe una necesidad operativa
justificada y documentada.

### 3.2 Menor privilegio
Cada usuario recibe el nivel mínimo de acceso necesario para desempeñar sus
funciones.

### 3.3 Segregación de funciones
Las funciones incompatibles entre sí se asignan a personas distintas para
prevenir errores y fraudes.

### 3.4 Trazabilidad
Todo acceso a información sensible debe quedar registrado y ser auditable.

---

## 4. Declaraciones de Política

### 4.1 Política de control de acceso *(A.9.1.1)*

1. El acceso a los sistemas se otorga sobre la base de requisitos de negocio
   y de seguridad, no por conveniencia operativa.
2. Las reglas de acceso se documentan formalmente y se mantienen actualizadas.
3. Toda solicitud de acceso debe pasar por un proceso de aprobación definido.

### 4.2 Acceso a redes y servicios de red *(A.9.1.2)*

1. El acceso a la red corporativa requiere autenticación individual.
2. Los servicios de red expuestos internamente se limitan a usuarios
   autorizados según su rol.
3. Las conexiones a redes inalámbricas corporativas utilizan cifrado.

### 4.3 Registro y baja de usuarios *(A.9.2.1)*

1. Toda solicitud de alta requiere autorización escrita del supervisor
   directo y validación de Recursos Humanos.
2. Cada usuario cuenta con una identidad única e intransferible. No se
   permiten cuentas compartidas ni genéricas.
3. Las cuentas temporales o de emergencia tienen fecha de expiración definida
   y se revisan semanalmente.
4. La baja de usuarios se ejecuta dentro de las 24 horas siguientes a la
   terminación de la relación laboral.

### 4.4 Provisión de accesos *(A.9.2.2)*

1. Los derechos de acceso se asignan mediante un proceso formal de solicitud
   y aprobación.
2. Los privilegios se otorgarán según el rol y las funciones del puesto,
   no a título personal.
3. Se mantiene un registro de todos los accesos asignados por usuario.

### 4.5 Gestión de accesos privilegiados *(A.9.2.3)*

1. Los accesos administrativos requieren aprobación de la Dirección de
   Tecnología y notificación a Seguridad de la Información.
2. Las cuentas privilegiadas son nominativas (no genéricas) y están sujetas
   a registro completo de actividad.
3. Los privilegios se revisan trimestralmente y se revocan cuando ya no
   sean necesarios.

### 4.6 Gestión de credenciales de autenticación *(A.9.2.4, A.9.3.1, A.9.4.3)*

1. Las credenciales son personales e intransferibles; su divulgación
   constituye una violación de esta política.
2. Las contraseñas cumplen requisitos mínimos de longitud y complejidad
   definidos en el estándar de autenticación.
3. Las credenciales temporales entregadas al alta deben cambiarse en el
   primer inicio de sesión.
4. No se almacenan contraseñas en texto plano ni en ubicaciones no cifradas.

### 4.7 Revisión de derechos de acceso *(A.9.2.5)*

1. Los derechos de acceso se revisan como mínimo cada seis meses.
2. Las cuentas inactivas por más de 90 días se deshabilitan.
3. Toda revisión queda documentada con evidencia de aprobación del
   responsable del sistema.

### 4.8 Retiro o ajuste de accesos *(A.9.2.6)*

1. Los accesos se retiran o ajustan ante cambios de puesto, traslados,
   licencias prolongadas o terminación de la relación laboral.
2. El retiro de accesos privilegiados se ejecuta de forma inmediata.
3. Se conserva evidencia del retiro para efectos de auditoría.

### 4.9 Restricción de acceso a la información *(A.9.4.1)*

1. El acceso a la información se restringe según su clasificación y la
   función del usuario.
2. La información clasificada como confidencial o restringida requiere
   controles adicionales de acceso.
3. Se aplica el principio de "pantalla limpia" en estaciones de trabajo.

### 4.10 Inicio de sesión seguro *(A.9.4.2)*

1. Los sistemas presentan un aviso de uso autorizado antes de la
   autenticación.
2. Las sesiones inactivas se cierran automáticamente tras un período máximo
   definido por el área de seguridad.
3. Los intentos fallidos de autenticación se limitan y se registran.
4. La autenticación multifactor (MFA) es obligatoria para acceso remoto,
   cuentas privilegiadas y sistemas con información clasificada.

### 4.11 Programas utilitarios privilegiados *(A.9.4.4)*

1. El uso de utilidades con capacidad de alterar sistemas se restringe a
   personal autorizado.
2. Estas herramientas se separan de las aplicaciones de uso general.
3. Su uso queda registrado y sujeto a revisión.

### 4.12 Acceso al código fuente *(A.9.4.5)*

1. El acceso al código fuente se limita al personal de desarrollo autorizado.
2. El código se gestiona en repositorios con control de versiones y
   trazabilidad de cambios.
3. El acceso al código de sistemas críticos requiere aprobación adicional.

### 4.13 Trabajo remoto *(A.6.2.2)*

1. El acceso remoto requiere autorización previa y dispositivo corporativo
   o dispositivo personal registrado.
2. Toda conexión remota se realiza a través de canal cifrado.
3. El trabajo remoto con información sensible cumple las mismas reglas de
   acceso que el trabajo presencial.

---

## 5. Responsabilidades

| Rol | Responsabilidad |
|-----|-----------------|
| **Usuarios** | Proteger sus credenciales, no compartirlas, reportar incidentes |
| **Supervisores** | Justificar y solicitar accesos según necesidad operativa |
| **Recursos Humanos** | Notificar altas, bajas y cambios de puesto oportunamente |
| **Tecnología** | Implementar y mantener los controles técnicos de acceso |
| **Seguridad de la Información** | Definir estándares, auditar cumplimiento, revisar privilegios |
| **Dirección** | Aprobar la política y asignar los recursos necesarios |

---

## 6. Cumplimiento

El incumplimiento de esta política puede derivar en:

- Notificación formal al supervisor y a Recursos Humanos
- Suspensión temporal de accesos
- Acciones disciplinarias conforme al reglamento interno
- Acciones legales cuando corresponda

---

## 7. Excepciones

Toda excepción a esta política debe:

1. Ser solicitada por escrito con justificación de negocio
2. Incluir análisis de riesgo y controles compensatorios
3. Ser aprobada por la Dirección de Seguridad de la Información
4. Tener fecha de expiración definida
5. Quedar registrada en el inventario de excepciones

---

## 8. Definiciones

| Término | Definición |
|---------|------------|
| **Acceso privilegiado** | Acceso que permite modificar configuraciones, gestionar usuarios o alterar controles de seguridad |
| **MFA** | Autenticación multifactor: verificación mediante dos o más factores independientes |
| **Menor privilegio** | Principio de otorgar únicamente los permisos mínimos necesarios |
| **Segregación de funciones** | Separación de tareas incompatibles entre distintas personas |
| **Cuenta genérica** | Cuenta compartida por múltiples usuarios (prohibida por esta política) |

---

## 9. Revisión y Actualización

Esta política se revisa anualmente o cuando ocurra un cambio significativo en:

- La normativa legal aplicable
- La infraestructura tecnológica
- La estructura organizacional
- Los resultados de auditorías o incidentes relevantes

---

## Historial de Revisiones

| Fecha | Versión | Descripción del Cambio | Autor |
|-------|---------|------------------------|-------|
| 2025-10-20 | 1.0 | Versión inicial como plantilla de trabajo | Jay Romero Amaya |

---

## 🔗 Nota sobre las Fuentes

- **Numeración de controles:** base en **ISO/IEC 27001:2013 (Anexo A)** —
  edición a la que tengo acceso y que apliqué en mi análisis de casos.
- **Equivalencias 2022:** derivadas de material de mapeo de transición entre
  ediciones. Son orientativas, ya que varios controles de 2013 se fusionaron
  o reorganizaron en 2022.
- Para el texto íntegro de los controles, consultar la documentación publicada
  por ISO en [iso.org](https://www.iso.org).

**Referencias:**
- ISO/IEC 27001:2013 — Requisitos del SGSI (Anexo A)
- ISO/IEC 27001:2022 — Edición vigente (Anexo A)
- ISO/IEC 27002 — Guía de implementación de controles

---

*Plantilla elaborada como ejercicio de aplicación de ISO/IEC 27001.
No constituye una política aprobada ni implementada en organización alguna.*
