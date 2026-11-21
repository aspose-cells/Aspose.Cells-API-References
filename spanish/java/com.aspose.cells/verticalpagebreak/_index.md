---
title: "VerticalPageBreak"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Encapsula el objeto que representa un salto de página vertical."
type: docs
url: /es/java/com.aspose.cells/verticalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class VerticalPageBreak
```

Encapsula el objeto que representa un salto de página vertical.

**Example**

```
         Workbook excel = new Workbook();
         //Add a pagebreak at G5
         excel.getWorksheets().get(0).getHorizontalPageBreaks().add("G5");
         excel.getWorksheets().get(0).getVerticalPageBreaks().add("G5");
```
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtiene el índice de columna del salto de página vertical. |
| [getEndRow()](#getEndRow--) | Obtiene el índice de fila final del salto de página vertical. |
| [getStartRow()](#getStartRow--) | Obtiene el índice de fila inicial del salto de página vertical. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getColumn() {#getColumn--}
```
public int getColumn()
```


Obtiene el índice de columna del salto de página vertical.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Obtiene el índice de fila final del salto de página vertical.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Obtiene el índice de fila inicial del salto de página vertical.

**Returns:**
int
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

