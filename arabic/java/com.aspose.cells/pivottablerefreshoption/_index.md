---
title: "PivotTableRefreshOption"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات تحديث مصدر بيانات جدول PivotTable."
type: docs
url: /ar/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

يمثل خيارات تحديث مصدر بيانات جدول PivotTable.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | يمثل خيارات تحديث مصدر بيانات جدول PivotTable. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | يشير إلى ما إذا كان يجب الاحتفاظ ببيانات المجموعة المحلية المخزنة مؤقتًا إذا ظلت القيم القصوى والدنيا دون تغيير. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | يمثل كيفية الاحتفاظ بالعناصر المحورية المفقودة. |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | يشير إلى ما إذا كان يجب الحفاظ على الترتيب الأصلي لعناصر المحور كما في مصدر البيانات القديم. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | يشير إلى ما إذا كان يجب الاحتفاظ ببيانات المجموعة المحلية المخزنة مؤقتًا إذا ظلت القيم القصوى والدنيا دون تغيير. |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | يشير إلى ما إذا كان يجب الحفاظ على الترتيب الأصلي لعناصر المحور كما في مصدر البيانات القديم. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | يمثل كيفية الاحتفاظ بالعناصر المحورية المفقودة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


يمثل خيارات تحديث مصدر بيانات جدول PivotTable.

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


يشير إلى ما إذا كان يجب الاحتفاظ ببيانات المجموعة المحلية المخزنة مؤقتًا إذا ظلت القيم القصوى والدنيا دون تغيير. القيمة الافتراضية هي false مما يعني تحديث المجموعة بالإعداد المحلي.

**Remarks**

هذا حل مؤقت، يرجى تعريب الجداول المحورية بتنفيذ [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


يمثل كيفية الاحتفاظ بالعناصر المحورية المفقودة.

انظر [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isKeepOriginalOrder() {#isKeepOriginalOrder--}
```
public boolean isKeepOriginalOrder()
```


يشير إلى ما إذا كان يجب الحفاظ على الترتيب الأصلي لعناصر المحور كما في مصدر البيانات القديم.

**Remarks**

ينطبق فقط على حقل المحور غير المرتب. عند تحديث هذا النوع من حقل المحور، يحتفظ Ms Excel بالترتيب الأصلي لمصدر البيانات القديم. القيمة الافتراضية لهذه الخاصية هي true، مما يمثل نفس سلوك Ms Excel. إذا كان المستخدم يحتاج إلى تحديث حقل المحور بالكامل كما البيانات في مصدر البيانات الجديد، يجب ضبط هذه الخاصية على false.

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




### setKeepCachedLocalGroupData(boolean value) {#setKeepCachedLocalGroupData-boolean-}
```
public void setKeepCachedLocalGroupData(boolean value)
```


يشير إلى ما إذا كان يجب الاحتفاظ ببيانات المجموعة المحلية المخزنة مؤقتًا إذا ظلت القيم القصوى والدنيا دون تغيير. القيمة الافتراضية هي false مما يعني تحديث المجموعة بالإعداد المحلي.

**Remarks**

هذا حل مؤقت، يرجى تعريب الجداول المحورية بتنفيذ [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


يشير إلى ما إذا كان يجب الحفاظ على الترتيب الأصلي لعناصر المحور كما في مصدر البيانات القديم.

**Remarks**

ينطبق فقط على حقل المحور غير المرتب. عند تحديث هذا النوع من حقل المحور، يحتفظ Ms Excel بالترتيب الأصلي لمصدر البيانات القديم. القيمة الافتراضية لهذه الخاصية هي true، مما يمثل نفس سلوك Ms Excel. إذا كان المستخدم يحتاج إلى تحديث حقل المحور بالكامل كما البيانات في مصدر البيانات الجديد، يجب ضبط هذه الخاصية على false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


يمثل كيفية الاحتفاظ بالعناصر المحورية المفقودة.

انظر [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

