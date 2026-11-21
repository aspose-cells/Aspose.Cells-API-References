---
title: "RevisionCellComment"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un registro de revisión de un cambio en el comentario de una celda."
type: docs
url: /es/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

Representa un registro de revisión de un cambio en el comentario de una celda.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Obtiene el tipo de acción de la revisión. |
| [getCellName()](#getCellName--) | Obtiene el nombre de la celda. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Obtiene el índice de columna del que contiene un comentario. |
| [getId()](#getId--) | Obtiene el número de esta revisión. |
| [getNewLength()](#getNewLength--) | Obtiene la longitud del comentario antes de que se hiciera esta revisión. |
| [getOldLength()](#getOldLength--) | Obtiene la longitud del texto del comentario añadido en esta revisión. |
| [getRow()](#getRow--) | Obtiene el índice de fila del que contiene un comentario. |
| [getType()](#getType--) | Obtiene el tipo de revisión. |
| [getWorksheet()](#getWorksheet--) | Obtiene la hoja de cálculo. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | Indica si es un comentario antiguo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | Obtiene el nombre de la celda. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Obtiene el tipo de acción de la revisión.

Ver [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
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


Obtiene el índice de columna del que contiene un comentario.

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
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


Obtiene la longitud del comentario antes de que se hiciera esta revisión.

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


Obtiene la longitud del texto del comentario añadido en esta revisión.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Obtiene el índice de fila del que contiene un comentario.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Obtiene el tipo de revisión.

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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


Indica si es un comentario antiguo.

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




### setCellName(String value) {#setCellName-java.lang.String-}
```
public void setCellName(String value)
```


Obtiene el nombre de la celda.

**Parameters:**
| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| valor | java.lang.String |  |

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

