---
title: "RevisionCustomView"
second_title: "Referencia de API de Aspose.Cells para Java"
description: "Representa un registro de revisión de la adición o eliminación de una vista personalizada al libro de trabajo."
type: docs
url: /es/java/com.aspose.cells/revisioncustomview/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCustomView extends Revision
```

Representa un registro de revisión de la adición o eliminación de una vista personalizada al libro de trabajo.
## Métodos

| Método | Descripción |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Obtiene el tipo de acción. |
| [getClass()](#getClass--) |  |
| [getGuid()](#getGuid--) | Obtiene el identificador único global de la vista personalizada. |
| [getId()](#getId--) | Obtiene el número de esta revisión. |
| [getType()](#getType--) | Obtiene el tipo de revisión. |
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
### getActionType() {#getActionType--}
```
public int getActionType()
```


Obtiene el tipo de acción.

Ver [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getGuid() {#getGuid--}
```
public UUID getGuid()
```


Obtiene el identificador único global de la vista personalizada.

**Returns:**
java.util.UUID
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

