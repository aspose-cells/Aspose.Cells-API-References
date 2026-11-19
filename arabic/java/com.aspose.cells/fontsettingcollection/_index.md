---
title: "FontSettingCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل القائمة."
type: docs
url: /ar/java/com.aspose.cells/fontsettingcollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FontSettingCollection extends CollectionBase
```

يمثل قائمة [FontSetting](../../com.aspose.cells/fontsetting).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [appendText(String text)](#appendText-java.lang.String-) | يضيف النص. |
| [clear()](#clear--) | امسح جميع الإعدادات. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [deleteText(int index, int count)](#deleteText-int-int-) | احذف بعض الأحرف. |
| [equals(Object obj)](#equals-java.lang.Object-) |  |
| [format(int startIndex, int length, Font font, StyleFlag flag)](#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | نسق النص باستخدام إعداد الخط. |
| [get(int index)](#get-int-) | يحصل على [FontSetting](../../com.aspose.cells/fontsetting) حسب الفهرس. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getHtmlString()](#getHtmlString--) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا الشكل. |
| [getParagraphEnumerator()](#getParagraphEnumerator--) | يحصل على المكرّر للفقرات. |
| [getText()](#getText--) | يحصل على نص الشكل. |
| [getTextAlignment()](#getTextAlignment--) | يمثل إعداد محاذاة جسم النص. |
| [getTextParagraphs()](#getTextParagraphs--) | يحصل على جميع الفقرات. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [insertText(int index, String text)](#insertText-int-java.lang.String-) | أدرج الفهرس في الموضع. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [replace(int index, int count, String text)](#replace-int-int-java.lang.String-) | استبدل النص. |
| [replace(String oldValue, String newValue)](#replace-java.lang.String-java.lang.String-) | استبدل النص. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | يضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا الشكل. |
| [setText(String value)](#setText-java.lang.String-) | يضبط نص الشكل. |
| [setWordArtStyle(int style)](#setWordArtStyle-int-) | يضبط نمط WordArt المحدد مسبقًا. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


يضيف عنصرًا إلى مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | الكائن لإضافته إلى مثيل CollectionBase. |

**Returns:**
int - الموضع الذي تم إدراج العنصر الجديد فيه.
### appendText(String text) {#appendText-java.lang.String-}
```
public void appendText(String text)
```


يضيف النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | النص. |

### clear() {#clear--}
```
public void clear()
```


امسح جميع الإعدادات.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


إرجاع ما إذا كان المثيل يحتوي على هذا الكائن

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | كائن اختبار |

**Returns:**
boolean - ما إذا كان المثيل يحتوي على هذا الكائن
### deleteText(int index, int count) {#deleteText-int-int-}
```
public void deleteText(int index, int count)
```


احذف بعض الأحرف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس البداية. |
| العدد | int | عدد الأحرف. |

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
### format(int startIndex, int length, Font font, StyleFlag flag) {#format-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void format(int startIndex, int length, Font font, StyleFlag flag)
```


نسق النص باستخدام إعداد الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startIndex | int | فهرس البداية. |
| length | int | الطول. |
| font | [Font](../../com.aspose.cells/font) | الخط. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | علامات الخط. |

### get(int index) {#get-int-}
```
public FontSetting get(int index)
```


يحصل على [FontSetting](../../com.aspose.cells/fontsetting) حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


يحصل على عدد العناصر الموجودة في مثيل CollectionBase.

**Returns:**
int - عدد العناصر الموجودة في مثيل CollectionBase.
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا الشكل.

**Returns:**
java.lang.String
### getParagraphEnumerator() {#getParagraphEnumerator--}
```
public Iterator getParagraphEnumerator()
```


يحصل على المكرّر للفقرات.

**Returns:**
java.util.Iterator -
### getText() {#getText--}
```
public String getText()
```


يحصل على نص الشكل.

**Returns:**
java.lang.String
### getTextAlignment() {#getTextAlignment--}
```
public ShapeTextAlignment getTextAlignment()
```


يمثل إعداد محاذاة جسم النص.

**Returns:**
[ShapeTextAlignment](../../com.aspose.cells/shapetextalignment)
### getTextParagraphs() {#getTextParagraphs--}
```
public TextParagraphCollection getTextParagraphs()
```


يحصل على جميع الفقرات.

**Returns:**
[TextParagraphCollection](../../com.aspose.cells/textparagraphcollection)
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


يحدد فهرس عنصر محدد في مثيل CollectionBase.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| o | java.lang.Object | يحدد فهرس عنصر محدد في مثيل CollectionBase. |

**Returns:**
int - فهرس القيمة إذا وجد في القائمة؛ وإلا -1.
### insertText(int index, String text) {#insertText-int-java.lang.String-}
```
public void insertText(int index, String text)
```


أدرج الفهرس في الموضع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس البداية. |
| نص | java.lang.String | النص. |

### iterator() {#iterator--}
```
public Iterator iterator()
```


يرجع كائن تعداد يتنقل عبر مثيل CollectionBase.

**Returns:**
java.util.Iterator - كائن تكرار لمثيل CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


يزيل العنصر في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر المراد إزالته. |

### replace(int index, int count, String text) {#replace-int-int-java.lang.String-}
```
public void replace(int index, int count, String text)
```


استبدل النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس البداية. |
| العدد | int | عدد الأحرف. |
| نص | java.lang.String | النص. |

### replace(String oldValue, String newValue) {#replace-java.lang.String-java.lang.String-}
```
public void replace(String oldValue, String newValue)
```


استبدل النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | java.lang.String | النص القديم. |
| newValue | java.lang.String | النص الجديد. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


يضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذا الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


يضبط نص الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setWordArtStyle(int style) {#setWordArtStyle-int-}
```
public void setWordArtStyle(int style)
```


يضبط نمط WordArt المحدد مسبقًا.

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

