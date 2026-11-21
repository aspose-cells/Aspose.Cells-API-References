---
title: "GradientFill"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar gradientfyllningen."
type: docs
url: /sv/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

Representerar gradientfyllningen.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | Vinkeln för linjär fyllning. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Hämtar gradientens riktningstyp. |
| [getFillType()](#getFillType--) | Hämtar gradientens fyllningstyp. |
| [getGradientColor1()](#getGradientColor1--) | Hämtar gradientfärg 1. |
| [getGradientColor2()](#getGradientColor2--) | Hämtar gradientfärg 2. |
| [getGradientColorType()](#getGradientColorType--) | Hämtar gradientfärgens typ. |
| [getGradientDegree()](#getGradientDegree--) | Hämtar gradientens grad. |
| [getGradientStops()](#getGradientStops--) | Representerar samlingen av gradientstopp. |
| [getGradientStyle()](#getGradientStyle--) | Hämtar gradientens stiltyp. |
| [getPresetColor()](#getPresetColor--) | Returnerar gradientens förinställda färg för den angivna fyllningen. |
| [getVariant()](#getVariant--) | Hämtar variant. |
| [hashCode()](#hashCode--) | Hämtar hashkoden. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | Vinkeln för linjär fyllning. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | Ställ in gradientens fyllningstyp och riktning. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Anger den angivna fyllningen till en enfärgsgradient. |
| [setPresetColor(int value)](#setPresetColor-int-) | Returnerar gradientens förinställda färg för den angivna fyllningen. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Ställer in den angivna fyllningen till en förinställd färggradient. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | Ställer in förinställd temagradientfyllning. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Ställer in den angivna fyllningen till en tvåfärgsgradient. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Ställer in den angivna fyllningen till en tvåfärgsgradient. |
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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


Vinkeln för linjär fyllning.

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


Hämtar gradientens riktningstyp.

Se [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Hämtar gradientens fyllningstyp.

Se [GradientFillType](../../com.aspose.cells/gradientfilltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Hämtar gradientfärg 1. Gäller för Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Hämtar gradientfärg 2. Gäller för Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Hämtar gradientfärgstyp. Gäller för Excel97-2003

Se [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Hämtar gradientgrad. Gäller för Excel97-2003

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


Representerar samlingen av gradientstopp.

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Hämtar gradientstilstyp. Gäller för Excel97-2003

Se [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Returnerar den förinställda gradientfärgen för den angivna fyllningen. Gäller för Excel97-2003

Se [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


Hämtar variant. Gäller för Excel97-2003

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Hämtar hashkoden.

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


Vinkeln för linjär fyllning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


Ställ in gradientens fyllningstyp och riktning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). Gradientfyllningstyp. |
| vinkel | double | Vinkeln. Gäller endast för GradientFillType.Linear. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). Riktningstypen. Gäller endast för GradientFillType.Radial och GradientFillType.Rectangle. |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast för Excel 2007.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | En gradientfärg. |
| grad | double | Gradientgraden. Kan vara ett värde från 0.0 (mörk) till 1.0 (ljus). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


Returnerar den förinställda gradientfärgen för den angivna fyllningen. Gäller för Excel97-2003

Se [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Ställer in den angivna fyllningen till en förinställd färggradient. Gäller endast för Excel 97-2003

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Förinställd färgtyp |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


Ställer in förinställd temagradientfyllning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). Den förinställda gradienttypen. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Temafärgstypen. |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | En gradientfärg. |
| color2 | [Color](../../com.aspose.cells/color) | Två gradientfärger. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | En gradientfärg. |
| transparency1 | double | Grad av transparens för färg1 som ett värde från 0,0 (opakt) till 1,0 (genomskinligt). |
| color2 | [Color](../../com.aspose.cells/color) | Två gradientfärger. |
| transparency2 | double | Grad av transparens för färg2 som ett värde från 0,0 (opakt) till 1,0 (genomskinligt). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Gradientskuggningsstil. |
| variant | int | Gradientvarianten. Kan vara ett värde från 1 till 4, vilket motsvarar en av de fyra varianterna på fliken Gradient i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2. |

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

