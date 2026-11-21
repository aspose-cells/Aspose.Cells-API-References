---
title: "GridHyperlinkCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

Inkapslar en samling av [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Lägger till en hyperlänk i en angiven cell eller ett cellområde. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Lägger till en hyperlänk i en angiven cell eller ett cellområde. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | Lägger till en hyperlänk i en specificerad cell. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Lägger till en hyperlänk i en angiven cell eller ett cellområde. |
| [clear()](#clear--) | Rensar alla hyperlänkar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) elementet vid det specificerade indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar storleken på enumeratorn |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | Hämtar cellens Hyperlink-objekt. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | Hämtar cellens Hyperlink-objekt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | Ta bort hyperlänken i det specificerade området. |
| [removeAt(int index)](#removeAt-int-) | Ta bort hyperlänken på det angivna indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Lägger till en hyperlänk i en angiven cell eller ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| firstRow | int | Första raden i hyperlänksområdet. |
| firstColumn | int | Första kolumnen i hyperlänksområdet. |
| totalRows | int | Antal rader i detta hyperlänksområde. |
| totalColumns | int | Antal kolumner i detta hyperlänksområde. |
| adress | java.lang.String | Adress för hyperlänken. |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) objektindex.
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


Lägger till en hyperlänk i en angiven cell eller ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |
| totalRows | int | Antal rader i detta hyperlänksområde. |
| totalColumns | int | Antal kolumner i detta hyperlänksområde. |
| adress | java.lang.String | Adress för hyperlänken. |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) objektindex.
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


Lägger till en hyperlänk i en specificerad cell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cellNamn | java.lang.String | Cellnamn. |
| adress | java.lang.String | Adress för hyperlänken. |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) objektindex.
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


Lägger till en hyperlänk i en angiven cell eller ett cellområde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| startCellName | java.lang.String | Den övre vänstra cellen i området. |
| endCellName | java.lang.String | Den nedre högra cellen i området. |
| adress | java.lang.String | Adress för hyperlänken. |
| textToDisplay | java.lang.String | Texten som ska visas för den angivna hyperlänken. |
| screenTip | java.lang.String | ScreenTip-texten för den angivna hyperlänken. |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) objektindex.
### clear() {#clear--}
```
public void clear()
```


Rensar alla hyperlänkar.

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
### get(int index) {#get-int-}
```
public GridHyperlink get(int index)
```


Hämtar [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) elementet vid det specificerade indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Hämtar storleken på enumeratorn

**Returns:**
int
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


Hämtar cellens Hyperlink-objekt. Om cellen inte har någon Hyperlink returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | GridCell-objektet. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


Hämtar cellens Hyperlink-objekt. Om cellen inte har någon Hyperlink returneras null.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rad | int | Raden för cellen. |
| kolumn | int | Kolumnen för cellen. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
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




### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```


Ta bort hyperlänken i det specificerade området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Området som innehåller hyperlänken. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Ta bort hyperlänken på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

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

