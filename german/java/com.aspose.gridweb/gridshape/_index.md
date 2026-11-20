---
title: "GridShape"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt ein Shape-Objekt dar."
type: docs
url: /de/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

Stellt ein Shape-Objekt dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | Liefert den Puffer des Objekts. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | Liefert die Sets-ID für die Form. |
| [getLeft()](#getLeft--) | Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln. |
| [getLeftToCorner()](#getLeftToCorner--) | Stellt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts dar, in Pixeln. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Liefert den mso-Zeichnungstyp. |
| [getName()](#getName--) | Ermittelt den Namen der Form. |
| [getText()](#getText--) | Stellt die Zeichenkette in diesem TextBox-Objekt dar. |
| [getTop()](#getTop--) | Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar. |
| [getTopToCorner()](#getTopToCorner--) | Stellt den vertikalen Versatz der shape vom oberen Rand des Arbeitsblatts dar, in Pixeln. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Stellt den Spaltenindex der oberen linken Ecke dar. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Stellt den Zeilenindex der oberen linken Ecke dar. |
| [getZOrderPosition()](#getZOrderPosition--) | Gibt die Position einer Form in der Z-Reihenfolge zurück. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Erstellt das Bild und speichert es in einen Stream im angegebenen PNG-Format. |
| [setID(String value)](#setID-java.lang.String-) | Liefert die Sets-ID für die Form. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Stellt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts dar, in Pixeln. |
| [setText(String value)](#setText-java.lang.String-) | Stellt die Zeichenkette in diesem TextBox-Objekt dar. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Stellt den vertikalen Versatz der shape vom oberen Rand des Arbeitsblatts dar, in Pixeln. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Gibt die Position einer Form in der Z-Reihenfolge zurück. |
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
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


Liefert den Puffer des Objekts.

**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getID() {#getID--}
```
public String getID()
```


Liefert die Sets-ID für die Form.

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


Stellt den horizontalen Versatz der Form von ihrer linken Spalte dar, in Einheiten von Pixeln.

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Stellt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts dar, in Pixeln.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Liefert den mso-Zeichnungstyp.

Siehe [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ermittelt den Namen der Form.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Stellt die Zeichenkette in diesem TextBox-Objekt dar.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Stellt den vertikalen Versatz der Form von ihrer oberen Zeile in Pixeln dar.

**Remarks**

Wenn das Shape im Diagramm ist, stellt es den vertikalen Versatz des Shapes von seiner oberen Kante dar.

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Stellt den vertikalen Versatz der shape vom oberen Rand des Arbeitsblatts dar, in Pixeln.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Stellt den Spaltenindex der oberen linken Ecke dar.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Stellt den Zeilenindex der oberen linken Ecke dar.

**Remarks**

Wenn das Shape im Shape oder in der Gruppe ist, wird UpperLeftRow ignoriert.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Gibt die Position einer Form in der Z-Reihenfolge zurück.

**Returns:**
int
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




### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Erstellt das Bild und speichert es in einen Stream im angegebenen PNG-Format.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Liefert die Sets-ID für die Form.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Stellt den horizontalen Versatz der shape vom linken Rand des Arbeitsblatts dar, in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Stellt die Zeichenkette in diesem TextBox-Objekt dar.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Stellt den vertikalen Versatz der shape vom oberen Rand des Arbeitsblatts dar, in Pixeln.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Gibt die Position einer Form in der Z-Reihenfolge zurück.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

