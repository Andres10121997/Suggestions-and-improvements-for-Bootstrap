# Sugerencias y mejoras para Bootstrap
## Objetivo
### Componentes
1. **<ins>Mejorar componentes</ins>:** Hay algunos componentes en `Bootstrap` que, si bien funcionan, no están utilizando componentes 'nativos' de `HTML`, sino una combinación de `<div>` y código `JavaScript`.
2. Agregar nuevos componentes.

## Componentes
### `Modal`
¿Qué es lo que propongo para mejorar el componente `Modal`?
1.	**<ins>Uso de la etiqueta `<dialog>`</ins>:** Propongo reemplazar los modales, que actualmente se construyen con `<div>` y manipulación de `JavaScript`, con la etiqueta nativa de `<dialog>` en `HTML`. Esto tiene varias ventajas:
  * **<ins>Simplicidad</ins>:** Al ser una etiqueta nativa, el código `HTML` se vuelve más limpio y simple.
  * **<ins>Menos dependencias</ins>:** Eliminar o simplificar el código `JavaScript` podría reducir el peso y mejorar el rendimiento de la página.
  * **<ins>Control del estado</ins>:** La etiqueta tiene un atributo open que facilita el control del estado del modal, sin necesidad de escribir scripts adicionales.
