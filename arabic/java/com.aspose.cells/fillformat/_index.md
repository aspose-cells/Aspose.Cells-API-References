---
title: "FillFormat"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل تنسيق التعبئة لشكل."
type: docs
url: /ar/java/com.aspose.cells/fillformat/
---

**Inheritance:**
java.lang.Object
```
public class FillFormat
```

يغلف الكائن الذي يمثل تنسيق التعبئة لشكل.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Excel object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a sample value to "A1" cell
         worksheet.getCells().get("A1").putValue(50);
         //Adding a sample value to "A2" cell
         worksheet.getCells().get("A2").putValue(100);
         //Adding a sample value to "A3" cell
         worksheet.getCells().get("A3").putValue(150);
         //Adding a sample value to "A4" cell
         worksheet.getCells().get("A4").putValue(200);
         //Adding a sample value to "B1" cell
         worksheet.getCells().get("B1").putValue(60);
         //Adding a sample value to "B2" cell
         worksheet.getCells().get("B2").putValue(32);
         //Adding a sample value to "B3" cell
         worksheet.getCells().get("B3").putValue(50);
         //Adding a sample value to "B4" cell
         worksheet.getCells().get("B4").putValue(40);
         //Adding a sample value to "C1" cell as category data
         worksheet.getCells().get("C1").putValue("Q1");
         //Adding a sample value to "C2" cell as category data
         worksheet.getCells().get("C2").putValue("Q2");
         //Adding a sample value to "C3" cell as category data
         worksheet.getCells().get("C3").putValue("Y1");
         //Adding a sample value to "C4" cell as category data
         worksheet.getCells().get("C4").putValue("Y2");
         //Adding a chart to the worksheet
         int chartIndex = worksheet.getCharts().add(ChartType.COLUMN, 5, 0, 15, 5);
         //Accessing the instance of the newly added chart
         Chart chart = worksheet.getCharts().get(chartIndex);
         //Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
         int seriesIndex = chart.getNSeries().add("A1:B4", true);
         //Setting the data source for the category data of NSeries
         chart.getNSeries().setCategoryData("C1:C4");
         //Filling the area of the 2nd NSeries with a gradient
         chart.getNSeries().get(seriesIndex).getArea().getFillFormat().setOneColorGradient(Color.getLime(), 1, GradientStyleType.HORIZONTAL, 1);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFillType()](#getFillType--) | يحصل على نوع التعبئة |
| [getGradientColor1()](#getGradientColor1--) | يعيد لون التدرج 1 للتعبئة المحددة. |
| [getGradientColor2()](#getGradientColor2--) | يعيد لون التدرج 2 للتعبئة المحددة. |
| [getGradientColorType()](#getGradientColorType--) | يعيد نوع لون التدرج للتعبئة المحددة. |
| [getGradientDegree()](#getGradientDegree--) | يعيد درجة التدرج للتعبئة المحددة. |
| [getGradientFill()](#getGradientFill--) | يحصل على كائن [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--). |
| [getGradientStyle()](#getGradientStyle--) | يعيد نمط التدرج للتعبئة المحددة. |
| [getGradientVariant()](#getGradientVariant--) | يعيد متغير التدرج للتعبئة المحددة. |
| [getImageData()](#getImageData--) | يحصل على بيانات الصورة. |
| [getPattern()](#getPattern--) | يمثل نمط عرض المنطقة. |
| [getPatternFill()](#getPatternFill--) | يحصل على كائن [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--). |
| [getPictureFormatType()](#getPictureFormatType--) | يحصل على نوع تنسيق الصورة. |
| [getPresetColor()](#getPresetColor--) | يعيد لون التدرج المحدد مسبقًا للتعبئة المحددة. |
| [getScale()](#getScale--) | يحصل على مقياس تنسيق الصورة. |
| [getSetType()](#getSetType--) | يحصل على نوع مجموعة تنسيق التعبئة. |
| [getSolidFill()](#getSolidFill--) | يحصل على كائن [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--). |
| [getTexture()](#getTexture--) | يمثل نوع النسيج للتعبئة المحددة. |
| [getTextureFill()](#getTextureFill--) | يحصل على كائن [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--). |
| [getTransparency()](#getTransparency--) | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [getType()](#getType--) | يحصل على نوع التعبئة. |
| [hashCode()](#hashCode--) | يحصل على رمز التجزئة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFillType(int value)](#setFillType-int-) | يضبط نوع التعبئة |
| [setImageData(byte[] value)](#setImageData-byte---) | يضبط بيانات الصورة. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | يضبط التعبئة المحددة لتصبح تدرج لون واحد. |
| [setPattern(int value)](#setPattern-int-) | يمثل نمط عرض المنطقة. |
| [setPictureFormatType(int value)](#setPictureFormatType-int-) | يضبط نوع تنسيق الصورة. |
| [setPresetColorGradient(int presetColor, int style, int variant)](#setPresetColorGradient-int-int-int-) | يضبط التعبئة المحددة إلى تدرج لون مسبق. |
| [setScale(double value)](#setScale-double-) | يضبط مقياس تنسيق الصورة. |
| [setSetType(int value)](#setSetType-int-) | يحصل على نوع مجموعة تنسيق التعبئة. |
| [setTexture(int value)](#setTexture-int-) | يمثل نوع النسيج للتعبئة المحددة. |
| [setTransparency(double value)](#setTransparency-double-) | يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [setTwoColorGradient(Color color1, Color color2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-com.aspose.cells.Color-int-int-) | يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين. |
| [setTwoColorGradient(Color color1, double transparency1, Color color2, double transparency2, int style, int variant)](#setTwoColorGradient-com.aspose.cells.Color-double-com.aspose.cells.Color-double-int-int-) | يضبط التعبئة المحددة لتصبح تدرجًا لونيًا من لونين. |
| [setType(int value)](#setType-int-) | يضبط نوع التعبئة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFillType() {#getFillType--}
```
public int getFillType()
```


يحصل على نوع التعبئة

انظر [FillType](../../com.aspose.cells/filltype).

**Returns:**
int
### getGradientColor1() {#getGradientColor1--}
```
public Color getGradientColor1()
```


يعيد لون التدرج 1 للتعبئة المحددة.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColor2() {#getGradientColor2--}
```
public Color getGradientColor2()
```


يعيد لون التدرج 2 للتعبئة المحددة.

**Remarks**

فقط عندما يكون نوع لون التدرج هو GradientColorType.TwoColors، تكون هذه الخاصية ذات معنى.

**Returns:**
[Color](../../com.aspose.cells/color)
### getGradientColorType() {#getGradientColorType--}
```
public int getGradientColorType()
```


يعيد نوع لون التدرج للتعبئة المحددة.

انظر [GradientColorType](../../com.aspose.cells/gradientcolortype).

**Returns:**
int
### getGradientDegree() {#getGradientDegree--}
```
public double getGradientDegree()
```


يعيد درجة التدرج للتعبئة المحددة. ينطبق فقط على Excel 2007.

**Remarks**

يمكن أن تكون قيمة فقط من 0.0 (غامق) إلى 1.0 (فاتح).

**Returns:**
double
### getGradientFill() {#getGradientFill--}
```
public GradientFill getGradientFill()
```


يحصل على كائن [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--).

**Returns:**
[GradientFill](../../com.aspose.cells/gradientfill)
### getGradientStyle() {#getGradientStyle--}
```
public int getGradientStyle()
```


يعيد نمط التدرج للتعبئة المحددة.

انظر [GradientStyleType](../../com.aspose.cells/gradientstyletype).

**Returns:**
int
### getGradientVariant() {#getGradientVariant--}
```
public int getGradientVariant()
```


يعيد المتغير التدرجي للتعبئة المحددة. ينطبق فقط على Excel 2007.

**Remarks**

يمكن أن تكون قيمة فقط من 1 إلى 4، تمثل أحد المتغيرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان النمط هو GradientStyle.FromCenter، يمكن أن يكون معامل Variant فقط 1 أو 2.

**Returns:**
int
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


يحصل على بيانات الصورة.

**Remarks**

إذا لم يكن تنسيق التعبئة تنسيق نسيج مخصص، يعيد null.

**Returns:**
byte[]
### getPattern() {#getPattern--}
```
public int getPattern()
```


يمثل نمط عرض المنطقة.

انظر إلى [FillPattern](../../com.aspose.cells/fillpattern).

**Returns:**
int
### getPatternFill() {#getPatternFill--}
```
public PatternFill getPatternFill()
```


يحصل على كائن [getPatternFill()](../../com.aspose.cells/fillformat\#getPatternFill--).

**Returns:**
[PatternFill](../../com.aspose.cells/patternfill)
### getPictureFormatType() {#getPictureFormatType--}
```
public int getPictureFormatType()
```


يحصل على نوع تنسيق الصورة.

انظر [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Returns:**
int
### getPresetColor() {#getPresetColor--}
```
public int getPresetColor()
```


يعيد لون التدرج المحدد مسبقًا للتعبئة المحددة.

انظر [GradientPresetType](../../com.aspose.cells/gradientpresettype).

**Returns:**
int
### getScale() {#getScale--}
```
public double getScale()
```


يحصل على مقياس تنسيق الصورة.

**Returns:**
double
### getSetType() {#getSetType--}
```
public int getSetType()
```


يحصل على نوع مجموعة تنسيق التعبئة.

انظر [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية FillFormat.FillType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getSolidFill() {#getSolidFill--}
```
public SolidFill getSolidFill()
```


يحصل على كائن [getSolidFill()](../../com.aspose.cells/fillformat\#getSolidFill--).

**Returns:**
[SolidFill](../../com.aspose.cells/solidfill)
### getTexture() {#getTexture--}
```
public int getTexture()
```


يمثل نوع النسيج للتعبئة المحددة.

انظر [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTextureFill() {#getTextureFill--}
```
public TextureFill getTextureFill()
```


يحصل على كائن [getTextureFill()](../../com.aspose.cells/fillformat\#getTextureFill--).

**Returns:**
[TextureFill](../../com.aspose.cells/texturefill)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع التعبئة.

انظر [FillType](../../com.aspose.cells/filltype).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية FillFormat.FillType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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




### setFillType(int value) {#setFillType-int-}
```
public void setFillType(int value)
```


يضبط نوع التعبئة

انظر [FillType](../../com.aspose.cells/filltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


يضبط بيانات الصورة.

**Remarks**

إذا لم يكن تنسيق التعبئة تنسيق نسيج مخصص، يعيد null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

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

### setPattern(int value) {#setPattern-int-}
```
public void setPattern(int value)
```


يمثل نمط عرض المنطقة.

انظر إلى [FillPattern](../../com.aspose.cells/fillpattern).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPictureFormatType(int value) {#setPictureFormatType-int-}
```
public void setPictureFormatType(int value)
```


يضبط نوع تنسيق الصورة.

انظر [FillPictureType](../../com.aspose.cells/fillpicturetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPresetColorGradient(int presetColor, int style, int variant) {#setPresetColorGradient-int-int-int-}
```
public void setPresetColorGradient(int presetColor, int style, int variant)
```


يضبط التعبئة المحددة لتصبح تدرجًا لونيًا مسبق الإعداد. ينطبق فقط على Excel 2007.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| presetColor | int | [GradientPresetType](../../com.aspose.cells/gradientpresettype). نوع اللون المسبق |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). نمط تظليل التدرج. |
| متغيّر | int | متغيّر التدرج. يمكن أن تكون قيمة من 1 إلى 4، تتطابق مع أحد المتغيّرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان النمط هو GradientStyle.FromCenter، لا يمكن أن يكون معامل Variant سوى 1 أو 2. |

### setScale(double value) {#setScale-double-}
```
public void setScale(double value)
```


يضبط مقياس تنسيق الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setSetType(int value) {#setSetType-int-}
```
public void setSetType(int value)
```


يحصل على نوع مجموعة تنسيق التعبئة.

انظر [FormatSetType](../../com.aspose.cells/formatsettype).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية FillFormat.FillType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTexture(int value) {#setTexture-int-}
```
public void setTexture(int value)
```


يمثل نوع النسيج للتعبئة المحددة.

انظر [TextureType](../../com.aspose.cells/texturetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


يرجع أو يضبط درجة شفافية المنطقة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يضبط نوع التعبئة.

انظر [FillType](../../com.aspose.cells/filltype).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام خاصية FillFormat.FillType. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2016. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

