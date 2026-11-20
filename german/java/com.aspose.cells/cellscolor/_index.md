---
title: "ZellenFarbe"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt alle Farbtypen dar."
type: docs
url: /de/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

Stellt alle Farbtypen dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | Liest die Farbe aus einem 32‑Bit‑ARGB‑Wert. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Liest die RGB‑Farbe. |
| [getColorIndex()](#getColorIndex--) | Liest den Farbindex in der Farbpalette. |
| [getThemeColor()](#getThemeColor--) | Ermittelt die Designfarbe. |
| [getTransparency()](#getTransparency--) | Liest die Transparenz als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| [getType()](#getType--) | Der Farbtyp. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | Liest die Farbe, die auf Zelle oder Form angewendet werden soll. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | Setzt die Farbe aus einem 32‑Bit‑ARGB‑Wert. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Setzt die RGB‑Farbe. |
| [setColorIndex(int value)](#setColorIndex-int-) | Setzt den Farbindex in der Farbpalette. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | Setzt die Farbe, die auf Zelle oder Form angewendet werden soll. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Ermittelt die Designfarbe. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | Setzt den Farbton der Formfarbe |
| [setTransparency(double value)](#setTransparency-double-) | Setzt die Transparenz als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```


Liest die Farbe aus einem 32‑Bit‑ARGB‑Wert.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```


Liest die RGB‑Farbe.

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


Liest den Farbindex in der Farbpalette. Gilt nur für indizierte Farben.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Liest die Designfarbe. Gilt nur für den Designfarbtyp.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Liest die Transparenz als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Der Farbtyp.

Siehe [ColorType](../../com.aspose.cells/colortype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isShapeColor() {#isShapeColor--}
```
public boolean isShapeColor()
```


Liest die Farbe, die auf Zelle oder Form angewendet werden soll.

**Remarks**

Der Ausdruck der Farbe von Zelle und Form ist unterschiedlich. Zum Beispiel wird die Designfarbe mit demselben Farbtonwert in der Zelle und der Form nicht gleich sein.

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




### setArgb(int value) {#setArgb-int-}
```
public void setArgb(int value)
```


Setzt die Farbe aus einem 32‑Bit‑ARGB‑Wert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Setzt die RGB‑Farbe.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


Setzt den Farbindex in der Farbpalette. Gilt nur für indizierte Farben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


Setzt die Farbe, die auf Zelle oder Form angewendet werden soll.

**Remarks**

Der Ausdruck der Farbe von Zelle und Form ist unterschiedlich. Zum Beispiel wird die Designfarbe mit demselben Farbtonwert in der Zelle und der Form nicht gleich sein.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Liest die Designfarbe. Gilt nur für den Designfarbtyp.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


Setzt den Farbton der Formfarbe

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Farbton | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Setzt die Transparenz als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent).

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

