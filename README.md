# Resumen de etiquetas Markdown
###### Y.H.H. - Desarrollo de Aplicaciones Web - Entornos de Desarrollo
###
### Sintaxis básica
| Elemento    |  Sintaxis    |
| ----------  | -----------  |
| Cabecera H1      | `#`       |
| ... | ...|
| Cabecera H6   | `######`      | 
| Negrita | `**negrita**` |
| Cursiva | `*cursiva*` |
| Cita | `> cita` |
| Código | `` |
| Línea horizontal | `---` |
| Enlace | `[titulo](https://www.ejemplo.com)` |
| Imágen | `![texto alternativo](ruta o enlace a la imagen)` |
###
##### Lista ordenada
```
1. Primero
2. Segundo
3. Tercero
4. Etcétera
```
###
##### Lista desordenada
```
- Primero
- Segundo
- Tercero
- Etcétera
```
#
### Sintaxis extendida
| Elemento    |  Sintaxis    |
| ----------  | -----------  |
| Emojis     | `:joy:`       |
| Destacar | `algo ==importante== aqui`|
| Tachar | `~~tachado~~` |
| ID de encabezado | `# Encabezado {#id-aqui}` |
| Superdíndice | `X^2^` |
| Subíndice | `H~2~O` |
###
##### Tabla
```
| Cabecera 1 | Cabecera 2 |
| ---------  | ---------- |
| Celda 1.1  | Celda 2.1  |
| Celda 1.2  | Celda 2.2  |
```
###
##### Bloque de código
```
` ` `
```
```
{
  "nombre": "John",
  "apellido": "Doe",
  "edad": 25
}
```
```
` ` `
```
###
##### Nota al pie
```
Frase con una nota al pie. [^1]

[^1]: Nota al pie.
```
###
##### Lista de definiciones
```
término
: definición1
```
###
##### Lista de tareas
```
- [x] Dormirse
- [ ] Despertarse
- [ ] Día arruinado
```