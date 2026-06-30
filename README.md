# DOSW-2026-POKEDEX-POKEPEDIA MabelBernal
# POKEPEDIA
![Pokepedia Banner](https://github.com/MabelBernalAmaya/DOSW-2026-POKEDEX-MabelBernal/blob/develop/Docs/pokepediaimagem.png)
**"Conoce · Explora · Aprende"**

---
![Pokepedia que es ](https://github.com/MabelBernalAmaya/DOSW-2026-POKEDEX-MabelBernal/blob/develop/Docs/que%20es%20pokepedia.png)
## ¿Qué es Poképedia?

Poképedia es mi versión de una Pokédex real, como proyecto individual para el curso de Desarrollo y Operaciones de Software (DOSW) — Intersemestral 2026.

La idea fue crear algo que se sintiera como una herramienta que usaria un entrenador Pokémon en donde  se pueda buscar cualquier Pokémon, ver toda su información, armar tu equipo y entender qué tan bueno es competitivamente. Todo con una identidad visual propia inspirada en el universo Pokémon pero con un estilo más tecnológico .

---
![que puedo hacer en pokepedia ](https://github.com/MabelBernalAmaya/DOSW-2026-POKEDEX-MabelBernal/blob/develop/Docs/qie%20puedo%20hacer%20en%20pokepedia.png)
##  Especificación de Requerimientos (Fase I)

### Módulos del Sistema (Requisitos Funcionales)
Que me permite hacer Pokepedia?


* **RF-01 (Registro Local):** Formulario para la creación de cuentas de usuario de forma segura con validación de credenciales.
* **RF-02 (Autenticación con Google):** Inicio de sesión rápido mediante la integración con **Google Auth API**, gestionando la sesión a través de tokens JWT.


* **RF-05 (Cuadrícula del Catálogo):** Vista principal en formato *Grid Layout* que despliega las tarjetas de los Pokémon con un diseño responsivo y estilo *glassmorphism* (semitransparente).
* **RF-06 (Ficha de Detalle):** Vista individual para analizar a fondo las estadísticas base, tipos elementales, habilidades y líneas evolutivas de cada espécimen.
* **RF-07 (Buscador en Tiempo Real):** Filtro reactivo que procesa la búsqueda por nombre o identificador numérico (ID) en tiempo real mientras el usuario escribe.
* **RF-08 y RF-11 (Filtros Avanzados):** Panel de control para combinar filtros concurrentes: segmentación por tipo elemental, región de origen, rangos de estadísticas base (1-255) y ordenamiento (A-Z, ID o velocidad máxima).

* **RF-09 (Construcción de Equipos):** Espacio de trabajo interactivo para gestionar y armar alineaciones competitivas con un límite estricto de hasta 6 ranuras (*slots*) por equipo.
* **RF-10 (Persistencia de Equipos):** Operaciones CRUD completas que permiten al usuario guardar múltiples equipos en su cuenta, modificar sus integrantes o eliminarlos de la base de datos.
* **RF-12 (Comparador Versus):** Interfaz para contrastar las estadísticas de dos Pokémon cara a cara, aplicando un resaltado visual sobre el atributo dominante.
* **RF-13 (Lista de Favoritos):** Marcado rápido de Pokémon predilectos para guardarlos e indexarlos directamente en el perfil del usuario.
* **RF-15 (Exportador a Showdown):** Función para generar y exportar la ficha del equipo en bloques de texto plano, 100% compatible con el formato de **Pokémon Showdown**.
* **RF-16 (Asistente de Sinergias):** Lógica del sistema que calcula la cobertura táctica (debilidades y resistencias) mediante una matriz dinámica y permite autocompletar espacios vacíos con un solo clic.



### Atributos del Sistema (Requisitos No Funcionales)

* ** Diseño e Interfaz (UI/UX):** La aplicación implementa un sistema visual oscuro de alto contraste estilo Cyberpunk. Utiliza un fondo negro puro (`#000000`), tipografías sans-serif de alta legibilidad y bordes emisivos neón (tonos púrpura, cian y rosa) para delimitar los estados interactivos.
* ** Percepción de Latencia:** Para optimizar la UX en peticiones asíncronas, la barra de búsqueda incorpora un componente animado (un signo de pregunta `?`) que genera un pulso de color continuo mientras se procesa la respuesta del servidor.
* ** Rendimiento y Carga:** Las búsquedas en el catálogo, el filtrado avanzado y el renderizado de gráficos deben responder en un tiempo máximo de **1.5 segundos** en entorno local, optimizando el manejo de estados en el cliente.
* ** Arquitectura y Mantenibilidad:** El código fuente sigue principios de modularidad (Frontend en React/Next.js y backend de la API en Node.js), asegurando alta cohesión y bajo acoplamiento para facilitar futuras pruebas unitarias y la escalabilidad del proyecto.
## Tablero Jira

Acá está toda la planeación del proyecto: la épica, los features por módulo, las historias de usuario de cada requerimiento y las tareas técnicas necesarias para desarrollarlos.

[Ver tablero en Jira](https://mailmabel.atlassian.net/jira/software/projects/POK/boards/34?atlOrigin=eyJpIjoiNWFjYzk2YWQ4MjlkNGY2ZTkwZTUxOTY0Y2MyYWNkODciLCJwIjoiaiJ9)

---
## Prototipo

El prototipo inicial fue diseñado en Figma y también en Lovable, siguiendo el manual de identidad de Poképedia.



 [Ver en Lovable](https://lovable.dev/projects/f9492b15-532e-4b33-b7dd-a442c0d80e93?magic_link=mc_a4e6599e-52ce-4d1b-b721-df4d378a091b)

---


---

## Documento de requerimientos

El análisis de requerimientos está basado en la plantilla DOSW e incluye los 16 requerimientos funcionales detallados con sus flujos, datos de entrada y salida, reglas de negocio, y los diagramas de casos de uso por cada uno. También están los 8 requerimientos no funcionales del sistema.

 [Ver documento de requerimientos](https://github.com/MabelBernalAmaya/DOSW-2026-POKEDEX-MabelBernal/blob/develop/Docs/Plantilla_Requerimientos_DOSW%20correccion.docx)

---

## Manual de identidad

Poképedia tiene su propia identidad . El manual  nos permite definir el nombre, el logotipo, la paleta de colores, las tipografías, la iconografía, las reglas de uso de marca y la mascota oficial usando la herramienta de Canva. 

| | |
|---|---|
| **Nombre** | Poképedia |
| **Eslogan** | Conoce · Explora · Aprende |
| **Colores** | Amarillo `#FCCA3E` · Morado `#7B2FBE` · Azul `#4ECDC4` · Negro `#0A0A0A` |
| **Tipografías** | Press Start 2P (títulos) · Inter (texto) |
| **Mascota** | Pikachu detective |


 [Ver manual de identidad](https://canva.link/aj3d2ue97w0291m)

![Manual de identidad ](https://github.com/MabelBernalAmaya/DOSW-2026-POKEDEX-MabelBernal/blob/develop/Docs/CONOCE-EXPLORA-APRENDE.png)

---

## Autora

**Mabel Fernanda Bernal Amaya**
DOSW · Intersemestral 2026