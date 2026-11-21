---
title: "GridRow"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar objektet som representerar en enskild bild i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

Inkapslar objektet som representerar en enskild bild i ett kalkylblad.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | Hämtar cellen. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Hämta cellen med ett specifikt index i listan. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Hämtar den första cellen i raden. |
| [getHeight()](#getHeight--) | Hämtar radens höjd i enheten Points. |
| [getHidden()](#getHidden--) | Anger om raden är dold. |
| [getIndex()](#getIndex--) | Hämtar indexet för denna rad. |
| [getLastCell()](#getLastCell--) | Hämtar den sista cellen i raden. |
| [getLastDataCell()](#getLastDataCell--) | Hämtar den sista cellen i raden. |
| [getOutlineLevel()](#getOutlineLevel--) | Hämtar konturnivån. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Anger om raden innehåller någon data |
| [iterator()](#iterator--) | Hämtar cellernas enumerator |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | Ställer in radhöjden i enheten punkter. |
| [setHidden(boolean value)](#setHidden-boolean-) | Anger om raden är dold. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | Ställer in konturnivån. |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


Hämtar cellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| kolumn | int | Kolumnindexet |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


Hämta cellen med ett specifikt index i listan.

**Remarks**

NOTE: Denna medlem är nu föråldrad. Använd istället Row.GetEnumerator()-metoden för att iterera alla celler i den här raden. Denna egenskap kommer att tas bort 12 månader senare, sedan februari 2015. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The Cell object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Hämtar den första cellen i raden.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


Hämtar radens höjd i enheten Points.

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


Anger om raden är dold.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Hämtar indexet för denna rad.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Hämtar den sista cellen i raden.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


Hämtar den sista cellen i raden.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


Hämtar konturnivån.

**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Anger om raden innehåller någon data

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hämtar cellernas enumerator

**Returns:**
java.util.Iterator - Cellernas enumerator
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Ställer in radhöjden i enheten punkter.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Anger om raden är dold.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


Ställer in konturnivån.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | byte |  |

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

