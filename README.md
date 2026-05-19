# Documentación Arquitectura AGROBODEGA

**Autores:**
[Nombre 1]
[Nombre 2]

---

## Índice

- [Documentación Arquitectura AGROBODEGA](#documentación-arquitectura-agrobodega)
  - [Portada](#portada)
- [Excel AGROBODEGA — Drivers Arquitectónicos](#excel-agrobodega--drivers-arquitectónicos)
  - [Hoja: TRADEOFF](#hoja-tradeoff)
  - [Hoja: Mapa de Empatía](#hoja-mapa-de-empatía)
  - [Hoja: Caracterización](#hoja-caracterización)
  - [Hoja: Primera Ronda de Votación](#hoja-primera-ronda-de-votación)
  - [Hoja: Segunda Votación](#hoja-segunda-votación)
  - [Hoja: ESC-CAL-USA-0001](#hoja-esc-cal-usa-0001)
  - [Hoja: ESC-CAL-USA-0002](#hoja-esc-cal-usa-0002)
  - [Hoja: ESC-CAL-USA-0003](#hoja-esc-cal-usa-0003)
  - [Hoja: ESC-CAL-USA-0004](#hoja-esc-cal-usa-0004)
  - [Hoja: ESC-CAL-USA-0005](#hoja-esc-cal-usa-0005)
  - [Hoja: ESC-CAL-USA-0006](#hoja-esc-cal-usa-0006)
  - [Hoja: ESC-CAL-SEG-0001](#hoja-esc-cal-seg-0001)
  - [Hoja: ESC-CAL-DIS-0001](#hoja-esc-cal-dis-0001)
  - [Hoja: ESC-CAL-USA-0012](#hoja-esc-cal-usa-0012)
  - [Hoja: ESC-CAL-CAP-0014](#hoja-esc-cal-cap-0014)
- [Restricciones — AGROBODEGA](#restricciones--agrobodega)
  - [Hoja: Restricciones de Negocio](#hoja-restricciones-de-negocio)
  - [Hoja: Restricciones Técnicas](#hoja-restricciones-técnicas)
  - [Hoja: Funcionalidades Críticas](#hoja-funcionalidades-críticas)
- [Documentación Elementos Arquitectónicos](#documentación-elementos-arquitectónicos)
  - [Hoja: Elementos Arquitectónicos](#hoja-elementos-arquitectónicos)
  - [Hoja: Plataforma Tecnológica](#hoja-plataforma-tecnológica)

---

## Portada

[🔼 Volver al índice](#índice)

**Proyecto:** AGROBODEGA
**Autores:** [Nombre 1] y [Nombre 2] — Universidad Católica de Oriente
**Documento consolidado:** Documentación completa de arquitectura del sistema AGROBODEGA
**Fecha de compilación:** 2026-05-19

---

## Excel AGROBODEGA — Drivers Arquitectónicos

[🔼 Volver al índice](#índice)

---

## Hoja: TRADEOFF

[🔼 Volver al índice](#índice)

Matriz de intercambio (tradeoff) que establece el orden de prioridad de los atributos de calidad según la perspectiva de cada rol del sistema. El número más bajo indica mayor prioridad.

| Atributo de Calidad | Adm. Bodega | Propietario | Adm. Sistema |
|---|---|---|---|
| Usabilidad | 1 | 4 | 13 |
| Disponibilidad | 2 | 2 | 9 |
| Rendimiento | 4 | 5 | 10 |
| Accesibilidad | 5 | 7 | 14 |
| Seguridad | 8 | 8 | 1 |
| Capacidad para ser administrado | 9 | 11 | 6 |
| Confiabilidad | 3 | 3 | 5 |
| Capacidad para ser soportado | 10 | 12 | 4 |
| Capacidad para ser probado | 7 | 9 | 8 |
| Capacidad | 6 | 6 | 11 |
| Capacidad para ser mantenido | 11 | 13 | 2 |
| Costo | 12 | 1 | 12 |
| Capacidad para ser desplegado | 13 | 14 | 3 |
| Escalabilidad | 14 | 10 | 7 |

---

## Hoja: Mapa de Empatía

[🔼 Volver al índice](#índice)

Ponderación de los atributos de calidad por actor. Los valores ponderados se calculan como la inversión del ranking (15 − ranking), y el porcentaje refleja el peso relativo de cada atributo sobre el total de 315 puntos.

| Atributo de Calidad | Adm. Bodega | Propietario | Adm. Sistema | Adm. Bodega Pond. | Propietario Pond. | Adm. Sistema Pond. | Total Pond. | % |
|---|---|---|---|---|---|---|---|---|
| Usabilidad | 1 | 4 | 13 | 14 | 11 | 2 | 27 | 8,57% |
| Rendimiento | 4 | 5 | 10 | 10 | 10 | 5 | 25 | 7,94% |
| Disponibilidad | 2 | 2 | 9 | 12 | 13 | 6 | 31 | 9,84% |
| Seguridad | 8 | 8 | 1 | 6 | 7 | 14 | 27 | 8,57% |
| Escalabilidad | 14 | 10 | 7 | 0 | 5 | 8 | 13 | 4,13% |
| Capacidad para ser mantenido | 11 | 13 | 2 | 3 | 2 | 13 | 18 | 5,71% |
| Capacidad para ser administrado | 9 | 11 | 6 | 5 | 4 | 9 | 18 | 5,71% |
| Capacidad para ser soportado | 10 | 12 | 4 | 4 | 3 | 11 | 18 | 5,71% |
| Costo | 12 | 1 | 12 | 2 | 14 | 3 | 19 | 6,03% |
| Capacidad para ser desplegado | 13 | 14 | 3 | 1 | 1 | 12 | 14 | 4,44% |
| Accesibilidad | 5 | 7 | 14 | 9 | 8 | 1 | 18 | 5,71% |
| Confiabilidad | 3 | 3 | 5 | 11 | 12 | 10 | 33 | 10,48% |
| Capacidad para ser probado | 7 | 9 | 8 | 7 | 6 | 7 | 20 | 6,35% |
| Capacidad | 6 | 6 | 11 | 8 | 9 | 4 | 21 | 6,67% |
| **Total** | **105** | **105** | **105** | | | | **315** | **100%** |

---

## Hoja: Caracterización

[🔼 Volver al índice](#índice)

Tabla completa de caracterización de atributos de calidad con sus escenarios asociados. El sistema cuenta con **284 escenarios de calidad** distribuidos entre los 14 atributos priorizados.

| Atributo de Calidad | Escenarios totales |
|---|---|
| Confiabilidad | 23 |
| Disponibilidad | 8 |
| Usabilidad | 32 |
| Rendimiento | 32 |
| Seguridad | 23 |
| Escalabilidad | 8 |
| Capacidad para ser mantenido | 10 |
| Capacidad para ser administrado | 13 |
| Capacidad para ser desplegado | 17 |
| Accesibilidad | 22 |
| Capacidad para ser probado | 16 |
| Capacidad | 18 |
| Capacidad para ser soportado | 29 |
| Costo | 33 |

A continuación se presentan los primeros escenarios de cada atributo como muestra representativa:

| Atributo de Calidad | Código Característica | Descripción Característica | Categoría | Código Escenario | Descripción Escenario |
|---|---|---|---|---|---|
| Capacidad para ser soportado | CAR-CS-0001 | Se debe asegurar que el sistema registre automáticamente los errores que ocurran durante su funcionamiento con el fin de facilitar su diagnóstico y corrección por parte del equipo de soporte. | Registro de errores | ESC-CAL CS 0001 | Registro de error durante operación del sistema. |
| Capacidad para ser soportado | CAR-CS-0001 | Se debe asegurar que el sistema registre automáticamente los errores que ocurran durante su funcionamiento con el fin de facilitar su diagnóstico y corrección por parte del equipo de soporte. | Registro de errores | ESC-CAL CS 0002 | Registro de error al guardar una entrada de inventario. |
| Capacidad para ser soportado | CAR-CS-0001 | Se debe asegurar que el sistema registre automáticamente los errores que ocurran durante su funcionamiento con el fin de facilitar su diagnóstico y corrección por parte del equipo de soporte. | Registro de errores | ESC-CAL CS 0003 | Registro de error al registrar una salida de producto. |
| Capacidad para ser soportado | CAR-CS-0002 | Se debe asegurar que el sistema permita identificar fácilmente el origen de los errores que ocurran durante su operación para facilitar su análisis. | Diagnóstico de errores | ESC-CAL CS 0004 | Identificación del módulo donde ocurrió un error. |
| Capacidad para ser soportado | CAR-CS-0002 | Se debe asegurar que el sistema permita identificar fácilmente el origen de los errores que ocurran durante su operación para facilitar su análisis. | Diagnóstico de errores | ESC-CAL CS 0005 | Consulta de información técnica de un error registrado. |
| Capacidad para ser soportado | CAR-CS-0003 | Se debe asegurar que el sistema mantenga un historial de eventos y operaciones realizadas por los usuarios para facilitar la revisión de incidentes. | Auditoría / trazabilidad | ESC-CAL CS 0006 | Registro de operación realizada por un usuario. |
| Capacidad para ser soportado | CAR-CS-0003 | Se debe asegurar que el sistema mantenga un historial de eventos y operaciones realizadas por los usuarios para facilitar la revisión de incidentes. | Auditoría / trazabilidad | ESC-CAL CS 0007 | Consulta del historial de operaciones del sistema. |
| Capacidad para ser soportado | CAR-CS-0003 | Se debe asegurar que el sistema mantenga un historial de eventos y operaciones realizadas por los usuarios para facilitar la revisión de incidentes. | Auditoría / trazabilidad | ESC-CAL CS 0008 | Consulta del historial de movimientos de inventario. |
| Capacidad para ser soportado | CAR-CS-0003 | Se debe asegurar que el sistema mantenga un historial de eventos y operaciones realizadas por los usuarios para facilitar la revisión de incidentes. | Auditoría / trazabilidad | ESC-CAL CS 0009 | Consulta del historial de accesos al sistema. |
| Capacidad para ser soportado | CAR-CS-0003 | Se debe asegurar que el sistema mantenga un historial de eventos y operaciones realizadas por los usuarios para facilitar la revisión de incidentes. | Auditoría / trazabilidad | ESC-CAL CS 0010 | Consulta del historial de registros de entradas y salidas. |
| Usabilidad | CAR-USA-0001 | Se debe asegurar que el sistema permita registrar información básica del negocio de manera clara, intuitiva y comprensible para los usuarios. | Facilidad de uso | ESC-CAL USA 0001 | Registro correcto de un producto base con datos válidos. |
| Usabilidad | CAR-USA-0001 | Se debe asegurar que el sistema permita registrar información básica del negocio de manera clara, intuitiva y comprensible para los usuarios. | Facilidad de uso | ESC-CAL USA 0002 | Registro correcto de una clasificación asociada a un producto base. |
| Usabilidad | CAR-USA-0001 | Se debe asegurar que el sistema permita registrar información básica del negocio de manera clara, intuitiva y comprensible para los usuarios. | Facilidad de uso | ESC-CAL USA 0003 | Registro correcto de un cosechero. |
| Usabilidad | CAR-USA-0001 | Se debe asegurar que el sistema permita registrar información básica del negocio de manera clara, intuitiva y comprensible para los usuarios. | Facilidad de uso | ESC-CAL USA 0004 | Registro correcto de un negociante. |
| Usabilidad | CAR-USA-0001 | Se debe asegurar que el sistema permita registrar información básica del negocio de manera clara, intuitiva y comprensible para los usuarios. | Facilidad de uso | ESC-CAL USA 0005 | Registro correcto de una entrada de inventario. |
| Usabilidad | CAR-USA-0001 | Se debe asegurar que el sistema permita registrar información básica del negocio de manera clara, intuitiva y comprensible para los usuarios. | Facilidad de uso | ESC-CAL USA 0006 | Registro correcto de una salida de inventario. |
| Usabilidad | CAR-USA-0001 | Se debe asegurar que el sistema permita registrar información básica del negocio de manera clara, intuitiva y comprensible para los usuarios. | Facilidad de uso | ESC-CAL USA 0007 | Intento inválido de registrar un producto base con nombre vacío. |
| Usabilidad | CAR-USA-0001 | Se debe asegurar que el sistema permita registrar información básica del negocio de manera clara, intuitiva y comprensible para los usuarios. | Facilidad de uso | ESC-CAL USA 0008 | Intento inválido de registrar una entrada sin seleccionar producto base. |

---

## Hoja: Primera Ronda de Votación

[🔼 Volver al índice](#índice)

Primera ronda de votación para seleccionar los escenarios de calidad más representativos por actor (Administrador de Bodega, Propietario de Bodega, Administrador de Sistema). De los 284 escenarios totales de la caracterización, cada actor votó los que consideraba más críticos para el negocio.

> Esta hoja contiene los mismos escenarios de la Caracterización con las columnas de votación de cada actor. Los escenarios con al menos un voto pasaron a la Segunda Votación.

---

## Hoja: Segunda Votación

[🔼 Volver al índice](#índice)

Segunda ronda de votación con los escenarios preseleccionados en la primera ronda. Contiene 114 escenarios que quedaron como los más relevantes para el sistema según los tres actores del negocio. Estos escenarios priorizados son la base para las decisiones arquitectónicas del sistema.

---

## Hoja: ESC-CAL-USA-0001

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-USA-0001
**Nombre:** Registrar producto base correctamente

**Objetivo:** Asegurar que el sistema AGROBODEGA permita registrar productos base de forma correcta, almacenando la información ingresada por el usuario y dejándola disponible para su uso en los procesos de inventario.

**Criterio de éxito:** El producto base se registra correctamente en el sistema y queda disponible para ser utilizado en operaciones posteriores del inventario.

**Prerequisitos:**
1. El usuario debe estar registrado en el sistema.
2. El usuario debe haber iniciado sesión en el sistema.
3. El usuario debe tener acceso al módulo de productos base.
4. El sistema debe estar en funcionamiento y conectado a la base de datos.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Ingresar el nombre de un producto base y presionar el botón guardar | Operación normal del sistema en ambiente productivo | Sistema | El sistema valida los datos ingresados y registra el producto base | El producto base queda almacenado en la base de datos y aparece en la lista de productos registrados |

---

## Hoja: ESC-CAL-USA-0002

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-USA-0002
**Nombre:** Registrar clasificación de producto base

**Objetivo:** Asegurar que el sistema permita registrar clasificaciones asociadas a los productos base, permitiendo organizar y categorizar los productos dentro del sistema.

**Criterio de éxito:** La clasificación queda asociada correctamente al producto base seleccionado.

**Prerequisitos:**
1. El usuario debe estar registrado en el sistema.
2. El usuario debe haber iniciado sesión en el sistema.
3. Debe existir al menos un producto base registrado.
4. El usuario debe tener acceso al módulo de clasificación.
5. El sistema debe estar en funcionamiento y conectado a la base de datos.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Seleccionar un producto base y registrar una nueva clasificación | Operación normal en ambiente productivo | Sistema | El sistema valida la información y guarda la clasificación | La clasificación aparece registrada y disponible para el registro de entradas |

---

## Hoja: ESC-CAL-USA-0003

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-USA-0003
**Nombre:** Registrar cosechero correctamente

**Objetivo:** Asegurar que el sistema permita registrar correctamente la información de los cosecheros que participan en la operación de la bodega.

**Criterio de éxito:** La información del cosechero se registra correctamente y queda disponible para su uso en el registro de entradas de inventario.

**Prerequisitos:**
1. El usuario debe estar registrado en el sistema.
2. El usuario debe haber iniciado sesión en el sistema.
3. El usuario debe tener acceso al módulo de cosecheros.
4. El sistema debe estar en funcionamiento y conectado a la base de datos.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Registrar los datos de un cosechero y presionar guardar | Operación normal en ambiente productivo | Sistema | El sistema valida los datos y guarda el registro | El cosechero aparece en el listado disponible para registrar entradas |

---

## Hoja: ESC-CAL-USA-0004

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-USA-0004
**Nombre:** Registrar negociante correctamente

**Objetivo:** Asegurar que el sistema permita registrar correctamente la información de los negociantes asociados a la operación de la bodega.

**Criterio de éxito:** El negociante se registra correctamente y queda disponible para su uso en el registro de salidas de inventario.

**Prerequisitos:**
1. El usuario debe estar registrado en el sistema.
2. El usuario debe haber iniciado sesión en el sistema.
3. El usuario debe tener acceso al módulo de negociantes.
4. El sistema debe estar en funcionamiento y conectado a la base de datos.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Registrar los datos de un negociante | Operación normal en ambiente productivo | Sistema | El sistema valida la información y guarda el registro | El negociante queda registrado y disponible para registrar salidas |

---

## Hoja: ESC-CAL-USA-0005

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-USA-0005
**Nombre:** Registro correcto de una entrada de inventario

**Objetivo:** Asegurar que el sistema AGROBODEGA registre correctamente las entradas de productos al inventario de la bodega, garantizando que la información ingresada por el usuario se almacene de forma consistente y actualice adecuadamente el inventario disponible.

**Criterio de éxito:** La entrada de inventario se registra exitosamente en el sistema, el inventario disponible se actualiza correctamente y el movimiento queda registrado en el historial de operaciones.

**Prerequisitos:**
1. El usuario debe haber iniciado sesión en el sistema.
2. El usuario debe tener permisos para registrar movimientos de inventario.
3. El producto debe estar previamente registrado en el sistema.
4. El sistema debe tener conexión con la base de datos.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Registrar una entrada de producto indicando producto, cantidad, lote y cosechero | Operación normal del sistema durante la gestión diaria de inventario | Sistema | El sistema valida los datos ingresados, registra la entrada en la base de datos, actualiza el inventario disponible y guarda el movimiento en el historial | La operación se registra correctamente y el inventario refleja el nuevo dato sin inconsistencias |

---

## Hoja: ESC-CAL-USA-0006

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-USA-0006
**Nombre:** Registro correcto de una salida de inventario

**Objetivo:** Asegurar que el sistema AGROBODEGA registre correctamente las salidas de productos del inventario de la bodega, garantizando que la información ingresada por el usuario se procese de forma correcta y se actualice el inventario disponible.

**Criterio de éxito:** La salida de inventario se registra correctamente, el sistema descuenta la cantidad correspondiente del inventario disponible y el movimiento queda registrado en el historial de operaciones.

**Prerequisitos:**
1. El usuario debe haber iniciado sesión en el sistema.
2. El usuario debe tener permisos para registrar salidas de inventario.
3. El producto debe estar previamente registrado en el sistema.
4. Debe existir inventario disponible del producto.
5. El sistema debe tener conexión con la base de datos.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Registrar una salida de producto indicando producto, cantidad, lote y destino | Operación normal del sistema durante la gestión diaria de inventario | Sistema | El sistema valida los datos ingresados, verifica que exista inventario suficiente, registra la salida en la base de datos, actualiza el inventario disponible y guarda el movimiento en el historial | La salida se registra correctamente, el inventario se reduce de forma consistente y el historial refleja el movimiento realizado |

---

## Hoja: ESC-CAL-SEG-0001

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-SEG-0001
**Nombre:** Inicio de sesión correcto con credenciales válidas

**Objetivo:** Asegurar que el sistema AGROBODEGA permita a los usuarios autenticarse correctamente mediante credenciales válidas, garantizando el acceso seguro a las funcionalidades del sistema según el rol asignado por el administrador.

**Criterio de éxito:** El usuario ingresa sus credenciales válidas, el sistema valida la información, inicia la sesión correctamente y permite el acceso a las funcionalidades correspondientes a su rol.

**Prerequisitos:**
1. El administrador del sistema debe haber creado previamente la cuenta del usuario.
2. El usuario debe tener un rol asignado dentro del sistema.
3. La cuenta del usuario debe estar activa y vigente.
4. El usuario no debe tener una sesión activa en el sistema.
5. El sistema debe estar disponible y conectado a la base de datos.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Ingresar credenciales válidas en el formulario de inicio de sesión | Operación normal del sistema durante el acceso a la plataforma web | Sistema | El sistema valida las credenciales ingresadas, autentica al usuario, inicia la sesión y redirige al panel principal según el rol asignado | El usuario accede correctamente al sistema y puede utilizar las funcionalidades correspondientes a su rol |

---

## Hoja: ESC-CAL-DIS-0001

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-DIS-0001
**Nombre:** Acceso correcto al sistema en cualquier momento del día para consultar o registrar información

**Objetivo:** Asegurar que el sistema AGROBODEGA esté disponible para los usuarios autorizados en cualquier momento del día, permitiendo consultar información y registrar operaciones de inventario sin interrupciones.

**Criterio de éxito:** Los usuarios pueden acceder al sistema, iniciar sesión y utilizar sus funcionalidades principales para consultar o registrar información sin que el sistema presente indisponibilidad.

**Prerequisitos:**
1. El sistema debe estar desplegado y en ejecución en el servidor.
2. La base de datos del sistema debe estar disponible.
3. El usuario debe tener una cuenta registrada en el sistema.
4. El usuario debe contar con credenciales válidas para iniciar sesión.
5. El usuario debe tener conexión a internet para acceder al sistema.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Acceder al sistema para consultar inventario o registrar movimientos | Operación normal del sistema durante cualquier momento de la jornada laboral | Sistema | El sistema permite el acceso al sistema, autenticación del usuario y utilización de las funcionalidades de consulta o registro de inventario | El sistema responde correctamente permitiendo realizar consultas o registros sin presentar fallos o interrupciones |

---

## Hoja: ESC-CAL-USA-0012

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-USA-0012
**Nombre:** Consulta correcta del historial de movimientos del inventario de forma comprensible

**Objetivo:** Asegurar que el sistema AGROBODEGA permita a los usuarios consultar el historial de movimientos del inventario de manera clara, organizada y comprensible, facilitando el seguimiento de las operaciones realizadas en la bodega.

**Criterio de éxito:** El sistema muestra correctamente el historial de movimientos de inventario, incluyendo información relevante como producto, tipo de movimiento, cantidad, fecha y usuario responsable.

**Prerequisitos:**
1. El usuario debe estar registrado en el sistema.
2. El usuario debe tener permisos para consultar información del inventario.
3. Deben existir registros previos de entradas o salidas de inventario en el sistema.
4. El usuario debe haber iniciado sesión en el sistema.
5. El sistema debe tener conexión con la base de datos.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de bodega o propietario de bodega | Solicitar la consulta del historial de movimientos de inventario | Operación normal del sistema durante la gestión diaria de inventario | Sistema | El sistema recupera la información almacenada de los movimientos de inventario y la presenta al usuario de forma organizada y comprensible | El usuario puede visualizar correctamente el historial de movimientos del inventario con la información clara y sin inconsistencias |

---

## Hoja: ESC-CAL-CAP-0014

[🔼 Volver al índice](#índice)

**Código:** ESC-CAL-CAP-0014
**Nombre:** Incremento en la cantidad de cosecheros y negociantes asociados a la operación

**Objetivo:** Asegurar que el sistema AGROBODEGA pueda gestionar un incremento en la cantidad de cosecheros y negociantes registrados, permitiendo almacenar y consultar su información sin afectar el funcionamiento del sistema.

**Criterio de éxito:** El sistema permite registrar nuevos cosecheros y negociantes y consultar su información correctamente, manteniendo la integridad y disponibilidad de los datos.

**Prerequisitos:**
1. El usuario debe estar autenticado en el sistema.
2. El usuario debe tener permisos para registrar o consultar terceros.
3. El sistema debe estar conectado a la base de datos.
4. El módulo de gestión de terceros debe estar disponible en el sistema.

| Fuente del estímulo | Estímulo | Ambiente | Artefacto | Respuesta | Medida de la respuesta |
|---|---|---|---|---|---|
| Usuario del sistema: Administrador de sistema | Registrar o consultar información de nuevos cosecheros o negociantes | Operación normal del sistema durante la gestión de información de terceros | Sistema | El sistema permite registrar nuevos terceros y almacenar su información correctamente, permitiendo su consulta posterior | El sistema registra y consulta la información de múltiples cosecheros y negociantes sin afectar el funcionamiento del sistema |

---

## Restricciones — AGROBODEGA

[🔼 Volver al índice](#índice)

---

## Hoja: Restricciones de Negocio

[🔼 Volver al índice](#índice)

| Tipo | Restricción de Negocio | Justificación | Plan de Acción |
|---|---|---|---|
| Humano | El propietario de la bodega no participa de manera constante en las operaciones diarias, ya que su enfoque principal está en la supervisión de ingresos, gastos, inventario consolidado y rentabilidad del negocio. | El propietario requiere tener control del negocio y acceso a información clave sin involucrarse en las operaciones diarias. | Definir funcionalidades orientadas a la supervisión, como reportes, alertas e indicadores, separándolas de las tareas operativas del sistema. |
| Tiempo | En AGROBODEGA, las entradas y salidas deben registrarse en el momento en que ocurren, ya que el negocio depende de saber qué producto entró, de qué cosechero proviene, en qué lote quedó y cuánto stock sale hacia cada negociante. | La operación de la bodega depende de conocer en tiempo real los movimientos de inventario para evitar errores, pérdidas y descontrol en los productos. | Definir como regla de negocio que ningún movimiento quede pendiente por registrar y diseñar el sistema para capturar rápidamente los datos. |
| Legal | AGROBODEGA maneja información personal de cosecheros, negociantes y usuarios, por lo que debe cumplir con la normativa colombiana de protección de datos (Ley 1581). | El manejo inadecuado de datos puede generar sanciones legales y pérdida de confianza. | Definir políticas de tratamiento de datos y restringir el acceso a la información según el rol del usuario. |
| Presupuesto | El proyecto tiene un presupuesto de $10.000.000 COP para el desarrollo, puesta en producción, mantenimiento y soporte del producto por el siguiente 1 año. | El propietario de la bodega cuenta con un presupuesto definido para el desarrollo de AGROBODEGA, por lo que el sistema debe planificarse dentro de este límite, garantizando la viabilidad del proyecto. | Se llevará a cabo una planificación inicial de los costos y un monitoreo continuo del uso de recursos, con el fin de mantener el proyecto dentro del presupuesto asignado. |
| Humano | Los usuarios del sistema presentan diferentes niveles de experiencia tecnológica, lo que puede dificultar su uso si el sistema es complejo. | Una alta complejidad puede afectar la adopción del sistema y generar errores en la operación. | Diseñar procesos estructurados con campos definidos y flujos de operación que guíen el registro de entradas, salidas y consultas de inventario. |
| Humano | No todos los usuarios del sistema realizan las mismas funciones dentro de la bodega, por lo que las operaciones deben corresponder a su rol. | Evita el uso indebido del sistema y reduce errores en la operación del negocio. | Definir roles de usuario y establecer qué operaciones puede realizar cada uno dentro del sistema. |
| Presupuesto | Cualquier costo adicional no contemplado dentro del presupuesto inicial debe contar con aprobación previa del propietario de la bodega. | Los costos no previstos pueden afectar el control financiero del proyecto y generar sobrecostos que superen la capacidad de pago. | Definir un procedimiento para la solicitud, evaluación y aprobación de costos adicionales durante el desarrollo del proyecto. |
| Humano | El equipo de desarrollo está conformado por dos estudiantes universitarios con carga académica activa, lo que limita la disponibilidad de tiempo para el desarrollo y atención de incidencias. | La disponibilidad parcial del equipo puede afectar los tiempos de desarrollo, entrega de funcionalidades y resolución de problemas durante el proyecto. | Definir un cronograma realista, priorizar funcionalidades clave del sistema y establecer tiempos de respuesta acordes a la disponibilidad del equipo. |

---

## Hoja: Restricciones Técnicas

[🔼 Volver al índice](#índice)

| Tipo | Restricción Técnica | Justificación |
|---|---|---|
| Prácticas de diseño | El diseño y desarrollo del software debe propender por seguir los principios SOLID. | Aplicar SOLID garantiza que AGROBODEGA pueda mantenerse modular, mantenible y extensible a lo largo del tiempo, lo cual es importante en un sistema donde módulos como inventario, entradas, salidas y reportes pueden seguir creciendo. |
| Prácticas de diseño | Se busca propender por la aplicación de principios de bajo acoplamiento y alta cohesión en los componentes del sistema. | Aplicar principios de bajo acoplamiento y alta cohesión permite que los módulos de AGROBODEGA funcionen de manera independiente, facilitando su mantenimiento y evolución. |
| Prácticas de diseño | Se debe propender por la implementación de una arquitectura por capas que separe la lógica de negocio, la presentación y el acceso a datos. | Implementar una arquitectura por capas permite que en AGROBODEGA la lógica de negocio, como el control de inventario, entradas y salidas, se mantenga separada de la interfaz y del acceso a datos, facilitando su mantenimiento y evolución. |
| Prácticas de diseño | Propender por el uso de patrones de diseño y de implementación como por ejemplo patrones GoF, GRASP, DRY, KISS. | Propender por la adopción de patrones de diseño permite que en AGROBODEGA funcionalidades como inventario, entradas, salidas y reportes se desarrollen siguiendo estructuras organizadas y reutilizables. |
| Prácticas de código limpio | Se debe propender por aplicación de prácticas de código limpio (Clean Code), evitando Messy Code y Code Smells. | Aplicar prácticas de código limpio permite que en AGROBODEGA el código relacionado con procesos como inventario, entradas, salidas y reportes sea claro y entendible para el equipo de desarrollo. |
| Prácticas DevOps | Se plantea la adopción de prácticas DevOps para la integración, despliegue y monitoreo del sistema. | Propender por la adopción de prácticas DevOps permite que en AGROBODEGA los cambios en funcionalidades como inventario, entradas, salidas y reportes se integren y desplieguen de forma controlada. |
| Prácticas DevOps | Propender por la adopción de los 12 factores de aplicación (más los 3 extendidos). | Adoptar los principios de los 12 factores de aplicación permite que en AGROBODEGA el sistema sea más organizado, configurable y fácil de desplegar en diferentes entornos. |
| Implementación | Propender por la adopción de una metodología ágil como Scrum para la gestión del desarrollo del proyecto, complementada con prácticas de desarrollo orientadas a la calidad del código. | La adopción de Scrum permite organizar el desarrollo de AGROBODEGA en iteraciones, facilitando la entrega progresiva de funcionalidades como inventario, entradas y salidas. |
| Implementación | Propender por la implementación de mecanismos de seguridad para el control de acceso y protección de la información. | Implementar mecanismos de seguridad permite que en AGROBODEGA el acceso a funcionalidades como inventario, entradas, salidas y reportes esté controlado según el rol del usuario. |
| Prácticas de desarrollo | Propender por la adopción de buenas prácticas en la estructuración y desarrollo del sistema. | Permite que en AGROBODEGA el desarrollo de funcionalidades como inventario, entradas, salidas y reportes se realice de forma organizada, facilitando su mantenimiento y evolución. |
| Prácticas de desarrollo | Propender por la implementación de pruebas durante el desarrollo del sistema. | Implementar pruebas durante el desarrollo permite que en AGROBODEGA funcionalidades como el registro de entradas, salidas y el control de inventario sean validadas de forma continua. |
| Plataforma | Propender por el uso de tecnologías de bases de datos relacionales que soporten el manejo de información transaccional del sistema. | El uso de bases de datos relacionales permite que en AGROBODEGA los procesos de inventario, entradas y salidas mantengan consistencia entre entidades como productos, lotes, cosecheros y negociantes. |

---

## Hoja: Funcionalidades Críticas

[🔼 Volver al índice](#índice)

| Identificador | Requisito Funcional | Justificación | Táctica | Descripción Estrategia |
|---|---|---|---|---|
| RF-16 | El sistema debe permitir registrar una entrada con: producto base, clasificación, cosechero, cantidad, lote y fecha. | Es fundamental registrar correctamente las entradas de productos, ya que estas representan el ingreso físico de mercancía a la bodega. Si no se realiza este registro, el inventario no reflejaría la realidad, afectando el control operativo y financiero del sistema. | Operación transaccional de registro de entradas | Se implementa una operación transaccional en la capa de servicio que valida los datos de entrada y registra el movimiento en la base de datos, garantizando consistencia entre el inventario y el ingreso físico de productos. |
| RF-17 | Al registrar una entrada válida, el sistema debe crear el lote y aumentar el inventario. | Es importante que el sistema automatice la creación del lote y la actualización del inventario, porque esto garantiza la trazabilidad de los productos y evita inconsistencias en el stock. | Gestión automática de lote e inventario | Al registrar una entrada válida, el sistema ejecuta automáticamente la creación del lote y la actualización del inventario dentro de una misma operación, garantizando trazabilidad y consistencia en los datos. |
| RF-18 | El sistema debe permitir registrar el cobro por entrada y asociarlo a la entrada correspondiente. | Es necesario registrar los cobros por entrada, ya que estos representan ingresos del servicio de almacenamiento. Asociarlos correctamente permite llevar un control financiero claro y evitar inconsistencias en los reportes económicos. | Asociación transaccional de cobro a entrada | El sistema registra el cobro únicamente si existe una entrada válida, vinculando ambas operaciones dentro de una misma lógica de negocio. Esto permite mantener consistencia entre los movimientos de inventario y los ingresos generados. |
| RF-22 | El sistema debe permitir registrar una salida con: lote seleccionado, cantidad, negociante y fecha. | Registrar las salidas es esencial para reflejar la entrega de productos. Sin este proceso, el sistema no podría controlar qué productos han salido de la bodega, generando desorden en el inventario. | Registro validado de salidas | Cada salida es registrada mediante validaciones en la capa de servicio que garantizan la existencia del lote, la cantidad solicitada y el tercero asociado, asegurando un control adecuado de los productos entregados. |
| RF-23 | Al registrar una salida, el sistema debe descontar automáticamente el stock del lote seleccionado. | Es importante que el sistema actualice automáticamente el inventario al registrar una salida, ya que esto evita errores humanos y mantiene la información actualizada en tiempo real. | Actualización automática de stock | Al registrar una salida, el sistema descuenta automáticamente la cantidad correspondiente del lote seleccionado, manteniendo la información del inventario actualizada y consistente en todo momento. |
| RF-24 | El sistema debe bloquear salidas cuando la cantidad solicitada supere el stock del lote y evitar stock negativo. | Es fundamental que el sistema valide la disponibilidad del producto antes de permitir una salida, ya que registrar cantidades superiores al stock generaría inconsistencias y pérdida de confiabilidad en el sistema. | Validación transaccional de stock | Antes de registrar una salida, el sistema valida que la cantidad solicitada no supere el stock disponible. La operación se ejecuta de forma transaccional, garantizando que no se generen inventarios negativos ni inconsistencias en la información. |
| RF-25 | El sistema debe permitir registrar el cobro por salida y asociarlo a la salida correspondiente. | Registrar los cobros por salida es clave para reflejar los ingresos generados por la operación. Asociarlos correctamente permite calcular ingresos, utilidades y tomar decisiones financieras. | Asociación de cobro a salida | El registro del cobro se realiza como una operación dependiente de la existencia de una salida previamente validada, garantizando la vinculación entre el movimiento de inventario y el ingreso generado. |
| RF-06 | El sistema debe permitir registrar productos base. | Es necesario contar con productos base, ya que estos son la base para registrar entradas, salidas, lotes e inventario. Sin ellos, el sistema no podría operar correctamente. | Registro validado de productos base | El sistema implementa validaciones en la capa de servicio para garantizar que los productos base se registren con información completa y consistente. |
| RF-08 | El sistema debe permitir configurar clasificaciones para cada producto base. | Es importante definir clasificaciones para cada producto, ya que esto permite organizar el inventario por tipo, facilitando el control y la trazabilidad de los productos. | Gestión de clasificaciones de productos | El sistema permite definir y asociar clasificaciones a los productos base mediante una estructura controlada, facilitando la organización del inventario. |
| RF-12 | El sistema debe permitir registrar cosecheros con datos básicos. | Es importante registrar los cosecheros, ya que representan el origen de los productos y permiten llevar trazabilidad sobre quién suministró cada lote. | Registro validado de cosecheros | El sistema registra los datos de los cosecheros mediante validaciones que garantizan integridad y consistencia, permitiendo asociarlos correctamente a los lotes. |
| RF-13 | El sistema debe permitir registrar negociantes con datos mínimos (nombre, apellidos y teléfono). | Permite identificar a quién se le realiza la salida de productos, garantizando trazabilidad y control de las operaciones comerciales de la bodega. | Registro validado de negociantes | El sistema gestiona el registro de negociantes asegurando la validez de sus datos, permitiendo asociarlos a las salidas de productos y garantizando trazabilidad. |
| RF-29 | El sistema debe permitir consultar inventario por lotes mostrando producto base, clasificación, cosechero y stock. | Permite conocer el estado real del inventario, facilitando la toma de decisiones y el control de los productos almacenados. | Consulta estructurada de inventario | El sistema implementa consultas estructuradas sobre la base de datos que permiten visualizar el inventario por lotes, integrando información como producto, clasificación, cosechero y stock disponible. |

---

## Documentación Elementos Arquitectónicos

[🔼 Volver al índice](#índice)

---

## Hoja: Elementos Arquitectónicos

[🔼 Volver al índice](#índice)

| Componente / Elemento Arquitectónico | Descripción | Justificación | Tipo Adquisición |
|---|---|---|---|
| Web Application Firewall (WAF) | [Vínculo](https://www.cloudflare.com/es-es/learning/ddos/glossary/web-application-firewall-waf/) | Asegura que AGROBODEGA cuente con una capa de protección como primera línea de defensa frente a ataques comunes en aplicaciones web, como inyección SQL, XSS, tráfico malicioso o accesos no autorizados, permitiendo filtrar y analizar las solicitudes HTTPS antes de que lleguen al backend y protegiendo así la información sensible del sistema. Drivers: Seguridad, Disponibilidad, Confiabilidad, Capacidad para ser soportado. | Adoptado |
| API Gateway | [Vínculo](https://konghq.com/products/kong-gateway) | Asegura que AGROBODEGA cuente con un punto de entrada centralizado para las solicitudes hacia sus servicios, permitiendo gestionar de forma ordenada el acceso a las APIs REST del sistema, aplicar controles de autenticación y autorización, manejar versionamiento, limitar peticiones y evitar la exposición directa de los servicios internos. Drivers: Seguridad, Disponibilidad, Rendimiento, Capacidad para ser administrado, Capacidad para ser soportado. | Adoptado |
| Identity Provider | [Vínculo](https://auth0.com/docs/get-started/identity-fundamentals/identity-and-access-management) | Asegura que AGROBODEGA cuente con un mecanismo centralizado para la autenticación y gestión de identidad de los usuarios del sistema, permitiendo controlar el acceso mediante credenciales seguras, tokens y roles definidos. Drivers: Seguridad, Confiabilidad, Capacidad para ser administrado, Capacidad para ser soportado, Usabilidad. | Adoptado |
| Key Vault | [Vínculo](https://developer.hashicorp.com/vault/docs/what-is-vault) | Asegura que AGROBODEGA cuente con un mecanismo seguro y centralizado para almacenar y administrar secretos de la aplicación como credenciales de base de datos, claves de API, certificados y tokens, evitando que esta información quede expuesta en el código fuente o repositorios. Drivers: Seguridad, Confiabilidad, Capacidad para ser administrado, Capacidad para ser soportado. | Adoptado |
| Cache de Datos | [Vínculo](https://redis.io/docs/latest/develop/get-started/) | Asegura que AGROBODEGA mejore el rendimiento del sistema mediante el almacenamiento temporal de información que se consulta con alta frecuencia, como inventario por lotes, productos base, clasificaciones y parámetros de negocio, evitando consultas repetitivas a la base de datos. Drivers: Rendimiento, Disponibilidad, Capacidad, Capacidad para ser soportado, Escalabilidad. | Adoptado |
| Databases | [Vínculo](https://www.postgresql.org/about/) | Asegura que AGROBODEGA cuente con un mecanismo persistente, estructurado y confiable para almacenar la información principal del sistema, garantizando integridad referencial, consistencia en las operaciones transaccionales y trazabilidad de los movimientos registrados en la bodega. Drivers: Confiabilidad, Seguridad, Capacidad, Capacidad para ser administrado, Capacidad para ser soportado. | Adoptado |
| Notification Gateway | [Vínculo](https://sendgrid.com/en-us/solutions/email-api/) | Asegura que AGROBODEGA cuente con un mecanismo centralizado para el envío de notificaciones a los usuarios del sistema, permitiendo comunicar eventos importantes como alertas de inventario, permanencia de lotes en bodega y confirmación de registros. Drivers: Usabilidad, Disponibilidad, Confiabilidad, Capacidad para ser soportado. | Adoptado |
| Parameters Catalog | [Vínculo](https://docs.spring.io/spring-cloud-config/docs/current/reference/html/) | Asegura que AGROBODEGA cuente con un mecanismo centralizado para administrar valores configurables del sistema, como porcentajes de comisión por entrada y salida, umbrales de permanencia de lotes y configuraciones generales, permitiendo modificar reglas de negocio sin cambiar el código fuente. Drivers: Capacidad para ser administrado, Capacidad para ser soportado, Capacidad para ser desplegado, Capacidad para ser mantenido, Usabilidad. | Adoptado |
| Message Catalog | [Vínculo](https://docs.strapi.io/dev-docs/intro) | Asegura que AGROBODEGA cuente con un mecanismo centralizado para administrar los mensajes mostrados a los usuarios, como errores de validación, confirmaciones y alertas operativas, sin necesidad de modificar el código fuente. Drivers: Usabilidad, Capacidad para ser administrado, Capacidad para ser soportado, Capacidad para ser probado. | Adoptado |
| Notification Catalog | [Vínculo](https://docs.strapi.io/dev-docs/intro) | Asegura que AGROBODEGA cuente con un mecanismo centralizado para definir, administrar y parametrizar los tipos de notificaciones que puede generar el sistema, como alertas por stock insuficiente o permanencia de lotes en bodega. Drivers: Usabilidad, Capacidad para ser administrado, Capacidad para ser soportado, Confiabilidad. | Adoptado |
| Instrumentation and Monitoring | [Vínculo](https://opentelemetry.io/docs/what-is-opentelemetry/) | Asegura que AGROBODEGA cuente con un mecanismo centralizado para el monitoreo, registro y trazabilidad de las operaciones del sistema, capturando logs, métricas y trazas de las funcionalidades críticas para facilitar la detección temprana de fallos y la auditoría de eventos. Drivers: Confiabilidad, Capacidad para ser soportado, Capacidad para ser probado, Disponibilidad. | Adoptado |
| CI/CD Pipeline | [Vínculo](https://docs.github.com/en/actions/about-github-actions/understanding-github-actions) | Asegura que AGROBODEGA cuente con un flujo automatizado para la integración, validación y despliegue continuo de la aplicación, reduciendo errores manuales y mejorando la calidad del software. Drivers: Capacidad para ser desplegado, Capacidad para ser probado, Capacidad para ser mantenido, Confiabilidad, Capacidad para ser soportado. | Adoptado |
| Containers (Docker) | [Vínculo](https://docs.docker.com/get-started/docker-overview/) | Asegura que AGROBODEGA pueda ejecutarse en entornos aislados y consistentes mediante el uso de contenedores, facilitando su despliegue en diferentes ambientes como desarrollo, pruebas y producción sin conflictos. Drivers: Capacidad para ser desplegado, Capacidad para ser soportado, Capacidad para ser mantenido, Confiabilidad. | Adoptado |
| Documentación de API | [Vínculo](https://springdoc.org/) | Asegura que AGROBODEGA cuente con una documentación clara, estandarizada y accesible de sus servicios REST, describiendo endpoints, parámetros, respuestas y estructuras de datos de todas las funcionalidades del sistema. Drivers: Capacidad para ser probado, Usabilidad, Capacidad para ser administrado. | Adoptado |
| Autorización de APIs | [Vínculo](https://auth0.com/docs/manage-users/access-control/rbac) | Asegura que AGROBODEGA controle el acceso a sus servicios de acuerdo con los roles y permisos definidos para cada tipo de usuario, restringiendo acciones sobre funcionalidades críticas como reportes de ganancias y configuración del sistema. Drivers: Seguridad, Confiabilidad, Capacidad para ser administrado. | Adoptado |

---

## Hoja: Plataforma Tecnológica

[🔼 Volver al índice](#índice)

| Tipo Adquisición | Componente | Fabricante | Nombre Comercial | Versión | Licenciamiento | Justificación | Motivación |
|---|---|---|---|---|---|---|---|
| Adoptado | Web Application Firewall (WAF) | Cloudflare, Inc. | Cloudflare WAF | Latest | Comercial SaaS (Freemium / Suscripción) | El WAF de Cloudflare se implementa como la primera línea de defensa de AGROBODEGA, inspeccionando y filtrando todo el tráfico HTTP/HTTPS antes de que alcance la aplicación. Su motor de seguridad protege contra inyecciones SQL, XSS, bots maliciosos y ataques DDoS. Al operar desde la red perimetral global de Cloudflare, bloquea amenazas en tiempo real sin introducir latencias significativas. | Garantizar una protección perimetral robusta para AGROBODEGA, previniendo ataques contra la aplicación web y asegurando la continuidad operativa del sistema. Contribuye a los drivers de seguridad, disponibilidad, confiabilidad y escalabilidad. |
| Adoptado | API Gateway | Kong Inc. | Kong Gateway | Latest | Open Source (Apache 2.0) / Enterprise Comercial | Kong Gateway se implementa como la puerta de entrada centralizada para todos los servicios expuestos por AGROBODEGA. Su arquitectura construida sobre NGINX proporciona enrutamiento, autenticación, autorización, limitación de tasa, registro y observabilidad. Compatibilidad nativa con JWT, OAuth 2.0 y OpenID Connect facilita la integración con el proveedor de identidades. | Centralizar el acceso a los servicios de AGROBODEGA mediante un único punto de entrada, fortaleciendo la seguridad, simplificando la gestión del tráfico y mejorando la observabilidad. Contribuye a los drivers de seguridad, escalabilidad, interoperabilidad, mantenibilidad y disponibilidad. |
| Adoptado | Identity Provider | Okta | Auth0 | Latest | Comercial SaaS (Freemium / Suscripción) | Auth0 by Okta se implementa como el proveedor centralizado de identidad y autenticación de AGROBODEGA, gestionando el acceso de los tres roles del sistema. Mediante estándares abiertos como OAuth 2.0, OpenID Connect y JWT, permite que el API Gateway valide cada solicitud. Su plan gratuito incluye hasta 25.000 usuarios activos mensuales, inicio de sesión seguro y tokens de sesión firmados. | Centralizar la gestión de identidad en una plataforma especializada, liberando al equipo de implementar mecanismos de autenticación propios. Contribuye a los drivers de seguridad, confiabilidad, capacidad para ser administrado y usabilidad. |
| Adoptado | Key Vault | HashiCorp (IBM) | HashiCorp Vault Community | Latest | Open Source / Business Source License | HashiCorp Vault Community Edition almacena de forma segura y cifrada todas las credenciales sensibles: conexión a PostgreSQL, tokens de Auth0 y Kong, claves de Redis y SendGrid. Cifra secretos en reposo y en tránsito, provee registro de auditoría de cada acceso y permite rotación automática de credenciales sin modificar el código. | Proteger la información de infraestructura más sensible mediante un mecanismo centralizado, auditable y desacoplado del código fuente. Contribuye a los drivers de seguridad, confiabilidad, capacidad para ser administrado y soportado. |
| Adoptado | Cache de Datos | Redis Ltd / Redis Community | Redis Community Edition | Latest | Open Source (RSALv2 / SSPL) | Redis almacena temporalmente en memoria datos de consulta frecuente: catálogo de productos base, clasificaciones, listas de cosecheros y negociantes, y parámetros de comisión. Evita consultas repetitivas a PostgreSQL durante picos de operación. Spring Data Redis provee integración nativa con Spring Boot. | Reducir la latencia en las operaciones más frecuentes de AGROBODEGA, garantizando respuesta en menos de 3 segundos incluso bajo carga simultánea. Contribuye a los drivers de rendimiento, disponibilidad, capacidad y escalabilidad. |
| Adoptado | Databases | PostgreSQL Global Development Group | PostgreSQL | Latest | Open Source | PostgreSQL 16 almacena toda la información transaccional del sistema. Cumplimiento pleno de propiedades ACID garantiza que operaciones como el registro de una entrada se ejecuten de forma atómica. Soporte para integridad referencial asegura que no existan salidas sin lote asociado. Spring Data JPA provee integración nativa mediante Hibernate. | Garantizar la integridad, consistencia y trazabilidad de toda la información de inventario y operaciones financieras. PostgreSQL es la fuente de verdad del sistema. Contribuye a los drivers de confiabilidad, seguridad, capacidad y capacidad para ser administrado. |
| Adoptado | Notification Gateway | Twilio Inc. | SendGrid | Latest | Freemium (100 emails/día gratis) | SendGrid abstrae del backend toda la complejidad técnica del envío de correos mediante su API REST. Permite enviar alertas de stock insuficiente, permanencia prolongada de lotes y confirmaciones de registro. Plan gratuito de 100 emails diarios es suficiente para el volumen esperado. | Desacoplar la lógica de negocio del mecanismo técnico de envío de notificaciones. Contribuye a los drivers de usabilidad, disponibilidad, confiabilidad y capacidad para ser soportado. |
| Adoptado | Parameters Catalog | VMware / Broadcom (Spring) | Spring Cloud Config Server | Latest | Open Source (Apache 2.0) | Spring Cloud Config Server externaliza del código fuente los valores que gobiernan las reglas de negocio: porcentajes de comisión por entrada y salida, umbrales de días de permanencia de lotes, estados del sistema y límites operativos. Los servicios obtienen dinámicamente estos parámetros al arrancar. Redis los cachea para disponibilidad con latencia mínima. | Permitir ajustar las reglas de negocio sin modificar el código fuente ni desplegar nuevamente la aplicación. Contribuye a los drivers de capacidad para ser administrado, soportado, desplegado y mantenido. |
| Adoptado | Message Catalog | Strapi Solutions SAS | Strapi Community (self-hosted) | Latest | Open Source | Strapi Community self-hosted centraliza todos los textos que AGROBODEGA muestra a los usuarios: mensajes de error de validación, confirmaciones de registro, alertas operativas y respuestas informativas. Cualquier ajuste se realiza desde la interfaz visual de Strapi sin intervención técnica ni redespliegue. | Separar el contenido textual de los mensajes de la lógica de negocio, permitiendo una comunicación clara y fácilmente actualizable. Contribuye a los drivers de usabilidad, capacidad para ser administrado, soportado y probado. |
| Adoptado | Notification Catalog | Strapi Solutions SAS | Strapi Community (self-hosted) | Latest | Open Source | Strapi Community self-hosted define y administra los tipos, plantillas y configuraciones de todas las notificaciones del sistema. El administrador puede ajustar destinatarios, asuntos y cuerpos desde la interfaz sin modificar el código. Las plantillas son consumidas por el Notification Gateway (SendGrid) al enviar cada alerta. | Centralizar la configuración y parametrización de todas las notificaciones, desacoplándolas del backend. Contribuye a los drivers de usabilidad, capacidad para ser administrado, soportado y confiabilidad. |
| Adoptado | Instrumentation and Monitoring | OpenTelemetry / Grafana Labs | OpenTelemetry + Grafana Stack | Latest | Open Source (Apache 2.0) | OpenTelemetry instrumenta el backend Spring Boot para capturar logs estructurados, métricas y trazas distribuidas de operaciones críticas. Grafana visualiza dashboards en tiempo real, Loki centraliza los logs y Tempo gestiona las trazas. Toda la suite corre en el mismo entorno Docker sin costos de licenciamiento. | Garantizar la observabilidad completa de AGROBODEGA en producción, permitiendo detectar y diagnosticar fallos antes de que impacten la operación. Contribuye a los drivers de confiabilidad, capacidad para ser soportado, probado y disponibilidad. |
| Adoptado | CI/CD Pipeline | Microsoft Corporation | GitHub Actions | Latest | Freemium (2.000 min/mes gratis) | GitHub Actions automatiza el ciclo completo de validación: compilación con Maven, ejecución de pruebas unitarias e integración, análisis estático con SonarQube, construcción de imagen Docker y despliegue al entorno de producción. La capa gratuita de 2.000 minutos mensuales es suficiente para el volumen de despliegues del proyecto. | Automatizar el proceso de integración, validación y despliegue, garantizando que cada versión haya pasado por pruebas. Contribuye a los drivers de capacidad para ser desplegado, probado, mantenido, confiabilidad y capacidad para ser soportado. |
| Adoptado | Containers (Docker) | Docker, Inc. | Docker Engine + Docker Compose | Latest | Open Source (Apache 2.0) / Docker Desktop Freemium | Docker Compose orquesta todos los servicios en contenedores aislados: backend Spring Boot, PostgreSQL, Redis, HashiCorp Vault, Spring Cloud Config Server, las dos instancias de Strapi y la suite Grafana. Un único archivo declarativo gestiona el arranque, la red interna y las dependencias entre servicios. | Garantizar que AGROBODEGA pueda desplegarse de forma consistente y portable en cualquier entorno, eliminando conflictos de dependencias. Contribuye a los drivers de capacidad para ser desplegado, soportado, mantenido y confiabilidad. |
| Adoptado | Documentación de API | SmartBear Software | Springdoc OpenAPI (Swagger UI) | Latest | Open Source (Apache 2.0) | Springdoc genera automáticamente la especificación OpenAPI 3.0 de todos los endpoints a partir de las anotaciones del código Spring Boot. Swagger UI expone una interfaz web interactiva para explorar y probar los endpoints directamente desde el navegador. La documentación se actualiza automáticamente con cada cambio en el código. | Proporcionar documentación clara, actualizada y ejecutable de todos los servicios REST, facilitando pruebas y validación durante el desarrollo. Contribuye a los drivers de capacidad para ser probado, usabilidad y capacidad para ser administrado. |
| Adoptado | Autorización de APIs | Auth0 (Okta) / Spring Security | Spring Security + Auth0 RBAC | Latest | Open Source (Apache 2.0) | Spring Security intercepta cada solicitud al backend y valida el token JWT emitido por Auth0, extrayendo el rol del usuario antes de permitir la operación. Garantiza que el administrador de bodega no acceda a reportes de rentabilidad y que ningún usuario no autenticado interactúe con ningún módulo del sistema. | Garantizar que cada usuario acceda únicamente a las funcionalidades de su rol, protegiendo información sensible como reportes de ganancias. Contribuye a los drivers de seguridad, confiabilidad y capacidad para ser administrado. |

---

docs: add arquitectura documentation
