# Historias de usuario

**Proyecto 2 · Catálogo Bibliográfico Accesible**
CLENA - Biblioteca Piloto del Caribe

Estas historias describen lo que debe permitir la aplicación que construye el equipo de Backend. Cada una está registrada como Issue en su repositorio con la etiqueta `historia-usuario`. Los puntos los estima el equipo de Backend y nosotros los registramos.

## Resumen

| HU | Historia | Prioridad | Puntos | Autor | Issue |
| --- | --- | --- | --- | --- | --- |
| HU-01 | Buscar con un solo campo desde el inicio | Debe tener | - | - | - |
| HU-02 | Buscar con filtros avanzados | Debe tener | - | - | - |
| HU-03 | Ver los resultados de forma clara | Debe tener | - | - | - |
| HU-04 | Ver el detalle y la ubicación de un recurso | Debe tener | - | - | - |
| HU-05 | Explorar la biblioteca por temas | Debe tener | - | - | - |
| HU-06 | Pedir ayuda a un bibliotecario | Debe tener | - | - | - |
| HU-07 | Encontrar un libro con una parte del título | Debe tener | - | - | - |
| HU-08 | Leer con letra grande y buen contraste | Debe tener | - | - | - |
| HU-09 | Buscar por tipo de material | Debe tener | - | - | - |
| HU-10 | Usar el catálogo desde el celular | Debería tener | - | - | - |
| HU-11 | Ver temas frecuentes sugeridos | Debería tener | - | - | - |
| HU-12 | Reconocer los libros por su portada | Podría tener | - | - | - |

---

## Consulta pública

### HU-01 · Buscar con un solo campo desde el inicio

**Como** visitante poco cómodo con la tecnología, **quiero** buscar un libro escribiendo solo una palabra en un único campo **para** encontrarlo sin tener que entender todos los filtros.

**Criterios de aceptación:**
- **Dado que** abro la pantalla de inicio, **cuando** cargue, **entonces** veo un solo campo de búsqueda grande y un botón "Buscar" visible.
- **Dado que** escribo "caribe" en el campo, **cuando** presiono Buscar, **entonces** aparece una lista de materiales relacionados.
- **Dado que** presiono Buscar con el campo vacío, **cuando** ocurra, **entonces** el sistema me avisa que escriba algo.

**Prioridad:** Debe tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-02 · Buscar con filtros avanzados

**Como** usuario que ya sabe qué busca, **quiero** combinar filtros por autor, título, tipo de material, año, idioma y área temática **para** encontrar un recurso específico entre muchos.

**Criterios de aceptación:**
- **Dado que** estoy en la búsqueda avanzada, **cuando** la abro, **entonces** veo cada filtro en un campo con su etiqueta clara.
- **Dado que** escribo un autor y elijo un idioma, **cuando** presiono Buscar, **entonces** solo veo resultados que cumplen ambos filtros.
- **Dado que** apliqué varios filtros, **cuando** presiono Limpiar, **entonces** todos los campos quedan vacíos.

**Prioridad:** Debe tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-03 · Ver los resultados de forma clara

**Como** usuario de la biblioteca, **quiero** ver los resultados ordenados con título, autor y tipo de material **para** identificar rápido cuál es el que necesito.

**Criterios de aceptación:**
- **Dado que** hice una búsqueda, **cuando** aparecen los resultados, **entonces** cada uno muestra título, autor y tipo de material.
- **Dado que** no hay coincidencias, **cuando** termina la búsqueda, **entonces** veo un mensaje que me sugiere cambiar las palabras o pedir ayuda.
- **Dado que** hay muchos resultados, **cuando** los reviso, **entonces** están divididos en páginas.

**Prioridad:** Debe tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-04 · Ver el detalle y la ubicación de un recurso

**Como** usuario de la biblioteca, **quiero** abrir un recurso y ver su información y dónde está en la biblioteca **para** ir directo a buscarlo sin preguntar.

**Criterios de aceptación:**
- **Dado que** estoy en los resultados, **cuando** abro un recurso, **entonces** veo su título, autor, año, idioma y tipo de material.
- **Dado que** el recurso está disponible, **cuando** veo su detalle, **entonces** aparecen la sala, la sección y el estante donde está.
- **Dado que** estoy en el detalle, **cuando** presiono "Volver", **entonces** regreso a mis resultados sin perder la búsqueda.

**Prioridad:** Debería tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-05 · Explorar la biblioteca por temas

**Como** usuario que no conoce el título ni el autor, **quiero** explorar por categorías y subcategorías **para** descubrir materiales relacionados con un área.

**Criterios de aceptación:**
- **Dado que** entro a "Explorar por temas", **cuando** se carga, **entonces** veo las categorías principales (por ejemplo, Programación, Redes o Inteligencia artificial).
- **Dado que** elijo una categoría, **cuando** la abro, **entonces** veo sus subcategorías y los materiales de ese tema.
- **Dado que** estoy dentro de una categoría, **cuando** quiero volver, **entonces** hay un botón visible para regresar.

**Prioridad:** Debe tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-06 · Pedir ayuda a un bibliotecario

**Como** usuario que no encuentra lo que busca, **quiero** contactar fácilmente al personal de la biblioteca **para** resolver mi duda sin sentir pena ni perder tiempo.

**Criterios de aceptación:**
- **Dado que** estoy en cualquier pantalla, **cuando** busco ayuda, **entonces** veo un botón visible de "Ayuda" o "Hablar con un bibliotecario".
- **Dado que** abro la sección de ayuda, **cuando** se carga, **entonces** veo instrucciones de uso, preguntas frecuentes, información de contacto y horarios de atención.
- **Dado que** envío un mensaje, **cuando** lo confirmo, **entonces** el sistema me muestra que fue enviado.

**Prioridad:** Podría tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-07 · Encontrar un libro con una parte del título

**Como** usuario de la biblioteca, **quiero** buscar escribiendo solo una parte del título **para** encontrarlo aunque no recuerde el nombre exacto.

**Criterios de aceptación:**
- **Dado que** escribo "cien años sole", **cuando** presiono Buscar, **entonces** aparece "Cien años de soledad" entre los primeros resultados.
- **Dado que** escribo una palabra sin tilde o con una letra mal, **cuando** busco, **entonces** el sistema igual muestra resultados parecidos.

**Prioridad:** Debe tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-08 · Leer con letra grande y buen contraste

**Como** adulto mayor, **quiero** que el texto sea grande y se vea con buen contraste **para** leer sin esforzarme ni pedir ayuda.

**Criterios de aceptación:**
- **Dado que** abro cualquier pantalla, **cuando** se carga, **entonces** el texto tiene un tamaño mínimo de 16 px.
- **Dado que** reviso botones y campos, **cuando** los veo, **entonces** son grandes y tienen colores con buen contraste.
- **Dado que** hay un formulario, **cuando** lo veo, **entonces** cada campo tiene su etiqueta visible.

**Prioridad:** Debe tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-09 · Buscar por tipo de material

**Como** usuario que quiere un material concreto, **quiero** filtrar por tipo (libro, periódico, poesía, cómic) **para** ir directo a lo que quiero leer.

**Criterios de aceptación:**
- **Dado que** estoy en la búsqueda, **cuando** abro el filtro de tipo de material, **entonces** veo las opciones disponibles.
- **Dado que** elijo "Periódico", **cuando** busco, **entonces** solo veo resultados de ese tipo.

**Prioridad:** Debe tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-10 · Usar el catálogo desde el celular

**Como** usuario de la biblioteca, **quiero** abrir el catálogo desde mi celular **para** buscar sin esperar un computador de la biblioteca.

**Criterios de aceptación:**
- **Dado que** abro el sitio desde un celular, **cuando** se carga, **entonces** todo se ve completo y sin tener que hacer zoom.
- **Dado que** escaneo un código QR en la biblioteca, **cuando** lo abro, **entonces** llego directo a la pantalla de búsqueda.

**Prioridad:** Podría tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-11 · Ver temas frecuentes sugeridos

**Como** usuario sin una idea clara de qué leer, **quiero** ver temas populares sugeridos **para** tener por dónde empezar.

**Criterios de aceptación:**
- **Dado que** estoy en el inicio, **cuando** lo veo, **entonces** aparece una lista de temas frecuentes.
- **Dado que** toco un tema sugerido, **cuando** lo elijo, **entonces** veo los materiales de ese tema.

**Prioridad:** Debería tener · **Puntos:** - · **Autor:** - · **Issue:** -

### HU-12 · Reconocer los libros por su portada

**Como** usuario joven que se guía por imágenes, **quiero** ver la portada de cada resultado **para** reconocer lo que busco sin leer tanto.

**Criterios de aceptación:**
- **Dado que** aparecen resultados, **cuando** los reviso, **entonces** cada uno muestra su portada si está disponible.
- **Dado que** un recurso no tiene portada, **cuando** aparece en la lista, **entonces** se muestra una imagen genérica por defecto.

**Prioridad:** Podría tener · **Puntos:** - · **Autor:** - · **Issue:** -

---

## Fuera del alcance de esta entrega

Estas funciones se consideraron, pero no se construyen ahora porque dependen de confirmar con la biblioteca que existen y que se pueden integrar:

- **Acceso del personal:** Que un trabajador autorizado se autentique para usar funciones internas.
- **Consultar préstamos y reservas:** Que un usuario identificado vea el estado de sus préstamos, fechas de devolución y reservas.
