---
title: "CellArea"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett område av celler."
type: docs
url: /sv/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

Representerar ett område av celler.

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## Fält

| Fält | Beskrivning |
| --- | --- |
| [EndColumn](#EndColumn) | Hämtar eller anger slutkolumnen för detta område. |
| [EndRow](#EndRow) | Hämtar eller anger slutraden för detta område. |
| [StartColumn](#StartColumn) | Hämtar eller anger startkolumnen för detta område. |
| [StartRow](#StartRow) | Hämtar eller anger startraden för detta område. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | Jämför två CellArea-objekt enligt deras övre vänstra hörn. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | Skapar ett cellområde. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | Skapar ett cellområde. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Returnerar en sträng som representerar det aktuella cellområdeobjektet. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


Hämtar eller anger slutkolumnen för detta område.

### EndRow {#EndRow}
```
public int EndRow
```


Hämtar eller anger slutraden för detta område.

### StartColumn {#StartColumn}
```
public int StartColumn
```


Hämtar eller anger startkolumnen för detta område.

### StartRow {#StartRow}
```
public int StartRow
```


Hämtar eller anger startraden för detta område.

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


Jämför två CellArea-objekt enligt deras övre vänstra hörn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int - Om två hörn är i olika rader jämförs deras radindex. Annars jämförs deras kolumnindex. Om två hörn är lika returneras 0.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


Skapar ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startRad | int | Startrad. |
| startColumn | int | Startkolumnen. |
| slutRad | int | Slutrad. |
| endColumn | int | Slutkolumn. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


Skapar ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startCellName | java.lang.String | Den övre vänstra cellen i området. |
| endCellName | java.lang.String | Den nedre högra cellen i området. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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


Returnerar en sträng som representerar det aktuella cellområdeobjektet.

**Returns:**
java.lang.String -
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

