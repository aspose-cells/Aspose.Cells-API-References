---
title: "GradientFill"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل تعبئة التدرج."
type: docs
url: /ar/java/com.aspose.cells/gradientfill/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Fill](../../com.aspose.cells/fill)
```
public class GradientFill extends Fill
```

يمثل تعبئة التدرج.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | / |
| [getAngle()](#getAngle--) | زاوية التعبئة الخطية. |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | يحصل على نوع اتجاه التدرج. |
| [getFillType()](#getFillType--) | يحصل على نوع تعبئة التدرج. |
| [getGradientColor1()](#getGradientColor1--) | يحصل على لون التدرج 1. |
| [getGradientColor2()](#getGradientColor2--) | يحصل على لون التدرج 2. |
| [getGradientColorType()](#getGradientColorType--) | يحصل على نوع لون التدرج. |
| [getGradientDegree()](#getGradientDegree--) | يحصل على درجة التدرج. |
| [getGradientStops()](#getGradientStops--) | يمثل مجموعة نقاط التدرج. |
| [getGradientStyle()](#getGradientStyle--) | يحصل على نوع نمط التدرج. |
| [getPresetColor()](#getPresetColor--) | يعيد لون التدرج المحدد مسبقًا للتعبئة المحددة. |
| [getVariant()](#getVariant--) | يحصل على المتغير. |
| [hashCode()](#hashCode--) | يحصل على رمز التجزئة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAngle(float value)](#setAngle-float-) | زاوية التعبئة الخطية. |
| [setGradient(int type, double angle, int direction)](#setGradient-int-double-int-) | عيّن نوع تعبئة التدرج والاتجاه. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | يضبط التعبئة المحددة لتصبح تدرج لون واحد. |
| [setPresetColor(int value)](#setPresetColor-int-) | يعيد لون التدرج المحدد مسبقًا للتعبئة المحددة. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | يضبط التعبئة المحددة إلى تدرج لون مسبق. |
| [setPresetThemeGradient(int gradientType, int themeColorType)](#setPresetThemeGradient-int-int-) | يضبط تعبئة التدرج للموضوع المحدد مسبقًا. |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين. |
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
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getAngle() {#getAngle--}
```
public float getAngle()
```


زاوية التعبئة الخطية.

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


يحصل على نوع اتجاه التدرج.

انظر [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype).

**Returns:**
int
### getFillType() {#getFillType--}
```
public int getFillType()
```


يحصل على نوع تعبئة التدرج.

انظر [GradientFillType](../../com.aspose.cells/gradientfilltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


يحصل على لون التدرج 1. ينطبق على Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


يحصل على لون التدرج 2. ينطبق على Excel97-2003

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


يحصل على نوع لون التدرج. ينطبق على Excel97-2003

انظر [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


يحصل على درجة التدرج. ينطبق على Excel97-2003

**Returns:**
double
### getGradientStops() {#getGradientStops--}
```
public GradientStopCollection getGradientStops()
```


يمثل مجموعة نقاط التدرج.

**Returns:**
[GradientStopCollection](../../com.aspose.cells/gradientstopcollection)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


يحصل على نوع نمط التدرج. ينطبق على Excel97-2003

انظر [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


يعيد لون التدرج المحدد مسبقًا للتعبئة المحددة. ينطبق على Excel97-2003

انظر [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getVariant() {#getVariant--}
```
public int getVariant()
```


يحصل على المتغير. ينطبق على Excel97-2003

**Returns:**
int
### hashCode() {#hashCode--}
```
public int hashCode()
```


يحصل على رمز التجزئة.

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


زاوية التعبئة الخطية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setGradient(int type, double angle, int direction) {#setGradient-int-double-int-}
```
public void setGradient(int type, double angle, int direction)
```


عيّن نوع تعبئة التدرج والاتجاه.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [GradientFillType](../../com.aspose.cells/gradientfilltype). نوع تعبئة التدرج. |
| زاوية | double | الزاوية. ينطبق فقط على GradientFillType.Linear. |
| direction | int | [GradientDirectionType](../../com.aspose.cells/gradientdirectiontype). نوع الاتجاه. ينطبق فقط على GradientFillType.Radial و GradientFillType.Rectangle. |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لون واحد. ينطبق فقط على Excel 2007.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | لون تدرج واحد. |
| درجة | double | درجة التدرج. يمكن أن تكون قيمة من 0.0 (داكن) إلى 1.0 (فاتح). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). نمط تظليل التدرج. |
| متغيّر | int | متغيّر التدرج. يمكن أن تكون قيمة من 1 إلى 4، تتطابق مع أحد المتغيّرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان النمط هو GradientStyle.FromCenter، لا يمكن أن يكون معامل Variant سوى 1 أو 2. |

### setPresetColor(int value) {#setPresetColor-int-}
```
public void setPresetColor(int value)
```


يعيد لون التدرج المحدد مسبقًا للتعبئة المحددة. ينطبق على Excel97-2003

انظر [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


يضبط التعبئة المحددة إلى تدرج لون محدد مسبقًا. ينطبق فقط على Excel 97-2003

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). نوع اللون المسبق |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). نمط تظليل التدرج. |
| متغيّر | int | متغيّر التدرج. يمكن أن تكون قيمة من 1 إلى 4، تتطابق مع أحد المتغيّرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان النمط هو GradientStyle.FromCenter، لا يمكن أن يكون معامل Variant سوى 1 أو 2. |

### setPresetThemeGradient(int gradientType, int themeColorType) {#setPresetThemeGradient-int-int-}
```
public void setPresetThemeGradient(int gradientType, int themeColorType)
```


يضبط تعبئة التدرج للموضوع المحدد مسبقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| gradientType | int | [PresetThemeGradientType](../../com.aspose.cells/presetthemegradienttype). نوع التدرج المحدد مسبقًا. |
| themeColorType | int | [ThemeColorType](../../com.aspose.cells/themecolortype). نوع لون السمة. |

### setTwoColorGradient(Color color1, Color color2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-}
```
public void setTwoColorGradient(Color color1, Color color2, int style, int variant)
```


يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين. ينطبق فقط على Excel 2007.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | لون تدرج واحد. |
| color2 | [Color](../../com.aspose.cells/color) | لونان متدرجان. |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). نمط تظليل التدرج. |
| متغيّر | int | متغيّر التدرج. يمكن أن تكون قيمة من 1 إلى 4، تتطابق مع أحد المتغيّرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان النمط هو GradientStyle.FromCenter، لا يمكن أن يكون معامل Variant سوى 1 أو 2. |

### setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant) {#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-}
```
public void setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)
```


يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين. ينطبق فقط على Excel 2007.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| color1 | [Color](../../com.aspose.cells/color) | لون تدرج واحد. |
| transparency1 | double | درجة شفافية اللون1 كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| color2 | [Color](../../com.aspose.cells/color) | لونان متدرجان. |
| transparency2 | double | درجة شفافية اللون2 كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). نمط تظليل التدرج. |
| متغيّر | int | متغيّر التدرج. يمكن أن تكون قيمة من 1 إلى 4، تتطابق مع أحد المتغيّرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان النمط هو GradientStyle.FromCenter، لا يمكن أن يكون معامل Variant سوى 1 أو 2. |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

