---
title: "LineFormat"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع إعدادات الخط."
type: docs
url: /ar/java/com.aspose.cells/lineformat/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FillFormat](../../com.aspose.cells/fillformat)
```
public class LineFormat extends FillFormat
```

يمثل جميع إعدادات الخط.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         Shape shape = shapes.addRectangle(1, 0, 1, 0, 50, 100);
         LineFormat lineFmt = shape.getLine();
 
         //do your business
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | يحدد ما إذا كانت هذه الحالة لها نفس القيمة كما في كائن [LineFormat](../../com.aspose.cells/lineformat) المحدد الآخر. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--) | يحصل على نوع طول السهم الابتدائي للخط. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--) | يحصل على نوع السهم الابتدائي للخط. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--) | يحصل على نوع عرض السهم الابتدائي للخط. |
| [getCapType()](#getCapType--) | يحدد نهايات القُبُعات. |
| [getClass()](#getClass--) |  |
| [getCompoundType()](#getCompoundType--) | يحدد نوع التركيب للخط. |
| [getDashStyle()](#getDashStyle--) | يحدد نوع التقطيع للخط. |
| [getEndArrowheadLength()](#getEndArrowheadLength--) | يحصل على نوع طول السهم النهائي للخط. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--) | يحصل على نوع السهم النهائي للخط. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--) | يحصل على نوع عرض السهم النهائي للخط. |
| [getFillType()](#getFillType--) | يحصل على نوع التعبئة |
| [getGradientColor1()](#getGradientColor1--) | يعيد لون التدرج 1 للتعبئة المحددة. |
| [getGradientColor2()](#getGradientColor2--) | يعيد لون التدرج 2 للتعبئة المحددة. |
| [getGradientColorType()](#getGradientColorType--) | يعيد نوع لون التدرج للتعبئة المحددة. |
| [getGradientDegree()](#getGradientDegree--) | يعيد درجة التدرج للتعبئة المحددة. |
| [getGradientFill()](#getGradientFill--) | يحصل على كائن [getGradientFill()](../../com.aspose.cells/fillformat\#getGradientFill--). |
| [getGradientStyle()](#getGradientStyle--) | يعيد نمط التدرج للتعبئة المحددة. |
| [getGradientVariant()](#getGradientVariant--) | يعيد متغير التدرج للتعبئة المحددة. |
| [getImageData()](#getImageData--) | يحصل على بيانات الصورة. |
| [getJoinType()](#getJoinType--) | يحدد نوع وصل الخط. |
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
| [getWeight()](#getWeight--) | يحصل على وزن الخط بوحدة النقاط. |
| [hashCode()](#hashCode--) | يحصل على رمز التجزئة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBeginArrowheadLength(int value)](#setBeginArrowheadLength-int-) | يضبط نوع طول السهم الابتدائي للخط. |
| [setBeginArrowheadStyle(int value)](#setBeginArrowheadStyle-int-) | يضبط نوع السهم الابتدائي للخط. |
| [setBeginArrowheadWidth(int value)](#setBeginArrowheadWidth-int-) | يضبط نوع عرض السهم الابتدائي للخط. |
| [setCapType(int value)](#setCapType-int-) | يحدد نهايات القُبُعات. |
| [setCompoundType(int value)](#setCompoundType-int-) | يحدد نوع التركيب للخط. |
| [setDashStyle(int value)](#setDashStyle-int-) | يحدد نوع التقطيع للخط. |
| [setEndArrowheadLength(int value)](#setEndArrowheadLength-int-) | يضبط نوع طول السهم النهائي للخط. |
| [setEndArrowheadStyle(int value)](#setEndArrowheadStyle-int-) | يضبط نوع السهم النهائي للخط. |
| [setEndArrowheadWidth(int value)](#setEndArrowheadWidth-int-) | يضبط نوع عرض السهم النهائي للخط. |
| [setFillType(int value)](#setFillType-int-) | يضبط نوع التعبئة |
| [setImageData(byte[] value)](#setImageData-byte---) | يضبط بيانات الصورة. |
| [setJoinType(int value)](#setJoinType-int-) | يحدد نوع وصل الخط. |
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
| [setWeight(double value)](#setWeight-double-) | يضبط وزن الخط بوحدة النقاط. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يحدد ما إذا كانت هذه الحالة لها نفس القيمة كما في كائن [LineFormat](../../com.aspose.cells/lineformat) المحدد الآخر.

**Example**

```
         //You have to make sure that the index value in this line of code exists
         LineFormat obj = workbook.getWorksheets().get(0).getShapes().get(0).getLine();
         if (lineFmt.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | الكائن [LineFormat](../../com.aspose.cells/lineformat) للمقارنة مع هذا الكائن. |

**Returns:**
boolean - true إذا كانت قيمة المعامل obj هي نفسها قيمة هذا الكائن؛ وإلا false. إذا كان obj يساوي null، تُعيد هذه الطريقة false.
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```
public int getBeginArrowheadLength()
```


يحصل على نوع طول السهم الابتدائي للخط.

انظر [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Example**

```
         lineFmt.setBeginArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getBeginArrowheadStyle() {#getBeginArrowheadStyle--}
```
public int getBeginArrowheadStyle()
```


يحصل على نوع السهم الابتدائي للخط.

انظر [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Example**

```
         lineFmt.setBeginArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getBeginArrowheadWidth() {#getBeginArrowheadWidth--}
```
public int getBeginArrowheadWidth()
```


يحصل على نوع عرض السهم الابتدائي للخط.

انظر [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Example**

```
         lineFmt.setBeginArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
### getCapType() {#getCapType--}
```
public int getCapType()
```


يحدد نهايات القُبُعات.

انظر [LineCapType](../../com.aspose.cells/linecaptype).

**Example**

```
         lineFmt.setCapType(LineCapType.FLAT);
```

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCompoundType() {#getCompoundType--}
```
public int getCompoundType()
```


يحدد نوع التركيب للخط.

انظر [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Example**

```
         lineFmt.setCompoundType(MsoLineStyle.SINGLE);
```

**Returns:**
int
### getDashStyle() {#getDashStyle--}
```
public int getDashStyle()
```


يحدد نوع التقطيع للخط.

انظر [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Example**

```
         lineFmt.setDashStyle(MsoLineDashStyle.SOLID);
```

**Returns:**
int
### getEndArrowheadLength() {#getEndArrowheadLength--}
```
public int getEndArrowheadLength()
```


يحصل على نوع طول السهم النهائي للخط.

انظر [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Example**

```
         lineFmt.setEndArrowheadLength(MsoArrowheadLength.LONG);
```

**Returns:**
int
### getEndArrowheadStyle() {#getEndArrowheadStyle--}
```
public int getEndArrowheadStyle()
```


يحصل على نوع السهم النهائي للخط.

انظر [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Example**

```
         lineFmt.setEndArrowheadStyle(MsoArrowheadStyle.ARROW_OPEN);
```

**Returns:**
int
### getEndArrowheadWidth() {#getEndArrowheadWidth--}
```
public int getEndArrowheadWidth()
```


يحصل على نوع عرض السهم النهائي للخط.

انظر [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Example**

```
         lineFmt.setEndArrowheadWidth(MsoArrowheadWidth.MEDIUM);
```

**Returns:**
int
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
### getJoinType() {#getJoinType--}
```
public int getJoinType()
```


يحدد نوع وصل الخط.

انظر [LineJoinType](../../com.aspose.cells/linejointype).

**Example**

```
         lineFmt.setJoinType(LineJoinType.ROUND);
```

**Returns:**
int
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
### getWeight() {#getWeight--}
```
public double getWeight()
```


يحصل على وزن الخط بوحدة النقاط.

**Example**

```
         lineFmt.setWeight(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```


يحصل على رمز التجزئة.

**Example**

```
         int hashCode = lineFmt.hashCode();
```

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




### setBeginArrowheadLength(int value) {#setBeginArrowheadLength-int-}
```
public void setBeginArrowheadLength(int value)
```


يضبط نوع طول السهم الابتدائي للخط.

انظر [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBeginArrowheadStyle(int value) {#setBeginArrowheadStyle-int-}
```
public void setBeginArrowheadStyle(int value)
```


يضبط نوع السهم الابتدائي للخط.

انظر [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBeginArrowheadWidth(int value) {#setBeginArrowheadWidth-int-}
```
public void setBeginArrowheadWidth(int value)
```


يضبط نوع عرض السهم الابتدائي للخط.

انظر [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCapType(int value) {#setCapType-int-}
```
public void setCapType(int value)
```


يحدد نهايات القُبُعات.

انظر [LineCapType](../../com.aspose.cells/linecaptype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCompoundType(int value) {#setCompoundType-int-}
```
public void setCompoundType(int value)
```


يحدد نوع التركيب للخط.

انظر [MsoLineStyle](../../com.aspose.cells/msolinestyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDashStyle(int value) {#setDashStyle-int-}
```
public void setDashStyle(int value)
```


يحدد نوع التقطيع للخط.

انظر [MsoLineDashStyle](../../com.aspose.cells/msolinedashstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEndArrowheadLength(int value) {#setEndArrowheadLength-int-}
```
public void setEndArrowheadLength(int value)
```


يضبط نوع طول السهم النهائي للخط.

انظر [MsoArrowheadLength](../../com.aspose.cells/msoarrowheadlength).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEndArrowheadStyle(int value) {#setEndArrowheadStyle-int-}
```
public void setEndArrowheadStyle(int value)
```


يضبط نوع السهم النهائي للخط.

انظر [MsoArrowheadStyle](../../com.aspose.cells/msoarrowheadstyle).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setEndArrowheadWidth(int value) {#setEndArrowheadWidth-int-}
```
public void setEndArrowheadWidth(int value)
```


يضبط نوع عرض السهم النهائي للخط.

انظر [MsoArrowheadWidth](../../com.aspose.cells/msoarrowheadwidth).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

### setJoinType(int value) {#setJoinType-int-}
```
public void setJoinType(int value)
```


يحدد نوع وصل الخط.

انظر [LineJoinType](../../com.aspose.cells/linejointype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

### setWeight(double value) {#setWeight-double-}
```
public void setWeight(double value)
```


يضبط وزن الخط بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

