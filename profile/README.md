# All Roads | Documentación de Desarrollo

Bienvenido al repositorio de documentación técnica y funcional de **All Roads**.

Url producto: **https://allroadsmedellin.com.co/**

<p align="center">
  <a href="https://github.com/All-Roads-1cero1/Documentacion_Desarrollo">
    <img src="https://img.shields.io/badge/DOCUMENTACIÓN-ALL%20ROADS-334155?style=for-the-badge&logo=github&logoColor=white" alt="Documentación All Roads">
  </a>
  &nbsp;
  <a href="https://github.com/All-Roads-1cero1/AllRoads_FrontEnd">
    <img src="https://img.shields.io/badge/FRONTEND-ALL%20ROADS-7C3AED?style=for-the-badge&logo=vue.js&logoColor=white" alt="Frontend All Roads">
  </a>
  &nbsp;
  <a href="https://github.com/All-Roads-1cero1/AllRoads_Backend">
    <img src="https://img.shields.io/badge/BACKEND-ALL%20ROADS-0F766E?style=for-the-badge&logo=nestjs&logoColor=white" alt="Backend All Roads">
  </a>
  
<a href="https://github.com/All-Roads-1cero1/user-admin">
  <img
    src="https://img.shields.io/badge/PANEL%20OPERATIVO-ADMIN%20DE%20USUARIOS-263238?style=for-the-badge&logo=github&logoColor=white"
    alt="Panel Operativo - Administración de Usuarios"
  >
</a>
&nbsp;

</p>

Este repositorio centraliza la documentación del proyecto desde la construcción del **MVP - Fase 1** hasta la planificación y ejecución de la **Fase 2**.

Aquí se encuentran documentos de alcance, actas de reunión, casos de uso, requisitos funcionales, planificación de desarrollo y documentación interna del proyecto.

---

# Estado general del proyecto

| Fase | Estado | Inicio | Entrega / cierre |
| :--- | :--- | :--- | :--- |
| **Fase 1 - MVP** | ✅ Entregado | 11 de mayo de 2026 | **5 de agosto de 2026** |
| **Fase 2** | 🟡 Planificada / En desarrollo | **26 de agosto de 2026** | **15 de diciembre de 2026** |

---

# Estructura de documentación

Actualmente el repositorio se encuentra organizado de la siguiente manera:

```text
Documentacion_Desarrollo
│
├── Documentacion_Fase2
│   ├── All_Roads_Documento_Interno_Fase2_V1.docx
│   ├── All_Roads_Fase2_Casos_de_Uso.docx
│   ├── All_Roads_Fase2_Requisitos_Funcionales.docx
│   └── All_Roads_Fase_2_Plan_DesarrolloV1.docx
│
└── Documentacion_MVP
    ├── ACTA DE REUNIÓN SPRINT 1.pdf
    ├── ACTA DE REUNIÓN SPRINT 2 (1).pdf
    ├── ACTA DE REUNIÓN SPRINT 2.pdf
    ├── Acta_de_reunion_Sprint_3_y_4.pdf
    ├── Alcance MVP All roads.pdf
    ├── Desarrollo-All_Roads_docMVP(INTERNO).docx
    │
    └── Casos_de_uso
        ├── CU-Administrador.md
        ├── CU-Pasarela-Pago.md
        ├── CU-Servicio-Correo.md
        └── CU-Visitante.md
```

---

# Fase 1 - MVP

## Información general

| Dato | Valor |
| :--- | :--- |
| **Proyecto** | All Roads |
| **Fase** | Desarrollo Fase 1 - MVP |
| **Estado** | ✅ Entregado |
| **Inicio** | 11 de mayo de 2026 |
| **Entrega final** | **5 de agosto de 2026** |
| **Portal** | Vue |
| **Backoffice** | Vue |
| **Backend** | NestJS |
| **Base de datos** | PostgreSQL |
| **Pasarela de pagos** | Integración externa |

---

## Objetivo del MVP

El objetivo de la primera fase fue construir una versión funcional de All Roads que permitiera completar el flujo principal de:

**Consulta → Carrito → Reserva → Pago → Confirmación → Consulta administrativa**

El MVP permitió validar la operación principal del producto antes de incorporar las funcionalidades administrativas avanzadas contempladas para la Fase 2.

---

# Alcance del MVP

## Portal público

| Elemento | Detalle |
| :--- | :--- |
| **Home** | Presentación principal del portal, tours destacados, aliados y contenido institucional. |
| **Listado de tours** | Visualización de tours disponibles. |
| **Detalle de tour** | Información general, descripción, imágenes, lugares, elementos incluidos, precio y tours relacionados. |
| **Carrito** | Permite agregar uno o varios tours y definir la cantidad de personas por tour. |
| **Formulario de reserva** | Captura de información necesaria para crear la reserva. |
| **Términos y condiciones** | Requisito previo para habilitar el pago. |
| **Pago** | Integración con la pasarela de pagos. |
| **Resultado de pago** | Visualización del estado final de la transacción. |
| **Correo de confirmación** | Envío de confirmación cuando la reserva/pago alcanza el estado correspondiente. |

---

## Backoffice administrativo

| Elemento | Detalle |
| :--- | :--- |
| **Login** | Inicio de sesión administrativo. |
| **Recuperación de contraseña** | Recuperación mediante correo y código de validación. |
| **Layout administrativo** | Estructura principal del panel administrativo. |
| **Protección de rutas** | Acceso únicamente para usuarios autenticados. |
| **Reservas** | Consulta de listado y detalle de reservas en modo solo lectura. |

---

# Documentación del MVP

La documentación correspondiente a la primera fase se encuentra en:

[`Documentacion_MVP`](./Documentacion_MVP/)

## Documentos principales

| Documento | Descripción |
| :--- | :--- |
| [Alcance MVP All Roads](./Documentacion_MVP/Alcance%20MVP%20All%20roads.pdf) | Documento de alcance funcional del MVP. |
| [Documento interno del MVP](./Documentacion_MVP/Desarrollo-All_Roads_docMVP(INTERNO).docx) | Documento interno de planificación y desarrollo de la Fase 1. |

---

## Actas de reunión

| Documento |
| :--- |
| [Acta de reunión - Sprint 1](./Documentacion_MVP/ACTA%20DE%20REUNI%C3%93N%20SPRINT%201.pdf) |
| [Acta de reunión - Sprint 2](./Documentacion_MVP/ACTA%20DE%20REUNI%C3%93N%20SPRINT%202.pdf) |
| [Acta de reunión - Sprint 2 (1)](./Documentacion_MVP/ACTA%20DE%20REUNI%C3%93N%20SPRINT%202%20(1).pdf) |
| [Acta de reunión - Sprint 3 y 4](./Documentacion_MVP/Acta_de_reunion_Sprint_3_y_4.pdf) |

---

## Casos de uso del MVP

Los casos de uso se encuentran en:

[`Documentacion_MVP/Casos_de_uso`](./Documentacion_MVP/Casos_de_uso/)

| Actor | Documento |
| :--- | :--- |
| **Administrador** | [CU-Administrador](./Documentacion_MVP/Casos_de_uso/CU-Administrador.md) |
| **Visitante** | [CU-Visitante](./Documentacion_MVP/Casos_de_uso/CU-Visitante.md) |
| **Pasarela de pago** | [CU-Pasarela-Pago](./Documentacion_MVP/Casos_de_uso/CU-Pasarela-Pago.md) |
| **Servicio de correo** | [CU-Servicio-Correo](./Documentacion_MVP/Casos_de_uso/CU-Servicio-Correo.md) |

---

# Flujo principal del MVP

1. El visitante ingresa al portal de All Roads.
2. Explora los tours disponibles.
3. Consulta el detalle de un tour.
4. Agrega uno o varios tours al carrito.
5. Define la cantidad de personas.
6. Revisa subtotales y valor total.
7. Diligencia la información de reserva.
8. Acepta términos y condiciones.
9. El sistema crea una reserva u orden previa.
10. El usuario es redirigido a la pasarela.
11. La pasarela procesa la transacción.
12. El sistema recibe y procesa el resultado.
13. Se actualiza el estado correspondiente.
14. El usuario visualiza el resultado de la transacción.
15. Cuando corresponde, se envía el correo de confirmación.
16. La reserva queda disponible para consulta administrativa.

---

# Fase 2

## Información general

| Dato | Valor |
| :--- | :--- |
| **Fase** | Desarrollo Fase 2 |
| **Inicio programado** | **26 de agosto de 2026** |
| **Entrega prevista** | **15 de diciembre de 2026** |
| **Duración estimada** | 16 semanas calendario |
| **Cantidad de sprints** | 4 |
| **Sprint 1** | 4 días de trabajo por semana |
| **Sprint 2** | 3 días de trabajo por semana |
| **Sprint 3** | 2 días de trabajo por semana |
| **Sprint 4** | 2 días de trabajo por semana |
| **Portal** | Vue |
| **Backoffice** | Vue |
| **Backend** | NestJS |
| **Base de datos** | PostgreSQL |
| **Pasarela** | Fintech 101 |

---

# Objetivo de la Fase 2

La Fase 2 tiene como objetivo convertir el MVP operativo en una plataforma administrable.

El sistema evolucionará para permitir que All Roads gestione directamente desde el Backoffice:

- tours;
- categorías;
- fechas;
- horarios;
- cupos;
- imágenes;
- reservas;
- cupones;
- dashboard;
- reportes;
- notificaciones;
- logs y auditoría.

El Portal dejará progresivamente de depender de información estática o mock y consumirá la información administrada desde Backend y Backoffice.

---

# Cronograma de la Fase 2

| Sprint | Fechas | Intensidad | Foco principal |
| :--- | :--- | :--- | :--- |
| **Sprint 1** | **26 de agosto al 15 de septiembre de 2026** | **4 días/semana** | Tours + Fechas/Horarios + Cupos |
| **Sprint 2** | **16 de septiembre al 20 de octubre de 2026** | **3 días/semana** | Galería + Reservas + Cupones |
| **Sprint 3** | **21 de octubre al 24 de noviembre de 2026** | **2 días/semana** | Logs + Dashboard + Reportes + Notificaciones |
| **Sprint 4** | **25 de noviembre al 15 de diciembre de 2026** | **2 días/semana** | QA + Correcciones + Regresión + Cierre |

---

# Sprint 1

## Tours + Fechas/Horarios + Cupos configurables

**Período:** 26 de agosto al 15 de septiembre de 2026  
**Intensidad:** 4 días de trabajo por semana.

### Objetivo

Completar la administración de tours desde Backoffice e integrar en el Portal la información real suministrada por Backend.

### Alcance

- Integrar en Backoffice la funcionalidad existente de crear tour.
- Integrar la funcionalidad existente de agregar horario.
- Integrar la funcionalidad existente de subir imagen cuando corresponda.
- Crear categorías.
- Asociar categorías a tours.
- Modificar tours.
- Eliminar tours mediante eliminación lógica.
- Publicar y despublicar tours.
- Habilitar e inhabilitar horarios.
- Listar tours para administración.
- Configurar cupos.
- Editar cupos.
- Permitir horarios sin límite o con límite.
- Definir capacidad máxima cuando exista límite.
- Consultar disponibilidad.
- Integrar tours reales en Portal.
- Integrar fechas y horarios reales en Portal.
- Mostrar alertas de disponibilidad.
- Eliminar la dependencia de información mock.

### Adelanto de Sprint 2

Cuando Backend complete el alcance correspondiente al Sprint 1, podrá adelantar:

- edición de campos básicos de reserva;
- reagendamiento de reservas;
- cancelación de reservas.

---

# Sprint 2

## Galería + Gestión avanzada de reservas + Cupones

**Período:** 16 de septiembre al 20 de octubre de 2026  
**Intensidad:** 3 días de trabajo por semana.

### Gestión de reservas

- Consultar información de una reserva.
- Editar campos permitidos.
- Reagendar reservas.
- Consultar fechas y horarios disponibles.
- Validar disponibilidad al reagendar.
- Validar cupos disponibles.
- Actualizar ocupación de cupos.
- Cancelar reservas.
- Liberar cupos cuando corresponda.

### Cupones

- Listar cupones.
- Consultar cupón.
- Crear cupón.
- Editar cupón.
- Activar o desactivar cupón.
- Eliminar cupón.
- Validar cupón.
- Aplicar descuentos dentro del flujo de compra.

### Galería de imágenes

- Integrar el endpoint existente para subir imágenes.
- Listar imágenes.
- Consultar imágenes.
- Editar información y orden.
- Seleccionar imagen principal.
- Eliminar imágenes.
- Reflejar los cambios de la galería en el Portal.

### Adelanto de Sprint 3

Cuando Backend complete el alcance correspondiente al Sprint 2, podrá adelantar:

- listado de logs;
- detalle de logs;
- trazabilidad administrativa.

---

# Sprint 3

## Logs + Dashboard + Reportes + Notificaciones

**Período:** 21 de octubre al 24 de noviembre de 2026  
**Intensidad:** 2 días de trabajo por semana.

### Logs y auditoría

- Listar logs.
- Consultar detalle de logs.
- Validar trazabilidad de acciones administrativas.
- Registrar acciones relevantes sobre tours.
- Registrar acciones sobre reservas.
- Registrar acciones sobre cupones.

### Dashboard

- Crear vista principal.
- Integrar indicadores.
- Consultar información consolidada.
- Incorporar filtros.
- Mostrar información de reservas, pagos y tours según los indicadores definidos.

### Reportes

- Adaptar el reporte de reservas.
- Utilizar el formato oficial suministrado.
- Integrar información de Backend.
- Implementar filtros requeridos.
- Validar consistencia de información.

### Notificaciones

- Notificar creación de reserva.
- Notificar modificación de reserva.
- Notificar creación de tour cuando corresponda.
- Notificar modificación de tour cuando corresponda.
- Enviar comunicaciones al correo administrativo configurado.

---

# Sprint 4

## QA + Correcciones + Regresión + Cierre

**Período:** 25 de noviembre al 15 de diciembre de 2026  
**Intensidad:** 2 días de trabajo por semana.

### Objetivo

Validar integralmente la Fase 2, corregir hallazgos y preparar una versión estable para entrega.

Durante este sprint no se deben incorporar nuevas funcionalidades que estén fuera del alcance definido.

### Alcance de QA

Se deben validar:

- tours;
- categorías;
- fechas;
- horarios;
- cupos;
- galería;
- reservas;
- reagendamientos;
- cancelaciones;
- cupones;
- logs;
- dashboard;
- reportes;
- notificaciones;
- Portal;
- Backoffice;
- Backend;
- integración con el flujo de pagos.

### Flujo principal de regresión

```text
Tour
  ↓
Fecha / Horario
  ↓
Disponibilidad / Cupos
  ↓
Carrito
  ↓
Reserva
  ↓
Cupón
  ↓
Pago
  ↓
Confirmación
```

Los hallazgos de QA deben reportarse progresivamente para permitir que Backend y Frontend realicen correcciones mientras continúa el ciclo de pruebas.

---

# Documentación de Fase 2

Todos los documentos correspondientes a esta fase se encuentran en:

[`Documentacion_Fase2`](./Documentacion_Fase2/)

## Documentos disponibles

| Documento | Descripción |
| :--- | :--- |
| [Documento Interno Fase 2](./Documentacion_Fase2/All_Roads_Documento_Interno_Fase2_V1.docx) | Documento interno de planificación, alcance, reglas, cronograma y control de la Fase 2. |
| [Casos de Uso Fase 2](./Documentacion_Fase2/All_Roads_Fase2_Casos_de_Uso.docx) | Casos de uso correspondientes a las nuevas funcionalidades de la Fase 2. |
| [Requisitos Funcionales Fase 2](./Documentacion_Fase2/All_Roads_Fase2_Requisitos_Funcionales.docx) | Requisitos funcionales definidos para la Fase 2. |
| [Plan de Desarrollo Fase 2](./Documentacion_Fase2/All_Roads_Fase_2_Plan_DesarrolloV1.docx) | Documento de alcance, cronograma y entregables de la Fase 2. |

---

# Definición de cupos

Los tours operarán inicialmente **sin límite de cupos**.

Sin embargo, la Fase 2 debe dejar preparado el sistema para configurar límites desde Backoffice.

Cada fecha/horario podrá trabajar en uno de dos modos:

| Modo | Comportamiento |
| :--- | :--- |
| **Sin límite** | No se aplica restricción por cantidad de personas. |
| **Con límite** | El administrador define una capacidad máxima. |

Cuando exista límite, Backend debe validar la disponibilidad antes de:

- crear una reserva;
- modificar una reserva cuando afecte cantidad o programación;
- reagendar una reserva.

La ocupación debe mantenerse consistente ante:

- nuevas reservas;
- reagendamientos;
- cancelaciones.

---

# Flujo del administrador después de Fase 2

El Backoffice evolucionará para permitir:

1. Iniciar sesión.
2. Recuperar contraseña.
3. Consultar tours.
4. Crear y modificar tours.
5. Publicar o despublicar tours.
6. Gestionar categorías.
7. Gestionar fechas y horarios.
8. Configurar cupos.
9. Gestionar imágenes.
10. Consultar reservas.
11. Editar campos permitidos de reservas.
12. Reagendar reservas.
13. Cancelar reservas.
14. Administrar cupones.
15. Consultar Dashboard.
16. Generar reportes.
17. Consultar logs de auditoría.
18. Recibir las notificaciones administrativas definidas.

---

# Reglas de negocio principales

| Regla | Definición |
| :--- | :--- |
| **Tours en compra** | Una compra puede contener uno o varios tours. |
| **Cantidad de personas** | La cantidad se define individualmente para cada tour. |
| **Precio total** | Se calcula según precio, cantidad de personas y tours incluidos. |
| **Términos y condiciones** | Deben ser aceptados antes de habilitar el pago. |
| **Orden previa al pago** | Se debe crear una reserva u orden pendiente antes de iniciar la pasarela. |
| **Pago** | Los datos sensibles son procesados por la pasarela de pagos. |
| **Confirmación** | El estado final depende de la respuesta obtenida desde la pasarela. |
| **Tours publicados** | Solo los tours publicados deben estar disponibles públicamente. |
| **Fechas y horarios** | Los horarios inhabilitados no deben estar disponibles para nuevas reservas. |
| **Cupos** | Por defecto son ilimitados, pero pueden configurarse con capacidad máxima. |
| **Disponibilidad** | Backend es responsable de validar capacidad cuando exista un límite. |
| **Reagendamiento** | Solo puede realizarse hacia fechas/horarios válidos y disponibles. |
| **Cancelación** | Debe liberar disponibilidad cuando exista control de cupos. |
| **Cupones** | Su estado, vigencia y reglas deben ser validados desde Backend. |
| **Auditoría** | Las acciones administrativas relevantes deben quedar registradas. |
| **Regresión** | La Fase 2 no debe afectar negativamente funcionalidades entregadas en el MVP. |

---

# Estados del pago

| Evento | Resultado esperado |
| :--- | :--- |
| **Pago aprobado** | Reserva pagada y envío de correo de confirmación. |
| **Pago rechazado** | Transacción rechazada. |
| **Error técnico** | Pago fallido. |
| **Tiempo vencido** | Transacción expirada. |
| **Transacción sin confirmación** | Permanece pendiente hasta finalizar o vencer el intento. |

---

# Tiempo de vigencia del pago

El tiempo disponible para completar el pago y mantener la reserva pendiente corresponde al definido por la pasarela:

**30 minutos**

---

# Actores principales

## Visitante

Usuario público que utiliza el Portal para:

- consultar tours;
- seleccionar fechas y horarios;
- definir cantidad de personas;
- consultar disponibilidad;
- agregar tours al carrito;
- diligenciar información de reserva;
- aplicar cupones cuando corresponda;
- aceptar términos;
- realizar el pago;
- consultar el resultado de la transacción.

---

## Administrador

Usuario autenticado que utiliza el Backoffice.

### MVP

Durante el MVP puede:

- iniciar sesión;
- recuperar contraseña;
- consultar reservas.

### Fase 2

La administración evoluciona para permitir:

- gestionar tours;
- gestionar categorías;
- administrar fechas y horarios;
- configurar cupos;
- administrar imágenes;
- gestionar reservas;
- administrar cupones;
- consultar Dashboard;
- generar reportes;
- consultar auditoría.

---

## Pasarela de pagos

Servicio externo encargado de:

- recibir al comprador;
- procesar la transacción;
- retornar o notificar el resultado;
- definir el estado final del intento de pago.

All Roads no almacena directamente información sensible de tarjetas.

---

## Servicio de correo

Servicio encargado de:

- enviar correos de confirmación;
- soportar notificaciones transaccionales;
- soportar las notificaciones administrativas definidas durante la Fase 2.

---

# Dependencias y definiciones pendientes de Fase 2

Durante la ejecución deberán cerrarse o validarse las siguientes definiciones:

- eventos definitivos de notificación;
- destinatarios de las notificaciones administrativas;
- indicadores definitivos del Dashboard;
- formato definitivo del Reporte operativo;
- reglas comerciales específicas de cupones;
- campos exactos que pueden modificarse en una reserva;
- estados que permiten reagendamiento;
- estados que permiten cancelación;
- comportamiento cuando se reduce el límite de cupos de un horario que ya posee reservas.

---

# Nota sobre Fintech 101

La integración de pagos existente debe conservarse durante la Fase 2.

La habilitación o configuración comercial de métodos de pago, como tarjeta de crédito dentro de **Fintech 101**, corresponde al responsable comercial y no constituye una tarea de desarrollo de Frontend o Backend.

El equipo de desarrollo es responsable de mantener correctamente la integración y procesar los estados/resultados suministrados por la pasarela.

---

# Control del proyecto

La evolución actual del proyecto es:

```text
FASE 1 - MVP
11 de mayo de 2026
        ↓
Desarrollo MVP
        ↓
5 de agosto de 2026
✅ MVP ENTREGADO
        ↓
26 de agosto de 2026
FASE 2
        ↓
Sprint 1
Tours + Fechas/Horarios + Cupos
        ↓
Sprint 2
Galería + Reservas + Cupones
        ↓
Sprint 3
Logs + Dashboard + Reportes + Notificaciones
        ↓
Sprint 4
QA + Correcciones + Regresión
        ↓
15 de diciembre de 2026
🎯 ENTREGA PREVISTA FASE 2
```

---

# Nota de control documental

Este repositorio documenta la evolución funcional y técnica de **All Roads**.

- La **Fase 1 - MVP fue entregada el 5 de agosto de 2026**.
- La **Fase 2 inicia el 26 de agosto de 2026**.
- La **entrega prevista de la Fase 2 es el 15 de diciembre de 2026**.
- La documentación de cada fase se mantiene separada dentro de `Documentacion_MVP` y `Documentacion_Fase2`.

Cualquier modificación de funcionalidades, reglas de negocio, cronograma o alcance debe pasar por revisión y validación del equipo responsable antes de incorporarse oficialmente al proyecto.
