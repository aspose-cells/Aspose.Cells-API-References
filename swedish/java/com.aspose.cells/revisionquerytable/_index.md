---
title: "RevisionQueryTable"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en revision av en ändring av ett frågetabellfält."
type: docs
url: /sv/java/com.aspose.cells/revisionquerytable/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionQueryTable extends Revision
```

Representerar en revision av en ändring av ett frågetabellfält.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellArea()](#getCellArea--) | Hämtar platsen för den påverkade frågetabellen. |
| [getClass()](#getClass--) |  |
| [getFieldId()](#getFieldId--) | Hämtar ID för det specifika fältet i frågetabellen som togs bort. |
| [getId()](#getId--) | Hämtar numret för den här revisionen. |
| [getType()](#getType--) | Representerar typen av revisionen. |
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
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


Hämtar platsen för den påverkade frågetabellen.

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


Hämtar ID för det specifika fältet i frågetabellen som togs bort.

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
### getType() {#getType--}
```
public int getType()
```


Representerar typen av revisionen.

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

