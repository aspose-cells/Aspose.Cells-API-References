---
title: "FilterValueCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة الفلاتر المتعددة."
type: docs
url: /ar/java/com.aspose.cells/filtervaluecollection/
---

**Inheritance:**
java.lang.Object، [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class FilterValueCollection extends CollectionBase
```

يمثل مجموعة الفلاتر المتعددة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | يضيف قيمة معيار تصفية تاريخ. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | يضيف قيمة معيار تصفية تاريخ ووقت. |
| [add(Object o)](#add-java.lang.Object-) | يضيف عنصرًا إلى مثيل CollectionBase. |
| [add(String filter)](#add-java.lang.String-) | يضيف معيار تصفية تسمية. |
| [clear()](#clear--) | يزيل جميع الكائنات من مثيل CollectionBase. |
| [contains(Object o)](#contains-java.lang.Object-) | إرجاع ما إذا كان المثيل يحتوي على هذا الكائن |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على [FilterValue](../../com.aspose.cells/filtervalue) حسب الفهرس. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد العناصر الموجودة في مثيل CollectionBase. |
| [getMatchBlank()](#getMatchBlank--) | يشير إلى ما إذا كان يجب التصفية حسب الفراغ. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | يحدد فهرس عنصر محدد في مثيل CollectionBase. |
| [iterator()](#iterator--) | يرجع كائن تعداد يتنقل عبر مثيل CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | يزيل العنصر في الفهرس المحدد. |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | يشير إلى ما إذا كان يجب التصفية حسب الفراغ. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


يضيف قيمة معيار تصفية تاريخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). نوع تصفية التاريخ. |
| سنة | int | السنة. |
| شهر | int | الشهر. |
| يوم | int | اليوم. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


يضيف قيمة معيار تصفية تاريخ ووقت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). نوع تصفية التاريخ. |
| سنة | int | السنة. |
| شهر | int | الشهر. |
| يوم | int | اليوم. |
| ساعة | int | الساعة. |
| دقيقة | int | الدقيقة. |
| ثانية | int | الثانية. |

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
### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


يضيف معيار تصفية تسمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تصفية | java.lang.String | بيانات الفلتر. |

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
public FilterValue get(int index)
```


يحصل على [FilterValue](../../com.aspose.cells/filtervalue) حسب الفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
[FilterValue](../../com.aspose.cells/filtervalue) - 
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
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


يشير إلى ما إذا كان يجب التصفية حسب الفراغ.

**Returns:**
boolean
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

### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


يشير إلى ما إذا كان يجب التصفية حسب الفراغ.

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

