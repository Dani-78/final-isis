CLENA+ — Historias de usuario

1. Objetivo

Las siguientes historias de usuario describen las necesidades principales de los usuarios de CLENA+ y sirven como base para definir las funciones y el diseño de la plataforma de consulta bibliotecaria.

El objetivo es mejorar la organización de la consulta de recursos bibliográficos y facilitar que los usuarios encuentren, comprendan y exploren los resultados.

---

2. Usuario: visitante o usuario de consulta

HU-01 — Buscar un recurso

Como estudiante, docente o usuario de la biblioteca,
quiero realizar una búsqueda mediante palabras clave, título o autor,
para encontrar los recursos bibliográficos que necesito.

Criterios de aceptación:

- El usuario puede realizar una búsqueda desde la página de inicio.
- El usuario puede introducir una palabra clave, título o autor.
- El sistema muestra una pantalla de resultados.
- Si el campo está vacío, el sistema muestra una indicación para realizar una búsqueda válida.
- La búsqueda pública no requiere iniciar sesión.

Interfaz relacionada:

- Inicio.
- Búsqueda general.
- Resultados de búsqueda.

---

HU-02 — Filtrar una búsqueda

Como usuario de la biblioteca,
quiero aplicar filtros a mi búsqueda,
para reducir la cantidad de resultados y encontrar recursos más relevantes.

Criterios de aceptación:

- El usuario puede filtrar por tipo de material.
- El usuario puede filtrar por año de publicación.
- El usuario puede filtrar por idioma.
- El usuario puede filtrar por área temática.
- Los filtros pueden combinarse.
- El usuario puede limpiar los filtros.
- Los filtros aplicados se muestran en los resultados.

Interfaz relacionada:

- Búsqueda avanzada.
- Resultados de búsqueda.

---

HU-03 — Revisar resultados

Como usuario de la biblioteca,
quiero visualizar los resultados de manera clara y organizada,
para comparar las opciones disponibles y seleccionar un recurso.

Criterios de aceptación:

- Cada resultado muestra la información bibliográfica disponible.
- El usuario puede identificar el título del recurso.
- Se muestra el autor cuando está disponible.
- Se muestra el año y tipo de material cuando existen esos datos.
- El usuario puede acceder al detalle de un recurso.
- Si no existen resultados, el sistema proporciona orientación para modificar la búsqueda.

Interfaz relacionada:

- Resultados de búsqueda.

---

HU-04 — Consultar los detalles de un recurso

Como usuario de la biblioteca,
quiero consultar la información detallada de un recurso,
para determinar si es el material que necesito.

Criterios de aceptación:

- Se muestra el título del recurso.
- Se muestra el autor o autores cuando están disponibles.
- Se muestra la información bibliográfica disponible.
- Se muestra una descripción o resumen cuando exista.
- Se muestran los temas relacionados cuando estén disponibles.
- El usuario puede regresar a los resultados.
- La disponibilidad solo se muestra si el sistema bibliotecario proporciona esa información.

Interfaz relacionada:

- Detalle del recurso.

---

HU-05 — Explorar recursos por tema

Como usuario que no conoce un título o autor específico,
quiero explorar los recursos agrupados por temas,
para descubrir materiales relacionados con un área de interés.

Criterios de aceptación:

- El usuario puede acceder a una sección de temas.
- Los temas se muestran de manera organizada.
- El usuario puede seleccionar una categoría.
- Al seleccionar una categoría se muestran los recursos relacionados.
- El usuario puede regresar a la lista de categorías.

Interfaz relacionada:

- Explorar por temas.
- Resultados de búsqueda.

---

HU-06 — Obtener ayuda para realizar una búsqueda

Como usuario de la biblioteca,
quiero encontrar instrucciones y ayuda fácilmente,
para poder utilizar correctamente la plataforma.

Criterios de aceptación:

- Existe una sección de ayuda fácilmente accesible.
- El usuario puede consultar preguntas frecuentes.
- Se muestran instrucciones básicas para realizar búsquedas.
- Se proporciona información de contacto oficial cuando esté disponible.
- Los canales de contacto solo se presentan como disponibles si realmente existen.

Interfaz relacionada:

- Ayuda y contacto.

---

3. Usuario: trabajador o bibliotecario

HU-07 — Acceder a las funciones del personal

Como trabajador autorizado de la biblioteca,
quiero iniciar sesión mediante mis credenciales institucionales,
para acceder a las herramientas internas que correspondan a mi rol.

Criterios de aceptación:

- Existe un acceso separado de la consulta pública.
- El trabajador puede introducir sus credenciales.
- El sistema valida la identidad.
- El sistema verifica los permisos correspondientes.
- Un usuario no autorizado no puede acceder a las funciones internas.
- El usuario puede regresar a la búsqueda pública.

Interfaz relacionada:

- Acceso del personal.
- Panel del personal, si se implementa.

---

4. Historias opcionales

Estas historias deben permanecer como funcionalidades futuras hasta confirmar que la biblioteca cuenta con los sistemas necesarios.

HU-08 — Consultar préstamos

Como usuario identificado de la biblioteca,
quiero consultar mis préstamos y fechas de devolución,
para conocer el estado de los recursos que tengo registrados.

Condición:
Esta historia solo se implementará si existe un sistema de cuentas de usuarios que pueda integrarse con CLENA+.

---

HU-09 — Consultar reservas

Como usuario identificado de la biblioteca,
quiero consultar mis reservas,
para conocer el estado de los recursos que he solicitado.

Condición:
Esta historia depende de que la biblioteca confirme que dispone de un sistema de reservas integrado.

---

5. Priorización inicial

Alta prioridad

- HU-01 — Buscar un recurso.
- HU-02 — Filtrar una búsqueda.
- HU-03 — Revisar resultados.
- HU-04 — Consultar los detalles de un recurso.
- HU-05 — Explorar recursos por tema.
- HU-06 — Obtener ayuda.

Media prioridad

- HU-07 — Acceder a las funciones del personal.

Baja / futura

- HU-08 — Consultar préstamos.
- HU-09 — Consultar reservas.

---

6. Relación entre historias y pantallas

Historia| Pantalla principal
HU-01| Inicio / Búsqueda
HU-02| Búsqueda avanzada
HU-03| Resultados
HU-04| Detalle del recurso
HU-05| Explorar por temas
HU-06| Ayuda y contacto
HU-07| Acceso del personal
HU-08| Cuenta personal
HU-09| Cuenta personal

7. Alcance del primer prototipo

El primer prototipo debe concentrarse en las historias relacionadas directamente con la consulta bibliotecaria:

1. Buscar recursos.
2. Filtrar búsquedas.
3. Revisar resultados.
4. Consultar detalles.
5. Explorar por temas.
6. Obtener ayuda.

Las funciones relacionadas con cuentas, préstamos, reservas y administración deben permanecer como funcionalidades futuras hasta que sean confirmadas por la biblioteca.
