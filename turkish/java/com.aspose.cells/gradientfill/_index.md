---
title: "GradientFill"
second_title: "Aspose.Cells for Java API Referansı"
description: "Degrade dolgu tipini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

Degrade dolgu tipini temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | Doğrusal doldurmanın açısı. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Gradyan yön türünü alır. |
| [getFillType()](#getFillType--) | Gradyan doldurma türünü alır. |
| [getGradientColor1()](#getGradientColor1--) | Gradient renk 1'i alır. |
| [getGradientColor2()](#getGradientColor2--) | Gradient renk 2'i alır. |
| [getGradientColorType()](#getGradientColorType--) | Gradient renk tipini alır. |
| [getGradientDegree()](#getGradientDegree--) | Gradient derecesini alır. |
| [getGradientStops()](#getGradientStops--) | Gradient durak koleksiyonunu temsil eder. |
| [getGradientStyle()](#getGradientStyle--) | Gradient stil tipini alır. |
| [getPresetColor()](#getPresetColor--) | Belirtilen dolgu için geçiş ön ayar rengini döndürür. |
| [getVariant()](#getVariant--) | Varyantı alır. |
| [hashCode()](#hashCode--) | Karma kodunu alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | Doğrusal doldurmanın açısı. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | Gradient doldurma tipini ve yönünü ayarla. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | Belirtilen dolguyu tek renkli bir degradeye ayarlar. |
| [setPresetColor(int value)](#setPresetColor-int-) | Belirtilen dolgu için geçiş ön ayar rengini döndürür. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | Belirtilen dolguyu ön ayarlı renk geçişine ayarlar. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | Önceden ayarlanmış tema gradient doldurmasını ayarlar. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | Belirtilen doldurmayı iki renkli bir degradeye ayarlar. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | Belirtilen doldurmayı iki renkli bir degradeye ayarlar. |
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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


Doğrusal doldurmanın açısı.

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


Gradyan yön türünü alır.

Bak [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


Gradyan doldurma türünü alır.

Bak [GradientFillType](../../com.aspose.cells/gradientfilltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


Gradient renk 1'i alır. Excel97-2003 için geçerlidir

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


Gradient renk 2'i alır. Excel97-2003 için geçerlidir

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


Gradient renk tipini alır. Excel97-2003 için geçerlidir

Bakın [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


Gradient derecesini alır. Excel97-2003 için geçerlidir

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


Gradient durak koleksiyonunu temsil eder.

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


Gradient stil tipini alır. Excel97-2003 için geçerlidir

Bak [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


Belirtilen doldurma için gradient önceden ayarlanmış rengi döndürür. Excel97-2003 için geçerlidir

Bakın [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


Varyantı alır. Excel97-2003 için geçerlidir

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


Karma kodunu alır.

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


Doğrusal doldurmanın açısı.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


Gradient doldurma tipini ve yönünü ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). Gradient doldurma tipi. |
| açı | double | Açı. Yalnızca GradientFillType.Linear için geçerlidir. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). Yön tipi. Yalnızca GradientFillType.Radial ve GradientFillType.Rectangle için geçerlidir. |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


Belirtilen doldurmayı tek renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| derece | double | Degrade derecesi. 0.0 (karanlık) ile 1.0 (açık) arasında bir değer olabilir. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


Belirtilen doldurma için gradient önceden ayarlanmış rengi döndürür. Excel97-2003 için geçerlidir

Bakın [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


Belirtilen doldurmayı önceden ayarlanmış renkli gradient olarak ayarlar. Yalnızca Excel 97-2003 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). Önceden tanımlı renk tipi |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


Önceden ayarlanmış tema gradient doldurmasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). Önceden ayarlanmış gradient tipi. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). Tema renk türü. |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


Belirtilen doldurmayı iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| color2 | [Color](../../com.aspose.cells/color) | İki degrade rengi. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


Belirtilen doldurmayı iki renkli bir degradeye ayarlar. Yalnızca Excel 2007 için geçerlidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | Tek bir degrade rengi. |
| transparency1 | double | color1'in şeffaflık derecesi, 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak. |
| color2 | [Color](../../com.aspose.cells/color) | İki degrade rengi. |
| transparency2 | double | color2'nin şeffaflık derecesi, 0.0 (opak) ile 1.0 (şeffaf) arasında bir değer olarak. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). Degrade gölgelendirme stili. |
| varyant | int | Gradient varyantı. 1 ile 4 arasında bir değer olabilir ve Doldurma Efektleri iletişim kutusundaki Gradient sekmesindeki dört varyanttan birine karşılık gelir. Stil GradientStyle.FromCenter ise, Variant argümanı yalnızca 1 veya 2 olabilir. |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

