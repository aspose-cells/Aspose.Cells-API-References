---
title: "RevisionCellComment"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en revisionspost för en ändring av cellkommentar."
type: docs
url: /sv/java/com.aspose.cells/revisioncellcomment/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellComment extends Revision
```

Representerar en revisionspost för en ändring av cellkommentar.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getActionType()](#getActionType--) | Hämtar åtgärdstypen för revisionen. |
| [getCellName()](#getCellName--) | Hämtar namnet på cellen. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hämtar kolumnindex för den som innehåller en kommentar. |
| [getId()](#getId--) | Hämtar numret för den här revisionen. |
| [getNewLength()](#getNewLength--) | Hämtar längden på kommentaren innan den här revisionen gjordes. |
| [getOldLength()](#getOldLength--) | Hämtar längden på kommentartexten som lades till i den här revisionen. |
| [getRow()](#getRow--) | Hämtar radindex för den som innehåller en kommentar. |
| [getType()](#getType--) | Hämtar typen av revision. |
| [getWorksheet()](#getWorksheet--) | Hämtar kalkylbladet. |
| [hashCode()](#hashCode--) |  |
| [isOldComment()](#isOldComment--) | Indikerar om det är en gammal kommentar. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCellName(String value)](#setCellName-java.lang.String-) | Hämtar namnet på cellen. |
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


Hämtar åtgärdstypen för revisionen.

Se [RevisionActionType](../../com.aspose.cells/revisionactiontype).

**Returns:**
int
### getCellName() {#getCellName--}
```
public String getCellName()
```


Hämtar namnet på cellen.

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


Hämtar kolumnindex för den som innehåller en kommentar.

**Returns:**
int
### getId() {#getId--}
```
public int getId()
```


Hämtar numret för den här revisionen.

**Remarks**

Noll betyder att den här revisionen inte innehåller ID.

**Returns:**
int
### getNewLength() {#getNewLength--}
```
public int getNewLength()
```


Hämtar längden på kommentaren innan den här revisionen gjordes.

**Returns:**
int
### getOldLength() {#getOldLength--}
```
public int getOldLength()
```


Hämtar längden på kommentartexten som lades till i den här revisionen.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Hämtar radindex för den som innehåller en kommentar.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Hämtar typen av revision.

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
### isOldComment() {#isOldComment--}
```
public boolean isOldComment()
```


Indikerar om det är en gammal kommentar.

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


Hämtar namnet på cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

