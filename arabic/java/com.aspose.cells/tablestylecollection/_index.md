---
title: "TableStyleCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع أنماط الجدول المخصصة."
type: docs
url: /ar/java/com.aspose.cells/tablestylecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleCollection extends CollectionBase
```

يمثل جميع أنماط الجدول المخصصة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [addPivotTableStyle(String name)](#addPivotTableStyle-java.lang.String-) | يضيف نمط جدول محوري مخصص. |
| [addTableStyle(String name)](#addTableStyle-java.lang.String-) | يضيف نمط جدول مخصص. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على نمط الجدول حسب الفهرس. |
| [get(String name)](#get-java.lang.String-) | يحصل على نمط الجدول حسب الاسم. |
| [getBuiltinTableStyle(int type)](#getBuiltinTableStyle-int-) | يحصل على نمط الجدول المدمج |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getDefaultPivotStyleName()](#getDefaultPivotStyleName--) | يحصل على اسم النمط الافتراضي لجدول محوري. |
| [getDefaultTableStyleName()](#getDefaultTableStyleName--) | يحصل على اسم النمط الافتراضي للجدول. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [setDefaultPivotStyleName(String value)](#setDefaultPivotStyleName-java.lang.String-) | يضبط اسم النمط الافتراضي لجدول محوري. |
| [setDefaultTableStyleName(String value)](#setDefaultTableStyleName-java.lang.String-) | يضبط اسم النمط الافتراضي للجدول. |
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
### addPivotTableStyle(String name) {#addPivotTableStyle-java.lang.String-}
```
public int addPivotTableStyle(String name)
```


يضيف نمط جدول محوري مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نمط الجدول المحوري. |

**Returns:**
int - فهرس نمط الجدول المحوري.
### addTableStyle(String name) {#addTableStyle-java.lang.String-}
```
public int addTableStyle(String name)
```


يضيف نمط جدول مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نمط الجدول. |

**Returns:**
int - فهرس نمط الجدول.
### clear() {#clear--}
```
public void clear()
```


يزيل جميع الكائنات من مثيل CollectionBase.

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
public TableStyle get(int index)
```


يحصل على نمط الجدول حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | موضع نمط الجدول في القائمة. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### get(String name) {#get-java.lang.String-}
```
public TableStyle get(String name)
```


يحصل على نمط الجدول حسب الاسم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| name | java.lang.String | اسم نمط الجدول. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### getBuiltinTableStyle(int type) {#getBuiltinTableStyle-int-}
```
public TableStyle getBuiltinTableStyle(int type)
```


يحصل على نمط الجدول المدمج

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [TableStyleType](../../com.aspose.cells/tablestyletype). نوع نمط الجدول المدمج. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - 
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
### getDefaultPivotStyleName() {#getDefaultPivotStyleName--}
```
public String getDefaultPivotStyleName()
```


يحصل على اسم النمط الافتراضي لجدول محوري.

**Returns:**
java.lang.String
### getDefaultTableStyleName() {#getDefaultTableStyleName--}
```
public String getDefaultTableStyleName()
```


يحصل على اسم النمط الافتراضي للجدول.

**Returns:**
java.lang.String
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

### setDefaultPivotStyleName(String value) {#setDefaultPivotStyleName-java.lang.String-}
```
public void setDefaultPivotStyleName(String value)
```


يضبط اسم النمط الافتراضي لجدول محوري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDefaultTableStyleName(String value) {#setDefaultTableStyleName-java.lang.String-}
```
public void setDefaultTableStyleName(String value)
```


يضبط اسم النمط الافتراضي للجدول.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

