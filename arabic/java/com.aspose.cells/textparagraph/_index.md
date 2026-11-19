---
title: "TextParagraph"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل إعداد الفقرة النصية."
type: docs
url: /ar/java/com.aspose.cells/textparagraph/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.FontSetting](../../com.aspose.cells/fontsetting)
```
public class TextParagraph extends FontSetting
```

يمثل إعداد الفقرة النصية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlignmentType()](#getAlignmentType--) | يحصل على نوع محاذاة النص الأفقية للفقرة. |
| [getBullet()](#getBullet--) | يحصل على العلامة النقطية. |
| [getChildren()](#getChildren--) | يحصل على جميع مقاطع النص في هذه الفقرة. |
| [getClass()](#getClass--) |  |
| [getDefaultTabSize()](#getDefaultTabSize--) | يحصل على الحجم الافتراضي لحرف الجدولة داخل هذه الفقرة. |
| [getFirstLineIndent()](#getFirstLineIndent--) | يحدد حجم المسافة البادئة التي سيتم تطبيقها على السطر الأول من النص في الفقرة. |
| [getFont()](#getFont--) | يرجع الخط لهذا الكائن. |
| [getFontAlignType()](#getFontAlignType--) | يحدد موضع الكلمات الفعلية عمودياً على سطر النص. |
| [getLeftMargin()](#getLeftMargin--) | يحدد الهامش الأيسر للفقرة. |
| [getLength()](#getLength--) | يسترجع طول الأحرف. |
| [getLineSpace()](#getLineSpace--) | يحصل على مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة. |
| [getLineSpaceSizeType()](#getLineSpaceSizeType--) | يحصل على مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة. |
| [getRightMargin()](#getRightMargin--) | يحدد الهامش الأيمن للفقرة. |
| [getSpaceAfter()](#getSpaceAfter--) | يحصل على مقدار المسافة البيضاء العمودية التي ستكون موجودة بعد الفقرة. |
| [getSpaceAfterSizeType()](#getSpaceAfterSizeType--) | يحصل على مقدار المسافة البيضاء العمودية التي ستكون موجودة بعد الفقرة. |
| [getSpaceBefore()](#getSpaceBefore--) | يحصل على مقدار المسافة البيضاء العمودية التي ستكون موجودة قبل الفقرة. |
| [getSpaceBeforeSizeType()](#getSpaceBeforeSizeType--) | يحصل على مقدار المسافة البيضاء العمودية التي ستكون موجودة قبل الفقرة. |
| [getStartIndex()](#getStartIndex--) | يسترجع الفهرس الابتدائي للأحرف. |
| [getStops()](#getStops--) | يحصل على قائمة نقاط التبويب. |
| [getTextOptions()](#getTextOptions--) | يرجع خيارات النص. |
| [getType()](#getType--) | يحصل على نوع عقدة النص. |
| [hashCode()](#hashCode--) |  |
| [isEastAsianLineBreak()](#isEastAsianLineBreak--) | يحدد ما إذا كان يمكن كسر كلمة شرق آسيوية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة. |
| [isHangingPunctuation()](#isHangingPunctuation--) | يحدد ما إذا كان يجب وضع علامات الترقيم بقوة على سطر النص أو وضعها على سطر نص مختلف. |
| [isLatinLineBreak()](#isLatinLineBreak--) | يحدد ما إذا كان يمكن كسر كلمة لاتينية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | يضبط نوع محاذاة النص الأفقية للفقرة. |
| [setDefaultTabSize(double value)](#setDefaultTabSize-double-) | يضبط الحجم الافتراضي لحرف الجدولة داخل هذه الفقرة. |
| [setEastAsianLineBreak(boolean value)](#setEastAsianLineBreak-boolean-) | يحدد ما إذا كان يمكن كسر كلمة شرق آسيوية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة. |
| [setFirstLineIndent(double value)](#setFirstLineIndent-double-) | يحدد حجم المسافة البادئة التي سيتم تطبيقها على السطر الأول من النص في الفقرة. |
| [setFontAlignType(int value)](#setFontAlignType-int-) | يحدد موضع الكلمات الفعلية عمودياً على سطر النص. |
| [setHangingPunctuation(boolean value)](#setHangingPunctuation-boolean-) | يحدد ما إذا كان يجب وضع علامات الترقيم بقوة على سطر النص أو وضعها على سطر نص مختلف. |
| [setLatinLineBreak(boolean value)](#setLatinLineBreak-boolean-) | يحدد ما إذا كان يمكن كسر كلمة لاتينية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة. |
| [setLeftMargin(double value)](#setLeftMargin-double-) | يحدد الهامش الأيسر للفقرة. |
| [setLineSpace(double value)](#setLineSpace-double-) | يضبط مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة. |
| [setLineSpaceSizeType(int value)](#setLineSpaceSizeType-int-) | يضبط مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة. |
| [setRightMargin(double value)](#setRightMargin-double-) | يحدد الهامش الأيمن للفقرة. |
| [setSpaceAfter(double value)](#setSpaceAfter-double-) | يضبط مقدار المسافة البيضاء العمودية التي ستكون موجودة بعد الفقرة. |
| [setSpaceAfterSizeType(int value)](#setSpaceAfterSizeType-int-) | يضبط مقدار المسافة البيضاء العمودية التي ستكون موجودة بعد الفقرة. |
| [setSpaceBefore(double value)](#setSpaceBefore-double-) | يضبط مقدار المسافة البيضاء العمودية التي ستكون موجودة قبل الفقرة. |
| [setSpaceBeforeSizeType(int value)](#setSpaceBeforeSizeType-int-) | يضبط مقدار المسافة البيضاء العمودية التي ستكون موجودة قبل الفقرة. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | يضبط نمط WordArt المحدد مسبقًا. |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```


يحصل على نوع محاذاة النص الأفقية للفقرة.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Returns:**
int
### getBullet() {#getBullet--}
```
public Bullet getBullet()
```


يحصل على العلامة النقطية.

**Returns:**
[Bullet](../../com.aspose.cells/bullet)
### getChildren() {#getChildren--}
```
public FontSetting[] getChildren()
```


يحصل على جميع مقاطع النص في هذه الفقرة. إذا كانت هذه الفقرة فارغة، يرجع الفقرة نفسها.

**Returns:**
com.aspose.cells.FontSetting[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultTabSize() {#getDefaultTabSize--}
```
public double getDefaultTabSize()
```


يحصل على الحجم الافتراضي لحرف الجدولة داخل هذه الفقرة.

**Returns:**
double
### getFirstLineIndent() {#getFirstLineIndent--}
```
public double getFirstLineIndent()
```


يحدد حجم المسافة البادئة التي سيتم تطبيقها على السطر الأول من النص في الفقرة.

**Returns:**
double
### getFont() {#getFont--}
```
public Font getFont()
```


يرجع الخط لهذا الكائن.

**Returns:**
[Font](../../com.aspose.cells/font)
### getFontAlignType() {#getFontAlignType--}
```
public int getFontAlignType()
```


يحدد موضع الكلمات الفعلية عمودياً على سطر النص. هذا يتعلق بالموضع العمودي للأحرف بالنسبة لخط الأساس.

انظر [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Returns:**
int
### getLeftMargin() {#getLeftMargin--}
```
public double getLeftMargin()
```


يحدد الهامش الأيسر للفقرة.

**Returns:**
double
### getLength() {#getLength--}
```
public int getLength()
```


يسترجع طول الأحرف.

**Returns:**
int
### getLineSpace() {#getLineSpace--}
```
public double getLineSpace()
```


يحصل على مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة.

**Returns:**
double
### getLineSpaceSizeType() {#getLineSpaceSizeType--}
```
public int getLineSpaceSizeType()
```


يحصل على مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة.

انظر [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getRightMargin() {#getRightMargin--}
```
public double getRightMargin()
```


يحدد الهامش الأيمن للفقرة.

**Returns:**
double
### getSpaceAfter() {#getSpaceAfter--}
```
public double getSpaceAfter()
```


يحصل على مقدار المسافة البيضاء العمودية التي ستكون موجودة بعد الفقرة.

**Returns:**
double
### getSpaceAfterSizeType() {#getSpaceAfterSizeType--}
```
public int getSpaceAfterSizeType()
```


يحصل على مقدار المسافة البيضاء العمودية التي ستكون موجودة بعد الفقرة.

انظر [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getSpaceBefore() {#getSpaceBefore--}
```
public double getSpaceBefore()
```


يحصل على مقدار المسافة البيضاء العمودية التي ستكون موجودة قبل الفقرة.

**Returns:**
double
### getSpaceBeforeSizeType() {#getSpaceBeforeSizeType--}
```
public int getSpaceBeforeSizeType()
```


يحصل على مقدار المسافة البيضاء العمودية التي ستكون موجودة قبل الفقرة.

انظر [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```


يسترجع الفهرس الابتدائي للأحرف.

**Returns:**
int
### getStops() {#getStops--}
```
public TextTabStopCollection getStops()
```


يحصل على قائمة نقاط التبويب.

**Returns:**
[TextTabStopCollection](../../com.aspose.cells/texttabstopcollection)
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


يرجع خيارات النص.

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getType() {#getType--}
```
public int getType()
```


يحصل على نوع عقدة النص.

انظر [TextNodeType](../../com.aspose.cells/textnodetype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEastAsianLineBreak() {#isEastAsianLineBreak--}
```
public boolean isEastAsianLineBreak()
```


يحدد ما إذا كان يمكن كسر كلمة شرق آسيوية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة.

**Returns:**
boolean
### isHangingPunctuation() {#isHangingPunctuation--}
```
public boolean isHangingPunctuation()
```


يحدد ما إذا كان يجب وضع علامات الترقيم بقوة على سطر النص أو وضعها على سطر نص مختلف.

**Returns:**
boolean
### isLatinLineBreak() {#isLatinLineBreak--}
```
public boolean isLatinLineBreak()
```


يحدد ما إذا كان يمكن كسر كلمة لاتينية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة.

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




### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```


يضبط نوع محاذاة النص الأفقية للفقرة.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDefaultTabSize(double value) {#setDefaultTabSize-double-}
```
public void setDefaultTabSize(double value)
```


يضبط الحجم الافتراضي لحرف الجدولة داخل هذه الفقرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setEastAsianLineBreak(boolean value) {#setEastAsianLineBreak-boolean-}
```
public void setEastAsianLineBreak(boolean value)
```


يحدد ما إذا كان يمكن كسر كلمة شرق آسيوية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFirstLineIndent(double value) {#setFirstLineIndent-double-}
```
public void setFirstLineIndent(double value)
```


يحدد حجم المسافة البادئة التي سيتم تطبيقها على السطر الأول من النص في الفقرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setFontAlignType(int value) {#setFontAlignType-int-}
```
public void setFontAlignType(int value)
```


يحدد موضع الكلمات الفعلية عمودياً على سطر النص. هذا يتعلق بالموضع العمودي للأحرف بالنسبة لخط الأساس.

انظر [TextFontAlignType](../../com.aspose.cells/textfontaligntype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setHangingPunctuation(boolean value) {#setHangingPunctuation-boolean-}
```
public void setHangingPunctuation(boolean value)
```


يحدد ما إذا كان يجب وضع علامات الترقيم بقوة على سطر النص أو وضعها على سطر نص مختلف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLatinLineBreak(boolean value) {#setLatinLineBreak-boolean-}
```
public void setLatinLineBreak(boolean value)
```


يحدد ما إذا كان يمكن كسر كلمة لاتينية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setLeftMargin(double value) {#setLeftMargin-double-}
```
public void setLeftMargin(double value)
```


يحدد الهامش الأيسر للفقرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLineSpace(double value) {#setLineSpace-double-}
```
public void setLineSpace(double value)
```


يضبط مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLineSpaceSizeType(int value) {#setLineSpaceSizeType-int-}
```
public void setLineSpaceSizeType(int value)
```


يضبط مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة.

انظر [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRightMargin(double value) {#setRightMargin-double-}
```
public void setRightMargin(double value)
```


يحدد الهامش الأيمن للفقرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setSpaceAfter(double value) {#setSpaceAfter-double-}
```
public void setSpaceAfter(double value)
```


يضبط مقدار المسافة البيضاء العمودية التي ستكون موجودة بعد الفقرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setSpaceAfterSizeType(int value) {#setSpaceAfterSizeType-int-}
```
public void setSpaceAfterSizeType(int value)
```


يضبط مقدار المسافة البيضاء العمودية التي ستكون موجودة بعد الفقرة.

انظر [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSpaceBefore(double value) {#setSpaceBefore-double-}
```
public void setSpaceBefore(double value)
```


يضبط مقدار المسافة البيضاء العمودية التي ستكون موجودة قبل الفقرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setSpaceBeforeSizeType(int value) {#setSpaceBeforeSizeType-int-}
```
public void setSpaceBeforeSizeType(int value)
```


يضبط مقدار المسافة البيضاء العمودية التي ستكون موجودة قبل الفقرة.

انظر [LineSpaceSizeType](../../com.aspose.cells/linespacesizetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


يضبط نمط WordArt المحدد مسبقًا.

**Remarks**

فقط لنص الشكل/المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | int | [PresetWordArtStyle](../../com.aspose.cells/presetwordartstyle). نمط WordArt المحدد مسبقًا. |

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

