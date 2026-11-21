---
title: "RevisionCellChange"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar revisionen som ändrar celler."
type: docs
url: /sv/java/com.aspose.cells/revisioncellchange/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Revision](../../com.aspose.cells/revision)
```
public class RevisionCellChange extends Revision
```

Representerar revisionen som ändrar celler.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellName()](#getCellName--) | Hämtar namnet på cellen. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Hämtar kolumnindex för cellen. |
| [getId()](#getId--) | Hämtar numret för den här revisionen. |
| [getNewFormula()](#getNewFormula--) | Hämtar den gamla formeln. |
| [getNewStyle()](#getNewStyle--) | Hämtar den nya stilen för cellen. |
| [getNewValue()](#getNewValue--) | Hämtar det nya värdet för cellen. |
| [getOldFormula()](#getOldFormula--) | Hämtar den gamla formeln. |
| [getOldStyle()](#getOldStyle--) | Hämtar den gamla stilen för cellen. |
| [getOldValue()](#getOldValue--) | Hämtar det gamla värdet för cellen. |
| [getRow()](#getRow--) | Hämtar radindex för cellen. |
| [getType()](#getType--) | Representerar revisionstypen. |
| [getWorksheet()](#getWorksheet--) | Hämtar kalkylbladet. |
| [hashCode()](#hashCode--) |  |
| [isNewFormatted()](#isNewFormatted--) | Indikerar om den här cellen är nyformaterad. |
| [isOldFormatted()](#isOldFormatted--) | Indikerar om den här cellen är gammalformaterad. |
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


Hämtar kolumnindex för cellen.

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
### getNewFormula() {#getNewFormula--}
```
public String getNewFormula()
```


Hämtar den gamla formeln.

**Returns:**
java.lang.String
### getNewStyle() {#getNewStyle--}
```
public Style getNewStyle()
```


Hämtar den nya stilen för cellen.

**Returns:**
[Style](../../com.aspose.cells/style)
### getNewValue() {#getNewValue--}
```
public Object getNewValue()
```


Hämtar det nya värdet för cellen.

**Returns:**
java.lang.Object
### getOldFormula() {#getOldFormula--}
```
public String getOldFormula()
```


Hämtar den gamla formeln.

**Returns:**
java.lang.String
### getOldStyle() {#getOldStyle--}
```
public Style getOldStyle()
```


Hämtar den gamla stilen för cellen.

**Returns:**
[Style](../../com.aspose.cells/style)
### getOldValue() {#getOldValue--}
```
public Object getOldValue()
```


Hämtar det gamla värdet för cellen.

**Returns:**
java.lang.Object
### getRow() {#getRow--}
```
public int getRow()
```


Hämtar radindex för cellen.

**Returns:**
int
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
### isNewFormatted() {#isNewFormatted--}
```
public boolean isNewFormatted()
```


Indikerar om den här cellen är nyformaterad.

**Returns:**
boolean
### isOldFormatted() {#isOldFormatted--}
```
public boolean isOldFormatted()
```


Indikerar om den här cellen är gammalformaterad.

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

