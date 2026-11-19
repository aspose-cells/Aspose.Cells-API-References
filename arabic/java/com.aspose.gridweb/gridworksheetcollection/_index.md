---
title: "GridWorksheetCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على مجموعة من الكائنات."
type: docs
url: /ar/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

يحتوي على مجموعة من كائنات [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add()](#add--) | يضيف ورقة عمل إلى المجموعة. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | يضيف ورقة عمل إلى المجموعة. |
| [addCopy(int sheetIndex)](#addCopy-int-) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة. |
| [calculateFormula()](#calculateFormula--) | يحسب نتيجة الصيغ. |
| [clear()](#clear--) | مسح جميع أوراق العمل. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على عنصر [GridWorksheet](../../com.aspose.gridweb/gridworksheet) عند الفهرس المحدد. |
| [get(String sheetName)](#get-java.lang.String-) | يحصل على عنصر [GridWorksheet](../../com.aspose.gridweb/gridworksheet) بالاسم المحدد. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على حجم المُعدد |
| [getDefaultFontName()](#getDefaultFontName--) | يحصل على اسم الخط الافتراضي للعنصر. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | يحصل على مجموعة جميع كائنات Name في جدول البيانات. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | يحصل على الفاصل العشري لتنسيق/تحليل القيم الرقمية. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | إدراج ورقة عمل. |
| [iterator()](#iterator--) | يحصل على مُعدد الصفوف |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر عند الفهرس المحدد. |
| [removeAt(String name)](#removeAt-java.lang.String-) | يزيل العنصر بالاسم المحدد. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | يضبط اسم الخط الافتراضي للعنصر. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | يضبط الفاصل العشري لتنسيق/تحليل القيم الرقمية. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | يضبط الرؤية للورقة . |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | يبدل الورقتين. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


يضيف ورقة عمل إلى المجموعة.

**Returns:**
int - فهرس كائن [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
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
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


يضيف ورقة عمل إلى المجموعة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم ورقة العمل |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس ورقة العمل المصدر. |

**Returns:**
int - فهرس كائن [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


يضيف ورقة عمل إلى المجموعة وينسخ البيانات من ورقة عمل موجودة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم ورقة العمل المصدر. |

**Returns:**
int - فهرس كائن [GridWorksheet](../../com.aspose.gridweb/gridworksheet).
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


يحسب نتيجة الصيغ.

### clear() {#clear--}
```
public void clear()
```


مسح جميع أوراق العمل.

**Remarks**

يجب أن يحتوي دفتر العمل على ورقة عمل.

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
### get(int index) {#get-int-}
```
public GridWorksheet get(int index)
```


يحصل على عنصر [GridWorksheet](../../com.aspose.gridweb/gridworksheet) عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس الصفري للعنصر. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


يحصل على عنصر [GridWorksheet](../../com.aspose.gridweb/gridworksheet) بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم ورقة العمل. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات.

**Remarks**

فهرس الورقة يبدأ من الصفر.

**Returns:**
int
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


يحصل على حجم المُعدد

**Returns:**
int
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


يحصل على اسم الخط الافتراضي للعنصر.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


يحصل على مجموعة جميع كائنات Name في جدول البيانات.

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


يحصل على الفاصل العشري لتنسيق/تحليل القيم الرقمية. الافتراضي هو الفاصل العشري للمنطقة الحالية.

**Returns:**
char
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
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
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


إدراج ورقة عمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الورقة |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


يحصل على مُعدد الصفوف

**Returns:**
java.util.Iterator - مُعدد الصفوف
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


يزيل العنصر عند الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | قيمة الفهرس للعنصر المراد إزالته. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


يزيل العنصر بالاسم المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم العنصر المراد إزالته. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


يمثل فهرس ورقة العمل النشطة عند فتح جدول البيانات.

**Remarks**

فهرس الورقة يبدأ من الصفر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


يضبط اسم الخط الافتراضي للعنصر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


يضبط الفاصل العشري لتنسيق/تحليل القيم الرقمية. الافتراضي هو الفاصل العشري للمنطقة الحالية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


يضبط الرؤية للورقة .

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetName | java.lang.String | اسم ورقة العمل المصدر. |
| isVisible | boolean | ما إذا كانت ورقة العمل مرئية |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


يبدل الورقتين.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex1 | int | ورقة العمل الأولى. |
| sheetIndex2 | int | ورقة العمل الثانية. |

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

