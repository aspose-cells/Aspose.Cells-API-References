---
title: "PivotTableCalculateOption"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات حساب بيانات جدول PivotTable."
type: docs
url: /ar/java/com.aspose.cells/pivottablecalculateoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableCalculateOption
```

يمثل خيارات حساب بيانات جدول PivotTable.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PivotTableCalculateOption()](#PivotTableCalculateOption--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRefreshCharts()](#getRefreshCharts--) | يشير إلى ما إذا كان تحديث المخططات يعتمد على جدول المحور هذا. |
| [getRefreshData()](#getRefreshData--) | يشير إلى ما إذا كان تحديث مصدر البيانات لجدول المحور. |
| [getRefreshOption()](#getRefreshOption--) | يحصل على الخيارات لتحديث مصدر البيانات إلى ذاكرة التخزين المؤقت للجدول المحوري. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | يمثل كيفية الاحتفاظ بالعناصر المحورية المفقودة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRefreshCharts(boolean value)](#setRefreshCharts-boolean-) | يشير إلى ما إذا كان تحديث المخططات يعتمد على جدول المحور هذا. |
| [setRefreshData(boolean value)](#setRefreshData-boolean-) | يشير إلى ما إذا كان تحديث مصدر البيانات لجدول المحور. |
| [setRefreshOption(PivotTableRefreshOption value)](#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-) | يضبط الخيارات لتحديث مصدر البيانات إلى ذاكرة التخزين المؤقت للجدول المحوري. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | يمثل كيفية الاحتفاظ بالعناصر المحورية المفقودة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableCalculateOption() {#PivotTableCalculateOption--}
```
public PivotTableCalculateOption()
```


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
### getRefreshCharts() {#getRefreshCharts--}
```
public boolean getRefreshCharts()
```


يشير إلى ما إذا كان تحديث المخططات يعتمد على جدول المحور هذا.

**Returns:**
boolean
### getRefreshData() {#getRefreshData--}
```
public boolean getRefreshData()
```


يشير إلى ما إذا كان تحديث مصدر البيانات لجدول المحور.

**Remarks**

إذا كان صحيحًا، يتم تحديث ذاكرة التخزين المؤقت للجدول المحوري من مصدر البيانات، ثم حساب جميع جداول المحور بناءً على نفس الذاكرة.

**Returns:**
boolean
### getRefreshOption() {#getRefreshOption--}
```
public PivotTableRefreshOption getRefreshOption()
```


يحصل على الخيارات لتحديث مصدر البيانات إلى ذاكرة التخزين المؤقت للجدول المحوري.

**Returns:**
[PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption)
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


يمثل كيفية الاحتفاظ بالعناصر المحورية المفقودة.

انظر [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

يعمل فقط عندما يكون [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\\#getRefreshData--) صحيحًا.

**Returns:**
int
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




### setRefreshCharts(boolean value) {#setRefreshCharts-boolean-}
```
public void setRefreshCharts(boolean value)
```


يشير إلى ما إذا كان تحديث المخططات يعتمد على جدول المحور هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRefreshData(boolean value) {#setRefreshData-boolean-}
```
public void setRefreshData(boolean value)
```


يشير إلى ما إذا كان تحديث مصدر البيانات لجدول المحور.

**Remarks**

إذا كان صحيحًا، يتم تحديث ذاكرة التخزين المؤقت للجدول المحوري من مصدر البيانات، ثم حساب جميع جداول المحور بناءً على نفس الذاكرة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRefreshOption(PivotTableRefreshOption value) {#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-}
```
public void setRefreshOption(PivotTableRefreshOption value)
```


يضبط الخيارات لتحديث مصدر البيانات إلى ذاكرة التخزين المؤقت للجدول المحوري.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


يمثل كيفية الاحتفاظ بالعناصر المحورية المفقودة.

انظر [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

يعمل فقط عندما يكون [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\\#getRefreshData--) صحيحًا.

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

