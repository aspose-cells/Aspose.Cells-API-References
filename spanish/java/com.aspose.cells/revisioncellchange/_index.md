---
title: "RevisionCellChange"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa la revisión que cambia celdas."
type: docs
url: /es/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

Representa la revisión que cambia celdas.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | Obtiene el nombre de la celda. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtiene el índice de columna de la celda. |
| [getId()](#getId--) | Obtiene el número de esta revisión. |
| [getNewFormula()](#getNewFormula--) | Obtiene la fórmula anterior. |
| [getNewStyle()](#getNewStyle--) | Obtiene el nuevo estilo de la celda. |
| [getNewValue()](#getNewValue--) | Obtiene el nuevo valor de la celda. |
| [getOldFormula()](#getOldFormula--) | Obtiene la fórmula anterior. |
| [getOldStyle()](#getOldStyle--) | Obtiene el estilo antiguo de la celda. |
| [getOldValue()](#getOldValue--) | Obtiene el valor antiguo de la celda. |
| [getRow()](#getRow--) | Obtiene el índice de fila de la celda. |
| [getType()](#getType--) | Representa el tipo de revisión. |
| [getWorksheet()](#getWorksheet--) | Obtiene la hoja de cálculo. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | Indica si esta celda está formateada como nueva. |
| [isOldFormatted()](#isOldFormatted--) | Indica si esta celda está formateada como antigua. |
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
### getCellName() {#getCellName--}
```
public String getCellName()
```


Obtiene el nombre de la celda.

**Returns:**
java.lang.String
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


Obtiene el índice de columna de la celda.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Obtiene el número de esta revisión.

**Remarks**

Cero significa que esta revisión no contiene id.

**Returns:**
int
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


Obtiene la fórmula anterior.

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


Obtiene el nuevo estilo de la celda.

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


Obtiene el nuevo valor de la celda.

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


Obtiene la fórmula anterior.

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


Obtiene el estilo antiguo de la celda.

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


Obtiene el valor antiguo de la celda.

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


Obtiene el índice de fila de la celda.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Representa el tipo de revisión.

Ver [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Obtiene la hoja de cálculo.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


Indica si esta celda está formateada como nueva.

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


Indica si esta celda está formateada como antigua.

**Returns:**
boolean
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

