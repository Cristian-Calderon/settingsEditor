# ⌨️ Vim Shortcuts — Referencia Rápida

Referencia completa de todos los keybindings configurados en `settings.json` para vscodevim.

> **Tecla líder:** `Space`

---

## 🟡 Insert Mode

| Atajo       | Acción                                                      |
| ----------- | ----------------------------------------------------------- |
| `jk` o `kj` | Salir de insert → normal mode                               |
| `Ctrl+j`    | Bajar por sugerencias de autocomplete                       |
| `Ctrl+k`    | Subir por sugerencias de autocomplete                       |
| `Ctrl+l`    | Mover cursor un carácter a la derecha (sin salir de insert) |

---

## 🔵 Normal Mode

### Archivo y editor

| Atajo       | Acción                         |
| ----------- | ------------------------------ |
| `Space + w` | Guardar archivo                |
| `Space + q` | Cerrar editor activo           |
| `Space + u` | Reabrir último editor cerrado  |
| `Space + n` | Ir al siguiente editor abierto |
| `Space + p` | Ir al editor anterior          |
| `Space + e` | Mostrar / ocultar sidebar      |

### Navegación entre splits

| Atajo       | Acción                  |
| ----------- | ----------------------- |
| `Space + h` | Foco al split izquierdo |
| `Space + l` | Foco al split derecho   |
| `Space + j` | Foco al split de abajo  |
| `Space + k` | Foco al split de arriba |

### Código

| Atajo           | Acción                                                          |
| --------------- | --------------------------------------------------------------- |
| `Space + /`     | Comentar / descomentar línea                                    |
| `Space + d`     | Ir a implementación (go to implementation)                      |
| `Space + Enter` | Partir la línea donde está el cursor                            |
| `D`             | Duplicar línea hacia abajo ⚠️ sobreescribe el `D` nativo de Vim |

### Movimiento por el archivo

| Atajo    | Acción                               |
| -------- | ------------------------------------ |
| `gg`     | Ir al inicio del archivo             |
| `G`      | Ir al final del archivo              |
| `{n}G`   | Ir a la línea número `n` (ej: `42G`) |
| `Ctrl+d` | Bajar media página                   |
| `Ctrl+u` | Subir media página                   |
| `0`      | Inicio de la línea                   |
| `$`      | Final de la línea                    |
| `w`      | Avanzar palabra a palabra            |
| `b`      | Retroceder palabra a palabra         |

---

## 🟣 Visual Mode

| Atajo       | Acción                            |
| ----------- | --------------------------------- |
| `Space + /` | Comentar / descomentar selección  |
| `V`         | Selección por líneas completas    |
| `v`         | Selección por caracteres          |
| `Ctrl+v`    | Selección en bloque (column mode) |

### Seleccionar todo el archivo

```
gg → V → G → y
```

O de golpe desde normal mode: `gg yG`

---

## 🔴 Surround (`vim.enableSurround: true`)

Estando en normal mode con el cursor sobre una palabra:

| Atajo   | Acción                                      |
| ------- | ------------------------------------------- |
| `ysiw"` | Rodear palabra con `"comillas dobles"`      |
| `ysiw'` | Rodear palabra con `'comillas simples'`     |
| `ysiw(` | Rodear palabra con `(paréntesis)`           |
| `ysiw{` | Rodear palabra con `{llaves}`               |
| `ysiw[` | Rodear palabra con `[corchetes]`            |
| `ysit`  | Rodear con etiqueta HTML `<tag>`            |
| `cs"'`  | Cambiar `"comillas dobles"` por `'simples'` |
| `cs({`  | Cambiar `(paréntesis)` por `{llaves}`       |
| `ds"`   | Eliminar las `"comillas"` que rodean        |
| `ds(`   | Eliminar los `(paréntesis)` que rodean      |

---

## ⚡ EasyMotion (`vim.easymotion: true`)

| Atajo           | Acción                                         |
| --------------- | ---------------------------------------------- |
| `Space Space w` | Saltar hacia adelante por palabras             |
| `Space Space b` | Saltar hacia atrás por palabras                |
| `Space Space f` | Saltar a un carácter específico hacia adelante |
| `Space Space F` | Saltar a un carácter específico hacia atrás    |

> Al activarlo aparecen letras sobre cada destino posible. Pulsa la letra para saltar directamente.

---

## 📝 Comandos Vim nativos útiles (sin configurar, funcionan por defecto)

| Atajo             | Acción                                                        |
| ----------------- | ------------------------------------------------------------- |
| `dd`              | Borrar línea completa                                         |
| `yy`              | Copiar línea completa                                         |
| `p`               | Pegar después del cursor                                      |
| `P`               | Pegar antes del cursor                                        |
| `u`               | Deshacer                                                      |
| `Ctrl+r`          | Rehacer                                                       |
| `ciw`             | Cambiar (borrar y entrar en insert) la palabra bajo el cursor |
| `diw`             | Borrar la palabra bajo el cursor                              |
| `yi"`             | Copiar el contenido dentro de `"comillas"`                    |
| `di"`             | Borrar el contenido dentro de `"comillas"`                    |
| `%`               | Saltar al par de la llave/paréntesis/corchete                 |
| `*`               | Buscar la palabra bajo el cursor hacia adelante               |
| `#`               | Buscar la palabra bajo el cursor hacia atrás                  |
| `/texto`          | Buscar `texto` en el archivo                                  |
| `n`               | Siguiente resultado de búsqueda                               |
| `N`               | Resultado anterior de búsqueda                                |
| `:.`              | Repetir el último comando                                     |
| `>>`              | Indentar línea                                                |
| `<<`              | Des-indentar línea                                            |
| `~`               | Cambiar mayúscula/minúscula del carácter bajo el cursor       |
| `gU` + movimiento | Convertir a mayúsculas (ej: `gUiw` → palabra en mayúsculas)   |
| `gu` + movimiento | Convertir a minúsculas                                        |
