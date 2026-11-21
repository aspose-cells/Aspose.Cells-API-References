---
title: "GridShape"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar ett formobjekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridshape/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridShape implements IGridSave
```

Representerar ett formobjekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuffer()](#getBuffer--) | Hämtar bufferten för objektet. |
| [getClass()](#getClass--) |  |
| [getID()](#getID--) | Hämtar Sets ID för formen. |
| [getLeft()](#getLeft--) | Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar. |
| [getLeftToCorner()](#getLeftToCorner--) | Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enheten pixlar. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Hämtar mso-ritningstyp. |
| [getName()](#getName--) | Hämtar namnet på formen. |
| [getText()](#getText--) | Representerar strängen i detta TextBox-objekt. |
| [getTop()](#getTop--) | Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar. |
| [getTopToCorner()](#getTopToCorner--) | Representerar det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Representerar index för övre vänstra kolumnen. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Representerar radindex för övre vänstra hörnet. |
| [getZOrderPosition()](#getZOrderPosition--) | Returnerar positionen för en shape i z-ordningen. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Skapar bilden och sparar den till en ström i det angivna png-formatet. |
| [setID(String value)](#setID-java.lang.String-) | Hämtar Sets ID för formen. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enheten pixlar. |
| [setText(String value)](#setText-java.lang.String-) | Representerar strängen i detta TextBox-objekt. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Representerar det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Returnerar positionen för en shape i z-ordningen. |
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
### getBuffer() {#getBuffer--}
```
public byte[] getBuffer()
```


Hämtar bufferten för objektet.

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


Hämtar Sets ID för formen.

**Returns:**
java.lang.String
### getLeft() {#getLeft--}
```
public int getLeft()
```


Representerar den horisontella förskjutningen av formen från dess vänstra kolumn, i enhet pixlar.

**Returns:**
int
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enheten pixlar.

**Returns:**
int
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Hämtar mso-ritningstyp.

Se [GridMsoDrawingType](../../com.aspose.gridweb/gridmsodrawingtype).

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Hämtar namnet på formen.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Representerar strängen i detta TextBox-objekt.

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Representerar den vertikala förskjutningen för formen från dess översta rad, i enheten pixlar.

**Remarks**

Om formen är i diagrammet, representerar den vertikala förskjutningen av formen från dess övre kant.

**Returns:**
int
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


Representerar det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Representerar index för övre vänstra kolumnen.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Representerar radindex för övre vänstra hörnet.

**Remarks**

Om formen är i en form eller i en grupp, kommer UpperLeftRow att ignoreras.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Returnerar positionen för en shape i z-ordningen.

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


Skapar bilden och sparar den till en ström i det angivna png-formatet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


Hämtar Sets ID för formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kant, i enheten pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Representerar strängen i detta TextBox-objekt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Representerar det vertikala offsetet för formen från kalkylbladets övre kant, i enhet pixlar.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Returnerar positionen för en shape i z-ordningen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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

