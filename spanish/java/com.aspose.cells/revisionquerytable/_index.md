---
title: "RevisionQueryTable"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa una revisión de un cambio de campo de tabla de consulta."
type: docs
url: /es/java/com.aspose.cells/revisionquerytable/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionQueryTable extends Revision
```

Representa una revisión de un cambio de campo de tabla de consulta.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellArea()](#getCellArea--) | Obtiene la ubicación de la tabla de consulta afectada. |
| [getClass()](#getClass--) |  |
| [getFieldId()](#getFieldId--) | Obtiene el ID del campo de tabla de consulta específico que fue eliminado. |
| [getId()](#getId--) | Obtiene el número de esta revisión. |
| [getType()](#getType--) | Representa el tipo de la revisión. |
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
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Obtiene la ubicación de la tabla de consulta afectada.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldId() {#getFieldId--}
```
public int getFieldId()
```


Obtiene el ID del campo de tabla de consulta específico que fue eliminado.

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
### getType() {#getType--}
```
public int getType()
```


Representa el tipo de la revisión.

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

