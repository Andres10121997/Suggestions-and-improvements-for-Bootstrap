# Sugerencias y mejoras para Bootstrap
## Objetivo
### Componentes
1. **<ins>Mejorar componentes</ins>:** Hay algunos componentes en `Bootstrap` que, si bien funcionan, no están utilizando componentes 'nativos' de `HTML`, sino una combinación de `<div>` y código `JavaScript`.
    * Lo que busco con este punto es que no se pase por alto todo lo que busca `HTML5`, que es que el `markup` sea claro.
3. Agregar nuevos componentes.

## Componentes
### Mejoras de componentes
#### `Accordion`
¿Qué propongo para mejorar el `Accordion`?
1. **<ins>Uso de la etiqueta [`<details>`](https://developer.mozilla.org/en/docs/Web/HTML/Reference/Elements/details)</ins>:** Propongo modificar parte del `Accordion` para que se integre la etiqueta nativa `<details>` por las siguientes razones:
    * **<ins>Simplicidad</ins>:** Al ser una etiqueta nativa, el código `HTML` se vuelve más limpio y simple.
    * **<ins>Menos dependencias</ins>:** Eliminar o simplificar el código `JavaScript` podría reducir el peso y mejorar el rendimiento de la página.

#### `Dropdown`
¿Qué propongo para mejorar los botones, links o similares que son `Dropdown`?
1.	**<ins>Uso de la etiqueta [`<details>`](https://developer.mozilla.org/en/docs/Web/HTML/Reference/Elements/details)</ins>:** Propongo modificar los botones, links y similares que son `Dropdown` por la etiqueta nativa `<details>` por las siguientes razones:
    * **<ins>Simplicidad</ins>:** Al ser una etiqueta nativa, el código `HTML` se vuelve más limpio y simple.
    * **<ins>Menos dependencias</ins>:** Eliminar o simplificar el código `JavaScript` podría reducir el peso y mejorar el rendimiento de la página.

#### `Modal`
¿Qué es lo que propongo para mejorar el componente `Modal`?
1.	**<ins>Uso de la etiqueta [`<dialog>`](https://developer.mozilla.org/en-US/docs/Web/HTML/Reference/Elements/dialog)</ins>:** Propongo mejorar los `Modal`, que actualmente se construyen con `<div>` y se manipula con `JavaScript`, con la etiqueta nativa de `<dialog>` en `HTML`. Esto tiene varias ventajas:
    * **<ins>Simplicidad</ins>:** Al ser una etiqueta nativa de `HTML`, el código de este lenguaje de marcado se vuelve más limpio y simple.
    * **<ins>Menos dependencias</ins>:** Eliminar o simplificar el código correspondiente de `JavaScript`, esto reduciría el peso y mejorar el rendimiento de la página.
    * **<ins>Control del estado</ins>:** La etiqueta tiene un atributo open que facilita el control del estado del `Modal`, sin necesidad de escribir `scripts` adicionales.
2. Ventajas para el equipo de desarrollo
    * El uso de la etiqueta `<dialog>` permite reducir la cantidad de código y la dependencia de bibliotecas externas, lo que puede simplificar el trabajo del equipo de desarrollo y mantener el código más limpio y fácil de mantener.

#### `Navbar`
Tener un mayor nivel de personalización:
1.	Tener la capacidad de poner la totalidad, o de manera parcial, los `navlinks` en la parte izquierda, central o derecha del `Navbar` y, de igual manera, el formulario.
2.	En la actualidad el `Navbar` se puede colorear de negro, azul y blanco, hay que tener más opciones.

### Nuevos componentes
#### `Sidebar`
Sé que el `Sidebar` se parece bastante al componente `Offcanvas`, pero creo que sería bastante bueno tener una barra horizontal que complemente al componente `Navbar`.
##### Ventajas
1.	**<ins>Mejorar la visibilidad del contenido</ins>:** “Los contenidos nuevos en tu web no siempre reciben buen tráfico desde el inicio, pero ponerlos en el `Sidebar` ayuda a llevar a más usuarios hacia ellos”.
2.	**<ins>Facilita la navegación</ins>:** “La barra lateral es un buen lugar para colocar una lista de categorías y las etiquetas por las que se relacionan los contenidos. De esta forma, los usuarios pueden navegar por la web con pocos clics y dar con la mayoría de los posts”.
3.	**<ins>Aporta estética al sitio</ins>:** “Los párrafos con líneas muy largas tienden a cansar a los usuarios, ya que estos se están acostumbrando a las vistas móviles. Un `Sidebar` simple sirve para acortar la longitud de los párrafos y hacerlos más compactos”.

## `TypeScript`
Sugiero reemplazar los `script` de `JavaScript` por `TypeScript` ¿Por qué? Para detectar errores antes de la ejecución, facilitar el mantenimiento del proyecto y obtener un autocompletado inteligente en el editor.

## Bibliografía
1. [Andres10121997 | GitHub](https://github.com/orgs/twbs/discussions/33851).
2. [Bootstrap | Modal](https://getbootstrap.com/docs/5.3/components/modal/).
3. [Bootstrap | Sidebars](https://getbootstrap.com/docs/5.3/examples/sidebars/).
4. [Caio](https://dev.to/doccaio/modal-vs-dialog-2bb2).
5. [Casasola, M.](https://seranking.com/es/blog/sidebar-barra-lateral/).
6. [Smith, T.](https://dev.to/iam_timsmith/dialogs-vs-modals-is-there-a-difference-210k).
7. [W3Schools](https://www.w3schools.com/tags/tag_dialog.asp).
8. [W3Schools](https://www.w3schools.com/tags/tag_details.asp).
