---
title: "MsoFillFormat"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل تنسيق التعبئة لشكل."
type: docs
url: /ar/java/com.aspose.cells/msofillformat/
---

**Inheritance:**
java.lang.Object
```
public class MsoFillFormat
```

يمثل تنسيق التعبئة لشكل.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBackColor()](#getBackColor--) | يحصل على لون خلفية الملف. |
| [getClass()](#getClass--) |  |
| [getForeColor()](#getForeColor--) | يحصل على لون مقدمة التعبئة. |
| [getImageData()](#getImageData--) | يحصل على بيانات تعبئة النسيج والصورة. |
| [getTexture()](#getTexture--) | يحصل على نوع تعبئة النسيج. |
| [getTransparency()](#getTransparency--) | يعيد أو يضبط درجة شفافية التعبئة المحددة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [hashCode()](#hashCode--) |  |
| [isVisible()](#isVisible--) | يشير إلى ما إذا كان هناك تعبئة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackColor(Color value)](#setBackColor-com.aspose.cells.Color-) | يضبط لون خلفية الملف. |
| [setForeColor(Color value)](#setForeColor-com.aspose.cells.Color-) | يضبط لون مقدمة التعبئة. |
| [setImageData(byte[] value)](#setImageData-byte---) | يضبط بيانات تعبئة النسيج والصورة. |
| [setOneColorGradient(Color color, double degree, int style, int variant)](#setOneColorGradient-com.aspose.cells.Color-double-int-int-) | يضبط التعبئة المحددة لتصبح تدرج لون واحد. |
| [setTransparency(double value)](#setTransparency-double-) | يعيد أو يضبط درجة شفافية التعبئة المحددة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف). |
| [setVisible(boolean value)](#setVisible-boolean-) | يشير إلى ما إذا كان هناك تعبئة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getBackColor() {#getBackColor--}
```
public Color getBackColor()
```


يحصل على لون خلفية الملف.

**Returns:**
[Color](../../com.aspose.cells/color)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getForeColor() {#getForeColor--}
```
public Color getForeColor()
```


يحصل على لون مقدمة التعبئة.

**Returns:**
[Color](../../com.aspose.cells/color)
### getImageData() {#getImageData--}
```
public byte[] getImageData()
```


يحصل على بيانات تعبئة النسيج والصورة.

**Returns:**
byte[]
### getTexture() {#getTexture--}
```
public int getTexture()
```


يحصل على نوع تعبئة النسيج.

انظر [TextureType](../../com.aspose.cells/texturetype).

**Returns:**
int
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


يعيد أو يضبط درجة شفافية التعبئة المحددة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Returns:**
double
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


يشير إلى ما إذا كان هناك تعبئة.

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




### setBackColor(Color value) {#setBackColor-com.aspose.cells.Color-}
```
public void setBackColor(Color value)
```


يضبط لون خلفية الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setForeColor(Color value) {#setForeColor-com.aspose.cells.Color-}
```
public void setForeColor(Color value)
```


يضبط لون مقدمة التعبئة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setImageData(byte[] value) {#setImageData-byte---}
```
public void setImageData(byte[] value)
```


يضبط بيانات تعبئة النسيج والصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setOneColorGradient(Color color, double degree, int style, int variant) {#setOneColorGradient-com.aspose.cells.Color-double-int-int-}
```
public void setOneColorGradient(Color color, double degree, int style, int variant)
```


يضبط التعبئة المحددة لتصبح تدرج لون واحد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| color | [Color](../../com.aspose.cells/color) | لون تدرج واحد. |
| درجة | double | درجة التدرج. يمكن أن تكون قيمة من 0.0 (داكن) إلى 1.0 (فاتح). |
| style | int | [GradientStyleType](../../com.aspose.cells/gradientstyletype). نمط تظليل التدرج. |
| متغيّر | int | متغيّر التدرج. يمكن أن تكون قيمة من 1 إلى 4، تتطابق مع أحد المتغيّرات الأربعة في علامة تبويب Gradient في مربع حوار Fill Effects. إذا كان النمط هو GradientStyle.FromCenter، لا يمكن أن يكون معامل Variant سوى 1 أو 2. |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


يعيد أو يضبط درجة شفافية التعبئة المحددة كقيمة من 0.0 (معتم) إلى 1.0 (شفاف).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يشير إلى ما إذا كان هناك تعبئة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

