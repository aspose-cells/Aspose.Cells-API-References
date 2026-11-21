---
title: "RevisionInsertDelete"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en revisionspost för en rad-/kolumninfogning-/borttagningsåtgärd."
type: docs
url: /sv/java/com.aspose.cells/revisioninsertdelete/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionInsertDelete extends Revision
```

Representerar en revisionspost för en rad-/kolumninfogning-/borttagningsåtgärd.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Hämtar åtgärdstypen för denna revision. |
| [getCellArea()](#getCellArea--) | Hämtar infognings-/borttagningsintervallet. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Hämtar numret för den här revisionen. |
| [getRevisions()](#getRevisions--) | Hämtar revisionslistan för denna operation. |
| [getType()](#getType--) | Representerar revisionstypen. |
| [getWorksheet()](#getWorksheet--) | Hämtar kalkylbladet. |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getActionType() {#getActionType--}
```
public int getActionType()
```


Hämtar åtgärdstypen för denna revision.

Se [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Hämtar infognings-/borttagningsintervallet.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getId() {#getId--}
```
public int getId()
```


Hämtar numret för den här revisionen.

**Remarks**

Noll betyder att den här revisionen inte innehåller ID.

**Returns:**
int
### getRevisions() {#getRevisions--}
```
public RevisionCollection getRevisions()
```


Hämtar revisionslistan för denna operation.

**Returns:**
[RevisionCollection](../../com.aspose.cells/revisioncollection)
### getType() {#getType--}
```
public int getType()
```


Representerar revisionstypen.

Se [RevisionType](../../com.aspose.cells/revisiontype).

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Hämtar kalkylbladet.

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

