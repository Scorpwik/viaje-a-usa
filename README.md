# Guía W&T USA 2026

Página personal de Joshua Alexander Lozada para el programa **Work & Travel** con visa **J-1** del verano 2026. Reúne el itinerario de vuelo, las cifras del empleo y del housing, el proceso de llegada, las reglas del programa y una lista de pendientes que se guarda en el navegador.

**Página en vivo:** [https://scorpwik.github.io/viaje-a-usa/](https://scorpwik.github.io/viaje-a-usa/)

**Repositorio:** [github.com/Scorpwik/viaje-a-usa](https://github.com/Scorpwik/viaje-a-usa)

## De qué se trata

El contenido de `index.html` corresponde a este viaje:

- Programa J-1 Work & Travel, con oferta firmada a través de InterExchange.
- Puesto: Housekeeping Room Attendant en Kalahari Resorts Texas, Round Rock, TX.
- Fechas del programa: 1 de junio al 31 de agosto de 2026.
- Ida: miércoles 27 de mayo de 2026, Quito (UIO) → Atlanta (ATL) → Austin (AUS), vuelos DL0632 y DL1397.
- Regreso a Quito: domingo 30 de agosto.

El pie de la página pide verificar siempre los datos con InterExchange y Kalahari Resorts antes de tomar una decisión. Ahí mismo consta que la guía se generó con IA.

## Secciones

En pantallas anchas, una barra lateral enlaza estas secciones. En pantallas de hasta 900 px, el mismo menú se abre con el botón del encabezado.

| Sección | Qué muestra |
| --- | --- |
| Pendientes | Lista de tareas del viaje. Se puede añadir, marcar, ver el detalle, borrar y reordenar. |
| Vuelo | Itinerario del 27 de mayo de 2026, la escala en Atlanta y el regreso del 30 de agosto. |
| Finanzas | Salario, horas, deducciones estimadas y el efectivo del check-in. |
| Llegada | Pasos al aterrizar en Austin y tareas para hacer antes de volar. |
| Segundo empleo | Lo que la visa J-1 permite y lo que prohíbe para un segundo trabajo. |
| Banco | Opciones de cuenta en Round Rock / Austin y documentos para abrirla. |
| Reglas | Normas del housing y del empleo: asistencia y uniforme. |
| Maleta | Qué llevar desde Ecuador y qué comprar en Texas. |
| Contactos | Housing, Kalahari, InterExchange y taxis de Round Rock. |
| Advertencias | Plazos, avisos y consecuencias que la guía marca como críticos. |

Al imprimir, la barra de navegación se oculta y el contenido ocupa todo el ancho.

## Lista de pendientes

La lista se guarda en el navegador, con `localStorage` y la clave `wt_todos_v2`.

- Si ese navegador todavía no tiene datos guardados, aparecen los pendientes iniciales escritos en la página.
- Al marcar una tarea, pasa al final de la lista.
- Se puede arrastrar un ítem para cambiar el orden.
- Cada ítem se abre para leer el detalle.
- Con `?view=true` la lista queda solo de lectura: se oculta la caja para añadir pendientes, se desactivan las casillas, se quita el botón de borrar y se desactiva el arrastre. En la página publicada: [https://scorpwik.github.io/viaje-a-usa/?view=true](https://scorpwik.github.io/viaje-a-usa/?view=true).

## Tecnologías

Todo el sitio está en un solo archivo, `index.html`. GitHub Pages lo publica desde la rama `main`, en la raíz del repositorio.

- HTML
- CSS en el mismo archivo: variables, Grid, media queries para pantallas angostas y estilos de impresión
- Fuentes [DM Sans](https://fonts.google.com/specimen/DM+Sans) y [DM Mono](https://fonts.google.com/specimen/DM+Mono), cargadas desde Google Fonts
- JavaScript en el mismo archivo, sin frameworks
- `localStorage` para la lista de pendientes

## Verla en la computadora

```bash
git clone https://github.com/Scorpwik/viaje-a-usa.git
cd viaje-a-usa
```

Abre `index.html` en el navegador. Con eso la página ya carga: es un archivo estático, sin instalación ni compilación.

Para abrir el modo solo lectura con una dirección local, sirve la carpeta y entra a `http://localhost:8000/?view=true`. Con Python:

```bash
python3 -m http.server 8000
```

## Autor

Joshua Alexander Lozada Zurita · GitHub: [Scorpwik](https://github.com/Scorpwik)
