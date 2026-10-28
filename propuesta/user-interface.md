# CLENA+ — Guía de interfaz y pantallas

## 1. Propósito

Definir una estructura inicial de las pantallas y los componentes de interfaz de CLENA+, una propuesta de rediseño de la plataforma de consulta bibliotecaria de la Biblioteca Piloto del Caribe, ubicada en el Centro de Lenguas Extranjeras (CLENA).

La interfaz debe facilitar la búsqueda y exploración de recursos bibliográficos, mostrar los resultados de manera comprensible y hacer visibles las opciones de ayuda y contacto. El objetivo principal es mejorar la organización y la facilidad de uso, conservando las funcionalidades de consulta existentes.

> Este documento describe una propuesta de interfaz. Las funciones de autenticación, préstamo, reservas y administración deberán confirmarse con la biblioteca antes de implementarse como funciones reales.

## 2. Tipos de usuario

### 2.1. Visitante o usuario de consulta

Persona que desea buscar libros u otros recursos bibliográficos.

- Puede entrar a la página principal.
- Puede buscar por palabra clave, título, autor y otros filtros disponibles.
- Puede explorar recursos por áreas temáticas.
- Puede consultar los detalles de un resultado.
- Puede acceder a la sección de ayuda y contacto.
- No debe necesitar una contraseña para realizar búsquedas públicas, salvo que el sistema actual de la biblioteca establezca otra condición.

### 2.2. Usuario identificado de la biblioteca (opcional)

Si la biblioteca dispone de servicios personalizados, este usuario podría identificarse mediante el método autorizado por la institución.

- Puede consultar sus datos básicos.
- Puede revisar préstamos, fechas de devolución o reservas únicamente si esos datos están disponibles en los sistemas existentes.
- No se debe mostrar información personal sin una identificación válida.

### 2.3. Trabajador o bibliotecario

Personal autorizado que puede necesitar acceder a herramientas internas.

- Debe entrar por una pantalla de acceso separada de la búsqueda pública.
- Debe identificarse con las credenciales que defina la institución.
- Solo debe ver las funciones que correspondan a sus permisos.
- No debe suponerse que cualquier trabajador puede modificar el catálogo o los registros.

**Importante:** que el usuario público pueda consultar sin contraseña no significa que las funciones internas deban estar abiertas. No usar una contraseña para la consulta pública y autenticar al personal son decisiones distintas.

## 3. Navegación principal

La navegación pública debe ser breve y consistente en todas las pantallas.

- **Inicio**
- **Buscar recursos**
- **Explorar por temas**
- **Ayuda y contacto**
- **Acceso del personal** (enlace discreto, claramente separado de la consulta pública)

En dispositivos móviles, las opciones pueden agruparse en un menú desplegable. Debe mantenerse visible una forma sencilla de volver al inicio.

## 4. Pantallas propuestas

### Pantalla 1. Inicio

**Objetivo:** explicar rápidamente qué permite hacer la plataforma y llevar al usuario a la búsqueda.

**Elementos:**

- Nombre y logotipo de CLENA+ / Biblioteca Piloto del Caribe.
- Menú principal.
- Título claro, por ejemplo: “Encuentra recursos para aprender e investigar”.
- Campo de búsqueda principal.
- Botón **Buscar**.
- Acceso visible a **Búsqueda avanzada**.
- Accesos por tema o categoría.
- Acceso a **Ayuda y contacto**.
- Horarios e información institucional, si están confirmados.
- Pie de página con información de la biblioteca.

**Comportamiento:**

- Al escribir una consulta y pulsar Buscar, abrir la pantalla de resultados con el término introducido.
- Si el campo está vacío, mostrar una indicación útil en lugar de fallar silenciosamente.
- No obligar a iniciar sesión para hacer una búsqueda pública.

### Pantalla 2. Búsqueda general o avanzada

**Objetivo:** permitir búsquedas con criterios específicos sin saturar la pantalla inicial.

**Campos y filtros propuestos:**

- Palabra clave.
- Título.
- Autor.
- Tipo de material.
- Año de publicación.
- Idioma.
- Área temática.

**Acciones:**

- Botón **Buscar**.
- Botón **Limpiar filtros**.
- Opción para volver a la búsqueda simple.

**Comportamiento:**

- Los campos deben tener etiquetas visibles; no depender solo del texto de ejemplo.
- Los filtros opcionales deben estar agrupados y ordenados.
- Si no se completa un filtro, la búsqueda debe poder continuar con los demás criterios.
- Mostrar un resumen de los filtros aplicados en la pantalla de resultados.

### Pantalla 3. Resultados de búsqueda

**Objetivo:** presentar los recursos encontrados y facilitar la comparación entre ellos.

**Elementos:**

- Texto de la búsqueda actual.
- Número de resultados, si el sistema proporciona ese dato.
- Filtros aplicados y opción de quitarlos.
- Ordenamiento, solo con criterios que el catálogo permita.
- Lista de resultados.
- Mensajes para estados de carga, error o ausencia de resultados.
- Acceso para modificar la búsqueda.

**Cada resultado puede mostrar, si esos datos existen:**

- Título.
- Autor o autores.
- Año de publicación.
- Tipo de material.
- Idioma.
- Imagen de portada, si está disponible.
- Breve descripción.
- Acción **Ver detalles**.

**Comportamiento:**

- Los filtros deben poder modificarse sin perder innecesariamente la consulta.
- La paginación o carga adicional debe ser clara.
- Si no hay resultados, sugerir revisar la ortografía, quitar filtros o probar otros términos.
- No inventar disponibilidad, ubicación o cantidad de ejemplares si el catálogo no entrega esos datos.

### Pantalla 4. Detalle de un recurso

**Objetivo:** mostrar la información disponible de un libro u otro material.

**Elementos posibles:**

- Título y portada.
- Autor o autores.
- Año, editorial, idioma y tipo de material.
- Descripción o resumen.
- Temas relacionados.
- Identificador bibliográfico, si existe.
- Información de ejemplares, sede o disponibilidad, únicamente si el sistema la proporciona.
- Botón para volver a los resultados.
- Acceso a ayuda si el usuario necesita orientación.

**Comportamiento:**

- Ocultar o identificar claramente los datos que no estén disponibles.
- Si la biblioteca no ofrece reservas en línea, no mostrar un botón funcional de reservar.
- Si se contempla una reserva futura, documentarla como una función pendiente de validar.

### Pantalla 5. Exploración por temas

**Objetivo:** ayudar a encontrar recursos cuando el usuario no conoce un título o autor específico.

**Categorías iniciales sugeridas:**

- Arquitectura.
- Bases de datos.
- Redes.
- Programación.
- Sistemas operativos.
- Seguridad informática.
- Inteligencia artificial.
- Otras áreas.

Las categorías deben adaptarse a los temas reales del catálogo de la biblioteca.

**Elementos:**

- Título e introducción breve.
- Tarjetas o lista de categorías.
- Nombre de cada categoría y, si se dispone del dato, cantidad de recursos.
- Acción **Explorar recursos**.

**Comportamiento:**

- Al seleccionar una categoría, mostrar los recursos relacionados o abrir resultados con el filtro temático aplicado.
- Incluir una opción para volver a todas las categorías.

### Pantalla 6. Ayuda y contacto

**Objetivo:** permitir que el usuario encuentre asistencia sin tener que recorrer toda la plataforma.

**Elementos:**

- Preguntas frecuentes.
- Información de contacto oficial.
- Horarios de atención confirmados.
- Instrucciones básicas para buscar recursos.
- Formulario de mensaje o solicitud de ayuda, si la institución lo autoriza.
- Chat con un bibliotecario, solo si existe o se implementará ese servicio.

**Si hay un formulario:**

- Asunto.
- Mensaje.
- Correo de contacto, si es necesario.
- Mensajes claros de envío correcto o error.
- Aviso sobre el uso de los datos enviados.

No presentar un chat, formulario o canal como operativo hasta que exista una implementación real.

### Pantalla 7. Acceso del personal

**Objetivo:** permitir que los trabajadores autorizados entren a las funciones internas sin confundirlas con la consulta pública.

**Elementos:**

- Identidad visual de la biblioteca.
- Título **Acceso del personal**.
- Campo de usuario o correo institucional.
- Campo de contraseña.
- Botón **Iniciar sesión**.
- Mensaje de error genérico si las credenciales no son válidas.
- Enlace de recuperación de acceso, únicamente si existe un procedimiento real.
- Enlace para volver a la búsqueda pública.

**Reglas de interfaz y seguridad:**

- No incluir una contraseña universal ni credenciales fijas en el código.
- No permitir entrar al panel interno solo por ocultar o mostrar un botón.
- Las autorizaciones deben verificarse en el servidor.
- No revelar si un usuario específico existe al mostrar errores de acceso.
- Si la institución utiliza otro método de autenticación, adaptar esta pantalla al método oficial.

### Pantalla 8. Panel del personal (opcional y sujeto a validación)

**Objetivo:** ofrecer una entrada organizada a las herramientas internas que la biblioteca autorice.

**Posibles elementos, solo si están dentro del alcance institucional:**

- Resumen de tareas o avisos.
- Accesos a las herramientas autorizadas.
- Información de la sesión.
- Nombre o rol del trabajador, si corresponde.
- Acción **Cerrar sesión**.

No asumir que el personal necesita administrar libros, editar registros, registrar préstamos o gestionar usuarios. Esas operaciones dependen del sistema actual, de los permisos y del alcance aprobado.

### Pantalla 9. Consulta de préstamos o cuenta personal (opcional)

Esta pantalla solo se debe incluir si la biblioteca confirma que existe un sistema de cuentas de usuarios y que puede integrarse con él.

**Posibles elementos:**

- Datos básicos del usuario.
- Préstamos activos.
- Fechas de devolución.
- Historial o reservas, si el sistema lo permite.
- Mensajes sobre vencimientos.

La información debe proceder del sistema institucional. No crear datos ficticios que puedan confundirse con préstamos reales. Si no existe esta integración, omitir la pantalla del prototipo funcional o marcarla como propuesta futura.

## 5. Componentes compartidos

Las pantallas deben reutilizar componentes visuales para mantener la consistencia.

- Encabezado y navegación.
- Pie de página.
- Campo de búsqueda.
- Campos de formulario con etiquetas.
- Botones principales y secundarios.
- Tarjetas de categorías.
- Tarjetas o filas de resultados.
- Filtros activos.
- Indicador de carga.
- Mensaje de error.
- Mensaje de ausencia de resultados.
- Confirmación de acciones, cuando corresponda.
- Enlace para regresar o cancelar.

## 6. Estados que deben diseñarse

No diseñar únicamente la pantalla ideal. Cada función relevante debe contemplar:

- **Inicial:** aún no se ha realizado una búsqueda.
- **Cargando:** se está consultando la información.
- **Con resultados:** se muestran los datos encontrados.
- **Sin resultados:** la consulta se completó, pero no encontró coincidencias.
- **Error:** no fue posible completar la operación.
- **Sin conexión:** cuando pueda detectarse ese estado.
- **Acceso denegado:** el usuario no tiene autorización para una función interna.
- **Sesión finalizada:** cuando exista autenticación.

Los mensajes deben explicar qué ocurrió y, cuando sea posible, cómo continuar.

## 7. Reglas visuales y de experiencia de usuario

- Priorizar claridad, organización, simplicidad, consistencia y accesibilidad.
- Utilizar textos directos y etiquetas comprensibles.
- Mantener una jerarquía visual clara: título, búsqueda, filtros y resultados.
- Evitar colocar todos los filtros y todas las opciones en un único formulario saturado.
- Usar un diseño adaptable a computador, tableta y móvil.
- Mantener contraste suficiente y no depender únicamente del color para comunicar estados.
- Hacer que los controles se puedan identificar y utilizar con teclado.
- Mostrar estados de foco y mensajes de validación.
- Usar tamaños de texto legibles y áreas táctiles cómodas.
- Mantener las mismas convenciones de botones, formularios y navegación en todas las pantallas.
- No incluir elementos decorativos que dificulten encontrar la búsqueda principal.

## 8. Flujos principales

### Flujo A. Buscar un libro

1. El usuario entra a Inicio.
2. Escribe un título, autor o palabra clave.
3. Pulsa **Buscar**.
4. Revisa los resultados.
5. Ajusta los filtros si es necesario.
6. Abre el detalle de un recurso.
7. Regresa a los resultados o consulta Ayuda.

### Flujo B. Buscar por tema

1. El usuario entra a **Explorar por temas**.
2. Selecciona una categoría.
3. Revisa los recursos relacionados.
4. Abre un resultado.
5. Vuelve a la categoría o modifica la búsqueda.

### Flujo C. Un trabajador inicia sesión

1. El trabajador selecciona **Acceso del personal**.
2. Introduce sus credenciales institucionales.
3. El sistema valida la identidad y los permisos.
4. Si la autenticación es correcta, abre las herramientas autorizadas.
5. El trabajador cierra sesión al terminar.

### Flujo D. Solicitar ayuda

1. El usuario abre **Ayuda y contacto**.
2. Consulta las instrucciones o preguntas frecuentes.
3. Si no resuelve su duda, utiliza un canal de contacto disponible.
4. El sistema confirma el envío solo si la solicitud se procesó correctamente.

## 9. Alcance recomendado para el primer prototipo

Para mantener el proyecto enfocado en el rediseño de la consulta bibliotecaria, se recomienda comenzar con:

1. Inicio.
2. Búsqueda general o avanzada.
3. Resultados de búsqueda.
4. Detalle de un recurso.
5. Exploración por temas.
6. Ayuda y contacto.
7. Acceso del personal como pantalla visual, si se necesita demostrar la separación entre consulta pública y herramientas internas.

El panel del personal, las cuentas de usuario, los préstamos, las reservas y la administración del catálogo deben tratarse como módulos opcionales hasta confirmar que la biblioteca los requiere y que existe acceso a los sistemas necesarios.

## 10. Criterios de aceptación del diseño

La propuesta visual se considerará satisfactoria cuando:

- Una persona pueda identificar dónde buscar sin necesitar instrucciones externas.
- La búsqueda simple esté disponible desde Inicio.
- Los filtros avanzados estén organizados y etiquetados.
- Los resultados permitan distinguir los recursos y acceder a sus detalles.
- Se pueda explorar por categorías temáticas.
- La ayuda y el contacto sean fáciles de localizar.
- Existan diseños para carga, error y ausencia de resultados.
- La navegación funcione en pantallas pequeñas.
- El acceso del personal esté separado de la consulta pública.
- Las pantallas no prometan funciones que todavía no estén implementadas o confirmadas.

## 11. Decisiones pendientes antes de desarrollar

Antes de convertir este diseño en un sistema funcional, confirmar con la biblioteca:

- Qué catálogo o API alimenta los resultados.
- Qué campos bibliográficos están realmente disponibles.
- Si se puede mostrar la disponibilidad de ejemplares.
- Si existe autenticación para trabajadores y cuál es el método oficial.
- Si los usuarios tienen cuentas, préstamos o reservas en línea.
- Qué herramientas necesita el personal.
- Qué canales de ayuda y horarios son oficiales.
- Qué datos se pueden consultar y cuáles requieren permisos.
- Si el proyecto será solo un prototipo visual o se conectará al sistema existente.

## 12. Principio general

CLENA+ debe facilitar que el usuario encuentre recursos bibliográficos, comprenda los resultados y sepa qué hacer después. La prioridad es organizar mejor las funciones existentes y reducir la confusión; las funciones nuevas deben incorporarse únicamente cuando sus requisitos y su viabilidad estén confirmados.
