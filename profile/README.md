# All Roads (Desarrollo)

Bienvenido a All Roads (Desarrollo). Este espacio centraliza la documentación técnica y las guías necesarias para contribuir, ejecutar y mantener el proyecto en su fase de desarrollo.

**Qué encontrarás aquí:**
##  Casos de Uso

En esta sección se listan los documentos de Casos de Uso del sistema.

| Actor | Documentación |
| :--- | :--- |
| **Administrador** | [Casos de Uso - Administrador](https://github.com/All-Roads-1cero1/Documentacion_Desarrollo/blob/main/Casos_de_uso/Casos-de-Uso-Administrador.pdf) |
| **Visitantes** | [Casos de Uso - Visitantes](https://github.com/All-Roads-1cero1/Documentacion_Desarrollo/blob/main/Casos_de_uso/Casos-de-Uso-Visitantes.pdf) |
| **Pasarela Pago** | [Casos de Uso - Pasarela Pago](https://github.com/All-Roads-1cero1/Documentacion_Desarrollo/blob/main/Casos_de_uso/Casos-de-Uso-Pasarela-Pago.pdf) |
| **Servicio Correo** | [Casos de Uso - Servicio Correo](https://github.com/All-Roads-1cero1/Documentacion_Desarrollo/blob/main/Casos_de_uso/Casos-de-Uso-Servicio-Correo.pdf) |

---


## Diagramas

### Modelo de la base de datos

Esta sección presenta el modelo de tablas de la base de datos

![Modelo DB](https://github.com/All-Roads-1cero1/Documentacion_Desarrollo/blob/main/model_db.svg)

Puedes acceder a la imagen en alta resolución directamente aquí: [Diagrama de clases](https://github.com/All-Roads-1cero1/Documentacion_Desarrollo/blob/main/model_db.svg).

---

##  Actores Clave del Sistema

Esta sección describe los principales actores que interactúan con el proyecto **All Roads** y sus roles en la arquitectura.

###  Actor: Visitante (VIS)

| Aspecto | Descripción |
| :--- | :--- |
| **Rol Principal** | Usuario público que navega el portal para explorar, reservar y pagar servicios turísticos sin requerir cuenta. |
| **Responsabilidades** | Explorar productos; seleccionar fecha y cupos; ingresar datos verídicos; aceptar políticas de datos y términos; **completar el pago** en la pasarela; revisar, consultar su reserva. |
| **Nivel de Acceso** | **Público sin autenticación** para navegación y armado de reserva. Validación puntual mediante consecutivo + dato personal para consultar reservas. |
| **Interacciones con sistemas externos** | Pasarela de Pagos (checkout); Servicio de Correo (confirmaciones y comprobantes). |

---

###  Actor: Pasarela de Pagos (PP)

| Aspecto | Descripción |
| :--- | :--- |
| **Rol Principal** | Proveedor externo (Wompi/PayU/MercadoPago) que autoriza, procesa y liquida las transacciones. |
| **Responsabilidades** | Exponer checkout seguro; aplicar antifraude, **notificar el resultado por webhook seguro** (aprobado, rechazado, pendiente); gestionar reversos/devoluciones y reportería. |
| **Nivel de Acceso** | Integración **API/Webhook autenticada** (llaves/firmas) server-to-server. Sin acceso a la UI del CMS. |
| **Interacciones con sistemas externos** | Backend de ALL ROADS (órdenes y webhooks); redes financieras/bancos. |

---

###  Actor: Servicio de Correo (SC)

| Aspecto | Descripción |
| :--- | :--- |
| **Rol Principal** | Servicio de mensajería transaccional que envía confirmaciones de reserva, comprobantes, avisos de pago y comunicaciones operativas. |
| **Responsabilidades** | **Entregar correos transaccionales**; gestionar plantillas HTML responsive; mantener autenticación de dominio; registrar eventos de envío/entrega/rebote para auditoría. |
| **Nivel de Acceso** | Integración **SMTP/API con credenciales seguras**. Sin acceso al CMS más allá del contenido a enviar. |
| **Interacciones con sistemas externos** | Backend de ALL ROADS (disparo de correos); Visitante (recepción de mensajes). |


###  Actor: Administrador (CMS Backoffice)

| Aspecto | Descripción |
| :--- | :--- |
| **Rol Principal** | Usuario interno encargado de administrar el sitio web mediante un panel de control CMS. |
| **Responsabilidades** | Gestionar el catálogo de productos turísticos, controlar la disponibilidad y reservas, editar contenidos del portal, administrar formularios de contacto, exportar datos y mantener la configuración del sistema. |
| **Nivel de Acceso** | **Autenticado** mediante credenciales y roles definidos. |
| **Interacciones con sistemas externos** | Pasarela de Pagos, Servicio de Correo, Visitante. |
