---
title: "CellsColor"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla typer av färg."
type: docs
url: /sv/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

Representerar alla typer av färg.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | Hämtar färgen från ett 32‑bit ARGB‑värde. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Hämtar RGB‑färgen. |
| [getColorIndex()](#getColorIndex--) | Hämtar färgindexet i färgpaletten. |
| [getThemeColor()](#getThemeColor--) | Hämtar temafärgen. |
| [getTransparency()](#getTransparency--) | Hämtar transparensen som ett värde från 0,0 (opak) till 1,0 (genomskinlig). |
| [getType()](#getType--) | Färgtypen. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | Hämtar färgen som ska tillämpas på cell eller form. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | Ställer in färgen från ett 32‑bit ARGB‑värde. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Ställer in RGB‑färgen. |
| [setColorIndex(int value)](#setColorIndex-int-) | Ställer in färgindexet i färgpaletten. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | Ställer in färgen som ska tillämpas på cell eller form. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Hämtar temafärgen. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | Ställ in nyansen för formens färg |
| [setTransparency(double value)](#setTransparency-double-) | Ställer in transparensen som ett värde från 0,0 (opak) till 1,0 (genomskinlig). |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```


Hämtar färgen från ett 32‑bit ARGB‑värde.

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


Hämtar RGB‑färgen.

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


Hämtar färgindexet i färgpaletten. Gäller endast för indexerad färg.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Hämtar temafärgen. Gäller endast för temafärgstyp.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


Hämtar transparensen som ett värde från 0,0 (opak) till 1,0 (genomskinlig).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


Färgtypen.

Se [ColorType](../../com.aspose.cells/colortype).

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


Hämtar färgen som ska tillämpas på cell eller form.

**Remarks**

Uttrycket för färgen på cellen och formen är olika. Till exempel kommer temafärgen med samma nyansvärde inte att vara densamma i cellen och i formen.

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


Ställer in färgen från ett 32‑bit ARGB‑värde.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Ställer in RGB‑färgen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


Ställer in färgindexet i färgpaletten. Gäller endast för indexerad färg.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


Ställer in färgen som ska tillämpas på cell eller form.

**Remarks**

Uttrycket för färgen på cellen och formen är olika. Till exempel kommer temafärgen med samma nyansvärde inte att vara densamma i cellen och i formen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Hämtar temafärgen. Gäller endast för temafärgstyp.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


Ställ in nyansen för formens färg

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| tint | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


Ställer in transparensen som ett värde från 0,0 (opak) till 1,0 (genomskinlig).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | double |  |

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

