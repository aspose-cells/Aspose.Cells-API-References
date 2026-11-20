---
title: "Rahmen"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Kapselt das Objekt, das den Zellenrand darstellt."
type: docs
url: /de/java/com.aspose.cells/border/
---

**Inheritance:**
java.lang.Object
```
public class Border
```

Kapselt das Objekt, das den Zellenrand darstellt.

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
         Cell cell = sheets.get(0).getCells().get("A1");
 
         Style style = cell.getStyle();
         //Set top border style and color
         Border border = style.getBorders().getByBorderType(BorderType.TOP_BORDER);
         border.setLineStyle(CellBorderType.MEDIUM);
         border.setColor(Color.getRed());
         cell.setStyle(style);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgbColor()](#getArgbColor--) | Liest die Farbe mit einem 32‑Bit‑ARGB‑Wert. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Liest das [Color](../../com.aspose.cells/color) des Rahmens. |
| [getLineStyle()](#getLineStyle--) | Liest den Zellenrahmentyp. |
| [getThemeColor()](#getThemeColor--) | Liest die Themenfarbe des Rahmens. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgbColor(int value)](#setArgbColor-int-) | Setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Setzt das [Color](../../com.aspose.cells/color) des Rahmens. |
| [setLineStyle(int value)](#setLineStyle-int-) | Setzt den Zellenrahmentyp. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | Setzt die Themenfarbe des Rahmens. |
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
### getArgbColor() {#getArgbColor--}
```
public int getArgbColor()
```


Liest die Farbe mit einem 32‑Bit‑ARGB‑Wert.

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


Liest das [Color](../../com.aspose.cells/color) des Rahmens.

**Returns:**
[Color](../../com.aspose.cells/color)
### getLineStyle() {#getLineStyle--}
```
public int getLineStyle()
```


Liest den Zellenrahmentyp.

Siehe [CellBorderType](../../com.aspose.cells/cellbordertype).

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


Liest die Themenfarbe des Rahmens.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
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




### setArgbColor(int value) {#setArgbColor-int-}
```
public void setArgbColor(int value)
```


Setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


Setzt das [Color](../../com.aspose.cells/color) des Rahmens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setLineStyle(int value) {#setLineStyle-int-}
```
public void setLineStyle(int value)
```


Setzt den Zellenrahmentyp.

Siehe [CellBorderType](../../com.aspose.cells/cellbordertype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


Setzt die Themenfarbe des Rahmens.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

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

