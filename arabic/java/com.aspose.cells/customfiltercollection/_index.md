---
title: "CustomFilterCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الفلاتر المخصصة."
type: docs
url: /ar/java/com.aspose.cells/customfiltercollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class CustomFilterCollection extends CollectionBase
```

يمثل الفلاتر المخصصة.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [CustomFilterCollection()](#CustomFilterCollection--) | ينشئ نسخة جديدة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-java.lang.Object-boolean-int-java.lang.Object-) | يفلتر قائمة باستخدام معايير مخصصة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على الفلتر المخصص في الفهرس المحدد. |
| [getAnd()](#getAnd--) | يشير إلى ما إذا كان للمعيارين علاقة \"و\". |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [setAnd(boolean value)](#setAnd-boolean-) | يشير إلى ما إذا كان للمعيارين علاقة \"و\". |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CustomFilterCollection() {#CustomFilterCollection--}
```
public CustomFilterCollection()
```


ينشئ نسخة جديدة.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى تعيين FilterColumn.FilterType كـ FilterType.CustomFilters ثم الحصول على FilterColumn.CustomFilters. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

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
### custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


يفلتر قائمة باستخدام معايير مخصصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). نوع عامل الفلتر |
| criteria1 | java.lang.Object | المعيار المخصص |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). نوع عامل الفلتر |
| criteria2 | java.lang.Object | المعيار المخصص |

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
public CustomFilter get(int index)
```


يحصل على الفلتر المخصص في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | الفهرس. |

**Returns:**
[CustomFilter](../../com.aspose.cells/customfilter) - 
### getAnd() {#getAnd--}
```
public boolean getAnd()
```


يشير إلى ما إذا كان للمعيارين علاقة \"و\".

**Returns:**
boolean
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

### setAnd(boolean value) {#setAnd-boolean-}
```
public void setAnd(boolean value)
```


يشير إلى ما إذا كان للمعيارين علاقة \"و\".

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

