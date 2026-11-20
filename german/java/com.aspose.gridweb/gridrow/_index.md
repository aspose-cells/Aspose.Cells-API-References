---
title: "GridRow"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das ein einzelnes Bild in einer Tabellenkalkulation darstellt."
type: docs
url: /de/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

Kapselt das Objekt, das ein einzelnes Bild in einer Tabellenkalkulation darstellt.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | Liefert die Zelle. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Rufen Sie die Zelle über einen bestimmten Index in der Liste ab. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Gibt die erste Zelle in der Zeile zurück. |
| [getHeight()](#getHeight--) | Ermittelt die Zeilenhöhe in Punkten. |
| [getHidden()](#getHidden--) | Gibt an, ob die Zeile ausgeblendet ist. |
| [getIndex()](#getIndex--) | Ermittelt den Index dieser Zeile. |
| [getLastCell()](#getLastCell--) | Gibt die letzte Zelle in der Zeile zurück. |
| [getLastDataCell()](#getLastDataCell--) | Gibt die letzte Zelle in der Zeile zurück. |
| [getOutlineLevel()](#getOutlineLevel--) | Gibt die Gliederungsebene zurück. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Gibt an, ob die Zeile Daten enthält. |
| [iterator()](#iterator--) | Ermittelt den Zellen-Enumerator |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | Setzt die Zeilenhöhe in Punkten. |
| [setHidden(boolean value)](#setHidden-boolean-) | Gibt an, ob die Zeile ausgeblendet ist. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | Setzt die Gliederungsebene. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


Liefert die Zelle.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Spalte | int | Der Spaltenindex |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


Rufen Sie die Zelle über einen bestimmten Index in der Liste ab.

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Row.GetEnumerator(), um alle Zellen in dieser Zeile zu iterieren. Diese Eigenschaft wird 12 Monate später, seit Februar 2015, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie erlebt haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position. |

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


Gibt die erste Zelle in der Zeile zurück.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


Ermittelt die Zeilenhöhe in Punkten.

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


Gibt an, ob die Zeile ausgeblendet ist.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ermittelt den Index dieser Zeile.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Gibt die letzte Zelle in der Zeile zurück.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


Gibt die letzte Zelle in der Zeile zurück.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


Gibt die Gliederungsebene zurück.

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


Gibt an, ob die Zeile Daten enthält.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ermittelt den Zellen-Enumerator

**Returns:**
java.util.Iterator - Der Zellen‑Enumerator
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


Setzt die Zeilenhöhe in Punkten.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Gibt an, ob die Zeile ausgeblendet ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


Setzt die Gliederungsebene.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte |  |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

