---
title: "GradientFill"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die Farbverlaufsfüllung dar."
type: docs
url: /de/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

Stellt die Farbverlaufsfüllung dar.
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | Der Winkel der linearen Füllung. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Ermittelt den Gradientenrichtungs‑Typ. |
| [getFillType()](#getFillType--) | Ermittelt den Gradientenfüllungs‑Typ. |
| [getGradientColor1()](#getGradientColor1--) | Ermittelt die erste Farbverlauffarbe. |
| [getGradientColor2()](#getGradientColor2--) | Ermittelt die zweite Farbverlauffarbe. |
| [getGradientColorType()](#getGradientColorType--) | Ermittelt den Farbverlauf‑Farbtyp. |
| [getGradientDegree()](#getGradientDegree--) | Ermittelt den Gradientenwinkel. |
| [getGradientStops()](#getGradientStops--) | Stellt die Sammlung von Farbverlaufspunkten dar. |
| [getGradientStyle()](#getGradientStyle--) | Ermittelt den Gradientenstil‑Typ. |
| [getPresetColor()](#getPresetColor--) | Gibt die voreingestellte Farbverlauffarbe für die angegebene Füllung zurück. |
| [getVariant()](#getVariant--) | Ermittelt Variante. |
| [hashCode()](#hashCode--) | Ermittelt den Hashcode. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | Der Winkel der linearen Füllung. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | Setzt den Gradientenfüllungs‑Typ und die Richtung. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Setzt die angegebene Füllung auf einen einfarbigen Farbverlauf. |
| [setPresetColor(int value)](#setPresetColor-int-) | Gibt die voreingestellte Farbverlauffarbe für die angegebene Füllung zurück. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Setzt die angegebene Füllung auf einen voreingestellten Farbverlauf. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | Setzt vordefinierte Themen‑Gradientenfüllung. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


/

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


Der Winkel der linearen Füllung.

**Returns:**
float
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Ermittelt den Gradientenrichtungs‑Typ.

Siehe [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Ermittelt den Gradientenfüllungs‑Typ.

Siehe [GradientFillType](../../com.aspose.cells/gradientfilltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Ermittelt die erste Farbverlauffarbe. Gilt für Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Ermittelt die zweite Farbverlauffarbe. Gilt für Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Ermittelt den Farbverlauf‑Farbtyp. Gilt für Excel97-2003

Siehe [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Ermittelt den Gradientenwinkel. Gilt für Excel97-2003

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


Stellt die Sammlung von Farbverlaufspunkten dar.

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Ermittelt den Gradientenstil‑Typ. Gilt für Excel97-2003

Siehe [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Gibt die vordefinierte Gradientfarbe für die angegebene Füllung zurück. Gilt für Excel97-2003

Siehe [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


Ermittelt Variante. Gilt für Excel97-2003

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Ermittelt den Hashcode.

**Returns:**
int -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAngle(float value) {#setAngle-float-}
```
public void setAngle(float value)
```


Der Winkel der linearen Füllung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


Setzt den Gradientenfüllungs‑Typ und die Richtung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). Gradientenfüllungs‑Typ. |
| Winkel | double | Der Winkel. Gilt nur für GradientFillType.Linear. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). Der Richtungstyp. Gilt nur für GradientFillType.Radial und GradientFillType.Rectangle. |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Setzt die angegebene Füllung auf einen Einfarbverlauf. Gilt nur für Excel 2007.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Eine Farbverlauffarbe. |
| Grad | double | Der Grad des Farbverlaufs. Kann ein Wert von 0.0 (dunkel) bis 1.0 (hell) sein. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


Gibt die vordefinierte Gradientfarbe für die angegebene Füllung zurück. Gilt für Excel97-2003

Siehe [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Setzt die angegebene Füllung auf einen voreingestellten Farbverlauf. Gilt nur für Excel 97-2003

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Vorgabefarbtyp |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


Setzt vordefinierte Themen‑Gradientenfüllung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). Der voreingestellte Verlaufstyp. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Der Theme-Farbtyp. |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Eine Farbverlauffarbe. |
| color2 | [Color](../../com.aspose.cells/color) | Zwei Gradientfarben. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Eine Farbverlauffarbe. |
| transparency1 | double | Der Transparenzgrad von color1 als Wert von 0.0 (undurchsichtig) bis 1.0 (klar). |
| color2 | [Color](../../com.aspose.cells/color) | Zwei Gradientfarben. |
| transparency2 | double | Der Transparenzgrad von color2 als Wert von 0.0 (undurchsichtig) bis 1.0 (klar). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradient-Schattierungsstil. |
| Variante | int | Die Gradientvariante. Kann ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fülleffekte. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

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

