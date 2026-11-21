---
title: "RevisionCellMove"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un registro de revisión en una celda que se movió."
type: docs
url: /es/java/com.aspose.cells/revisioncellmove/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellMove extends Revision
```

Representa un registro de revisión de una(s) celda(s) que se movió.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDestinationArea()](#getDestinationArea--) | Obtiene el área de destino. |
| [getId()](#getId--) | Obtiene el número de esta revisión. |
| [getSourceArea()](#getSourceArea--) | Obtiene el área de origen. |
| [getSourceWorksheet()](#getSourceWorksheet--) | Obtiene la hoja de cálculo de origen. |
| [getType()](#getType--) | Representa el tipo de revisión. |
| [getWorksheet()](#getWorksheet--) | Obtiene la hoja de cálculo. |
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
### getDestinationArea() {#getDestinationArea--}
```
public CellArea getDestinationArea()
```


Obtiene el área de destino.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getId() {#getId--}
```
public int getId()
```


Obtiene el número de esta revisión.

**Remarks**

Cero significa que esta revisión no contiene id.

**Returns:**
int
### getSourceArea() {#getSourceArea--}
```
public CellArea getSourceArea()
```


Obtiene el área de origen.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getSourceWorksheet() {#getSourceWorksheet--}
```
public Worksheet getSourceWorksheet()
```


Obtiene la hoja de cálculo de origen.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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

