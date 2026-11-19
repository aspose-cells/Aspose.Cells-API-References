---
title: "TextEffectFormat"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الخصائص والطرق التي تنطبق على كائنات WordArt."
type: docs
url: /ar/java/com.aspose.cells/texteffectformat/
---

**Inheritance:**
java.lang.Object
```
public class TextEffectFormat
```

يحتوي على الخصائص والطرق التي تنطبق على كائنات WordArt.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
         shapes.addTextEffect(MsoPresetTextEffect.TEXT_EFFECT_1, "Aspose", "Arial", 30, false, false, 0, 0, 0, 0, 100, 200);
         TextEffectFormat textEffectFormat = shapes.get(0).getTextEffect();
         textEffectFormat.setTextEffect(MsoPresetTextEffect.TEXT_EFFECT_10);
         workbook.save("Book1.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFontBold()](#getFontBold--) | يشير إلى ما إذا كان الخط عريضًا. |
| [getFontItalic()](#getFontItalic--) | يشير إلى ما إذا كان الخط مائلًا. |
| [getFontName()](#getFontName--) | اسم الخط المستخدم في WordArt. |
| [getFontSize()](#getFontSize--) | الحجم (بالنقاط) للخط المستخدم في WordArt. |
| [getPresetShape()](#getPresetShape--) | يحصل على نوع الشكل المحدد مسبقًا. |
| [getRotatedChars()](#getRotatedChars--) | إذا كان true، فإن الأحرف في WordArt المحدد تدور 90 درجة بالنسبة إلى الشكل المحيط بـ WordArt. |
| [getText()](#getText--) | النص في WordArt. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFontBold(boolean value)](#setFontBold-boolean-) | يشير إلى ما إذا كان الخط عريضًا. |
| [setFontItalic(boolean value)](#setFontItalic-boolean-) | يشير إلى ما إذا كان الخط مائلًا. |
| [setFontName(String value)](#setFontName-java.lang.String-) | اسم الخط المستخدم في WordArt. |
| [setFontSize(int value)](#setFontSize-int-) | الحجم (بالنقاط) للخط المستخدم في WordArt. |
| [setPresetShape(int value)](#setPresetShape-int-) | يضبط نوع الشكل المحدد مسبقًا. |
| [setRotatedChars(boolean value)](#setRotatedChars-boolean-) | إذا كان true، فإن الأحرف في WordArt المحدد تدور 90 درجة بالنسبة إلى الشكل المحيط بـ WordArt. |
| [setText(String value)](#setText-java.lang.String-) | النص في WordArt. |
| [setTextEffect(int effect)](#setTextEffect-int-) | يضبط تأثير النص المحدد مسبقًا. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFontBold() {#getFontBold--}
```
public boolean getFontBold()
```


يشير إلى ما إذا كان الخط عريضًا.

**Returns:**
boolean
### getFontItalic() {#getFontItalic--}
```
public boolean getFontItalic()
```


يشير إلى ما إذا كان الخط مائلًا.

**Returns:**
boolean
### getFontName() {#getFontName--}
```
public String getFontName()
```


اسم الخط المستخدم في WordArt.

**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public int getFontSize()
```


الحجم (بالنقاط) للخط المستخدم في WordArt.

**Returns:**
int
### getPresetShape() {#getPresetShape--}
```
public int getPresetShape()
```


يحصل على نوع الشكل المحدد مسبقًا.

انظر [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Returns:**
int
### getRotatedChars() {#getRotatedChars--}
```
public boolean getRotatedChars()
```


إذا كان true، فإن الأحرف في WordArt المحدد تدور 90 درجة بالنسبة إلى الشكل المحيط بـ WordArt.

**Returns:**
boolean
### getText() {#getText--}
```
public String getText()
```


النص في WordArt.

**Returns:**
java.lang.String
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




### setFontBold(boolean value) {#setFontBold-boolean-}
```
public void setFontBold(boolean value)
```


يشير إلى ما إذا كان الخط عريضًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFontItalic(boolean value) {#setFontItalic-boolean-}
```
public void setFontItalic(boolean value)
```


يشير إلى ما إذا كان الخط مائلًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```


اسم الخط المستخدم في WordArt.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFontSize(int value) {#setFontSize-int-}
```
public void setFontSize(int value)
```


الحجم (بالنقاط) للخط المستخدم في WordArt.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPresetShape(int value) {#setPresetShape-int-}
```
public void setPresetShape(int value)
```


يضبط نوع الشكل المحدد مسبقًا.

انظر [MsoPresetTextEffectShape](../../com.aspose.cells/msopresettexteffectshape).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRotatedChars(boolean value) {#setRotatedChars-boolean-}
```
public void setRotatedChars(boolean value)
```


إذا كان true، فإن الأحرف في WordArt المحدد تدور 90 درجة بالنسبة إلى الشكل المحيط بـ WordArt.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


النص في WordArt.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextEffect(int effect) {#setTextEffect-int-}
```
public void setTextEffect(int effect)
```


يضبط تأثير النص المحدد مسبقًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| effect | int | [MsoPresetTextEffect](../../com.aspose.cells/msopresettexteffect). تأثير النص المحدد. |

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

