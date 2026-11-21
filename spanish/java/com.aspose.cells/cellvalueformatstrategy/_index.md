---
title: "CellValueFormatStrategy"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Especifica cómo aplicar estilo al valor de la celda."
type: docs
url: /es/java/com.aspose.cells/cellvalueformatstrategy/
---

**Inheritance:**
java.lang.Object
```
public final class CellValueFormatStrategy
```

Especifica cómo aplicar estilo al valor de la celda.
## Campos

| Campo | Descripción |
| --- | --- |
| [CELL_STYLE](#CELL-STYLE) | Solo formateado con el estilo original de la celda. |
| [DISPLAY_STRING](#DISPLAY-STRING) | Obtiene la cadena mostrada en MS Excel. |
| [DISPLAY_STYLE](#DISPLAY-STYLE) | Formateado con el estilo mostrado de la celda. |
| [NONE](#NONE) | No formateado. |
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CELL_STYLE {#CELL-STYLE}
```
public static final int CELL_STYLE
```


Solo formateado con el estilo original de la celda.

### DISPLAY_STRING {#DISPLAY-STRING}
```
public static final int DISPLAY_STRING
```


Obtiene la cadena mostrada en MS Excel. La principal diferencia con [DISPLAY\_STYLE](../../com.aspose.cells/cellvalueformatstrategy\#DISPLAY-STYLE) es que esta opción también considera el efecto del ancho de columna. Si el ancho de columna es demasiado pequeño para mostrar la cadena formateada completamente, "\#" puede mostrarse, tal como lo hace MS Excel.

### DISPLAY_STYLE {#DISPLAY-STYLE}
```
public static final int DISPLAY_STYLE
```


Formateado con el estilo mostrado de la celda.

### NONE {#NONE}
```
public static final int NONE
```


No formateado.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

