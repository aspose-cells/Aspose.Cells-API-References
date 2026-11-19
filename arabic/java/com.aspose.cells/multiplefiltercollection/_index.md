---
title: "MultipleFilterCollection"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مجموعة الفلاتر المتعددة."
type: docs
url: /ar/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

يمثل مجموعة الفلاتر المتعددة.

**Remarks**

ملاحظة: هذه الفئة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام [FilterValueCollection](../../com.aspose.cells/filtervaluecollection). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | ينشئ نسخة جديدة واحدة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | يضيف قيمة معيار تصفية تاريخ. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | يضيف قيمة معيار تصفية تاريخ ووقت. |
| [add(String filter)](#add-java.lang.String-) | يضيف معيار تصفية تسمية. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | يحصل على [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) أو قيمة نصية. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | يحصل على عدد قيم التصفية. |
| [getMatchBlank()](#getMatchBlank--) | يشير إلى ما إذا كان يجب التصفية حسب الفراغ. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | احصل على المُعدِّد لقيمة التصفية، |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | يشير إلى ما إذا كان يجب التصفية حسب الفراغ. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


ينشئ نسخة جديدة واحدة.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى تعيين FilterColumn.FilterType كـ FilterType.MultipleFilters ثم الحصول على FilterColumn.MultipleFilters. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

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

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


يضيف معيار تصفية تسمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| تصفية | java.lang.String | بيانات الفلتر. |

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
public Object get(int index)
```


يحصل على [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) أو قيمة نصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int |  |

**Returns:**
java.lang.Object - 
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


يحصل على عدد قيم التصفية.

**Returns:**
int
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
### iterator() {#iterator--}
```
public Iterator iterator()
```


احصل على المُعدِّد لقيمة التصفية،

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

