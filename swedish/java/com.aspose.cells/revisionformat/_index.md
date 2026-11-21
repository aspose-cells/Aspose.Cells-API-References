---
title: "RevisionFormat"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en revisionspost med information om en formateringsändring."
type: docs
url: /sv/java/com.aspose.cells/revisionformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionFormat extends Revision
```

Representerar en revisionspost med information om en formateringsändring.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Det intervall som denna formatering tillämpades på. |
| [getClass()](#getClass--) |  |
| [getId()](#getId--) | Hämtar numret för den här revisionen. |
| [getStyle()](#getStyle--) | Hämtar den tillämpade stilen. |
| [getType()](#getType--) | Hämtar typen av revision. |
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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


Det intervall som denna formatering tillämpades på.

**Returns:**
com.aspose.cells.CellArea[]
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
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Hämtar den tillämpade stilen.

**Returns:**
[Style](../../com.aspose.cells/style)
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

