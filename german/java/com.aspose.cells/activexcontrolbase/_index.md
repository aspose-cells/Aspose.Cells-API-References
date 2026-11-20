---
title: "ActiveXControlBase"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt das ActiveX‑Steuerelement dar."
type: docs
url: /de/java/com.aspose.cells/activexcontrolbase/
---

**Inheritance:**
java.lang.Object
```
public abstract class ActiveXControlBase
```

Stellt das ActiveX‑Steuerelement dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackOleColor()](#getBackOleColor--) | Liefert die OLE-Farbe des Hintergrunds. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Ermittelt die Binärdaten des Steuerelements. |
| [getForeOleColor()](#getForeOleColor--) | Ermittelt die OLE-Farbe des Vordergrunds. |
| [getHeight()](#getHeight--) | Ermittelt die Höhe des Steuerelements in Punkten. |
| [getLinkedCell()](#getLinkedCell--) | Ermittelt die verknüpfte Zelle. |
| [getListFillRange()](#getListFillRange--) | Ermittelt den Ausfüllbereich der Liste. |
| [getMouseIcon()](#getMouseIcon--) | Ermittelt ein benutzerdefiniertes Symbol, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [getMousePointer()](#getMousePointer--) | Ermittelt den Typ des Symbols, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [getShadow()](#getShadow--) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [getType()](#getType--) | Ermittelt den Typ des ActiveX-Steuerelements. |
| [getWidth()](#getWidth--) | Liest die Breite des Steuerelements in Punkten. |
| [getWorkbook()](#getWorkbook--) | Liest das [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) Objekt. |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackOleColor(int value)](#setBackOleColor-int-) | Legt die OLE-Farbe des Hintergrunds fest. |
| [setForeOleColor(int value)](#setForeOleColor-int-) | Legt die OLE-Farbe des Vordergrunds fest. |
| [setHeight(double value)](#setHeight-double-) | Legt die Höhe des Steuerelements in Punkten fest. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Legt die verknüpfte Zelle fest. |
| [setListFillRange(String value)](#setListFillRange-java.lang.String-) | Legt den Listenfüllbereich fest. |
| [setMouseIcon(byte[] value)](#setMouseIcon-byte---) | Legt ein benutzerdefiniertes Symbol fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [setMousePointer(int value)](#setMousePointer-int-) | Legt den Typ des Symbols fest, das als Mauszeiger für das Steuerelement angezeigt wird. |
| [setShadow(boolean value)](#setShadow-boolean-) | Gibt an, ob ein Schatten angezeigt werden soll. |
| [setVisible(boolean value)](#setVisible-boolean-) | Gibt an, ob dieses Steuerelement sichtbar ist. |
| [setWidth(double value)](#setWidth-double-) | Legt die Breite des Steuerelements in Punkten fest. |
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
### getBackOleColor() {#getBackOleColor--}
```
public int getBackOleColor()
```


Liefert die OLE-Farbe des Hintergrunds.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Ermittelt die Binärdaten des Steuerelements.

**Returns:**
byte[]
### getForeOleColor() {#getForeOleColor--}
```
public int getForeOleColor()
```


Ermittelt die OLE-Farbe des Vordergrunds.

**Remarks**

Gilt nicht für das Image-Steuerelement.

**Returns:**
int
### getHeight() {#getHeight--}
```
public double getHeight()
```


Ermittelt die Höhe des Steuerelements in Punkten.

**Returns:**
double
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


Ermittelt die verknüpfte Zelle.

**Returns:**
java.lang.String
### getListFillRange() {#getListFillRange--}
```
public String getListFillRange()
```


Ermittelt den Ausfüllbereich der Liste.

**Returns:**
java.lang.String
### getMouseIcon() {#getMouseIcon--}
```
public byte[] getMouseIcon()
```


Ermittelt ein benutzerdefiniertes Symbol, das als Mauszeiger für das Steuerelement angezeigt wird.

**Returns:**
byte[]
### getMousePointer() {#getMousePointer--}
```
public int getMousePointer()
```


Ermittelt den Typ des Symbols, das als Mauszeiger für das Steuerelement angezeigt wird.

Siehe [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Returns:**
int
### getShadow() {#getShadow--}
```
public boolean getShadow()
```


Gibt an, ob ein Schatten angezeigt werden soll.

**Returns:**
boolean
### getType() {#getType--}
```
public abstract int getType()
```


Ermittelt den Typ des ActiveX-Steuerelements.

Siehe [ControlType](../../com.aspose.cells/controltype).

**Returns:**
int
### getWidth() {#getWidth--}
```
public double getWidth()
```


Liest die Breite des Steuerelements in Punkten.

**Returns:**
double
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Liest das [getWorkbook()](../../com.aspose.cells/activexcontrolbase\#getWorkbook--) Objekt.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isVisible() {#isVisible--}
```
public boolean isVisible()
```


Gibt an, ob dieses Steuerelement sichtbar ist.

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




### setBackOleColor(int value) {#setBackOleColor-int-}
```
public void setBackOleColor(int value)
```


Legt die OLE-Farbe des Hintergrunds fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setForeOleColor(int value) {#setForeOleColor-int-}
```
public void setForeOleColor(int value)
```


Legt die OLE-Farbe des Vordergrunds fest.

**Remarks**

Gilt nicht für das Image-Steuerelement.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Legt die Höhe des Steuerelements in Punkten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Legt die verknüpfte Zelle fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setListFillRange(String value) {#setListFillRange-java.lang.String-}
```
public void setListFillRange(String value)
```


Legt den Listenfüllbereich fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | java.lang.String |  |

### setMouseIcon(byte[] value) {#setMouseIcon-byte---}
```
public void setMouseIcon(byte[] value)
```


Legt ein benutzerdefiniertes Symbol fest, das als Mauszeiger für das Steuerelement angezeigt wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | byte[] |  |

### setMousePointer(int value) {#setMousePointer-int-}
```
public void setMousePointer(int value)
```


Legt den Typ des Symbols fest, das als Mauszeiger für das Steuerelement angezeigt wird.

Siehe [ControlMousePointerType](../../com.aspose.cells/controlmousepointertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShadow(boolean value) {#setShadow-boolean-}
```
public void setShadow(boolean value)
```


Gibt an, ob ein Schatten angezeigt werden soll.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Gibt an, ob dieses Steuerelement sichtbar ist.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setWidth(double value) {#setWidth-double-}
```
public void setWidth(double value)
```


Legt die Breite des Steuerelements in Punkten fest.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | double |  |

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

