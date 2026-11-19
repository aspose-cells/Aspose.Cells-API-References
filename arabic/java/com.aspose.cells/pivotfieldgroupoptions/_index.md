---
title: "PivotFieldGroupOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "خيارات إعدادات تجميع حقل المحور."
type: docs
url: /ar/java/com.aspose.cells/pivotfieldgroupoptions/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldGroupOptions
```

خيارات إعدادات تجميع حقل المحور.

**Example**

```
         // Load the sample workbook
         Workbook wb = new Workbook("sampleGroupPivotFieldsInPivotTable.xlsx");
         // Access the second worksheet and its pivot table
         PivotTable pt = wb.getWorksheets().get(1).getPivotTables().get(0);
         // Group the first row field (a date field) by months and quarters
         PivotFieldGroupOptions options = new PivotFieldGroupOptions();
         options.setStartDate(new DateTime(2008, 1, 1));
         options.setEndDate(new DateTime(2008, 9, 5));
         options.setGroupTypes(new /*PivotGroupByType*/int[] { PivotGroupByType.MONTHS, PivotGroupByType.QUARTERS });
         pt.getRowFields().get(0).group(options);
         // Calculate the pivot table data and save the output file
         pt.calculateData();
         wb.save("outputGroupPivotFieldsInPivotTable.xlsx");
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PivotFieldGroupOptions()](#PivotFieldGroupOptions--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDiscreteGroupItems()](#getDiscreteGroupItems--) | يحصل على عناصر المجموعة المتقطعة. |
| [getEndDate()](#getEndDate--) | يحصل على القيمة النهائية لنطاق التجميع. |
| [getEndNumber()](#getEndNumber--) | يحصل على القيمة النهائية لنطاق التجميع. |
| [getGroupType()](#getGroupType--) | يحصل على نوع التجميع لحقل المحور. |
| [getGroupTypes()](#getGroupTypes--) | يحصل على نوع التجميع لحقل المحور. |
| [getInterval()](#getInterval--) | يحصل على حجم الفاصل لكل مجموعة. |
| [getNewPivotField()](#getNewPivotField--) | يحصل على قيمة تشير إلى ما إذا كان يجب إنشاء حقول محور جديدة بعد التجميع. |
| [getStartDate()](#getStartDate--) | يحصل على القيمة الابتدائية لنطاق التجميع. |
| [getStartNumber()](#getStartNumber--) | يحصل على القيمة الابتدائية لنطاق التجميع. |
| [hashCode()](#hashCode--) |  |
| [isAutoEnd()](#isAutoEnd--) | يحصل على قيمة تشير إلى ما إذا كانت القيمة النهائية محددة تلقائيًا. |
| [isAutoStart()](#isAutoStart--) | يحصل على قيمة تشير إلى ما إذا كانت القيمة الابتدائية محددة تلقائيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoEnd(boolean value)](#setAutoEnd-boolean-) | يضبط قيمة تشير إلى ما إذا كانت القيمة النهائية محددة تلقائيًا. |
| [setAutoStart(boolean value)](#setAutoStart-boolean-) | يضبط قيمة تشير إلى ما إذا كانت القيمة الابتدائية محددة تلقائيًا. |
| [setDiscreteGroupItems(DiscreteGroupItem[] value)](#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---) | يضبط عناصر المجموعة المتقطعة. |
| [setEndDate(DateTime value)](#setEndDate-com.aspose.cells.DateTime-) | يضبط القيمة النهائية لنطاق التجميع. |
| [setEndNumber(double value)](#setEndNumber-double-) | يضبط القيمة النهائية لنطاق التجميع. |
| [setGroupType(int value)](#setGroupType-int-) | يضبط نوع التجميع لحقل المحور. |
| [setGroupTypes(int[] value)](#setGroupTypes-int---) | يضبط نوع التجميع لحقل المحور. |
| [setInterval(double value)](#setInterval-double-) | يضبط حجم الفاصل لكل مجموعة. |
| [setNewPivotField(boolean value)](#setNewPivotField-boolean-) | يضبط قيمة تشير إلى ما إذا كان يجب إنشاء حقول محور جديدة بعد التجميع. |
| [setStartDate(DateTime value)](#setStartDate-com.aspose.cells.DateTime-) | يضبط القيمة الابتدائية لنطاق التجميع. |
| [setStartNumber(double value)](#setStartNumber-double-) | يضبط القيمة الابتدائية لنطاق التجميع. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotFieldGroupOptions() {#PivotFieldGroupOptions--}
```
public PivotFieldGroupOptions()
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
### getDiscreteGroupItems() {#getDiscreteGroupItems--}
```
public DiscreteGroupItem[] getDiscreteGroupItems()
```


يحصل على عناصر المجموعة المتقطعة.

**Remarks**

إذا تم تعيين هذه الخاصية،[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Returns:**
com.aspose.cells.DiscreteGroupItem[]
### getEndDate() {#getEndDate--}
```
public DateTime getEndDate()
```


يحصل على القيمة النهائية لنطاق التجميع.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getEndNumber() {#getEndNumber--}
```
public double getEndNumber()
```


يحصل على القيمة النهائية لنطاق التجميع.

**Returns:**
double
### getGroupType() {#getGroupType--}
```
public int getGroupType()
```


يحصل على نوع التجميع لحقل المحور. فقط لتجميع حقل المحور التاريخ والوقت.

انظر [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Example**

```
         //init
         PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
         // Group by year and month together
         /*PivotGroupByType*/int pivotGroupByType = pivotFieldGroupOptions.getGroupType();
         pivotGroupByType = PivotGroupByType.YEARS | PivotGroupByType.MONTHS;
         pivotFieldGroupOptions.setGroupType(pivotGroupByType);
```

**Returns:**
int
### getGroupTypes() {#getGroupTypes--}
```
public int[] getGroupTypes()
```


يحصل على نوع التجميع لحقل المحور.

انظر [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

سيتم تجاهل الترتيب في هذه الخاصية. عند تحديد أنواع تجميع متعددة، سيتم إدراج حقول المجموعة الأساسية بترتيب تصاعدي وعرض حقل المجموعة إلى منطقة الصف/العمود بترتيب تنازلي (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Returns:**
int[]
### getInterval() {#getInterval--}
```
public double getInterval()
```


يحصل على حجم الفاصل لكل مجموعة.

**Remarks**

فقط لمجموعة الأرقام والأيام.

**Returns:**
double
### getNewPivotField() {#getNewPivotField--}
```
public boolean getNewPivotField()
```


يحصل على قيمة تشير إلى ما إذا كان يجب إنشاء حقول محور جديدة بعد التجميع.

**Remarks**

إذا لم يتم تعيينه صراحةً، فإن القيمة الافتراضية هي false لتجميع الأرقام و true لتجميع التاريخ والوقت، true للمجموعة المتقطعة. يعمل فقط على أول حقل محور مجموعة جديد للحقل الأساسي.

**Returns:**
boolean
### getStartDate() {#getStartDate--}
```
public DateTime getStartDate()
```


يحصل على القيمة الابتدائية لنطاق التجميع.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getStartNumber() {#getStartNumber--}
```
public double getStartNumber()
```


يحصل على القيمة الابتدائية لنطاق التجميع.

**Returns:**
double
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutoEnd() {#isAutoEnd--}
```
public boolean isAutoEnd()
```


يحصل على قيمة تشير إلى ما إذا كانت القيمة النهائية محددة تلقائيًا.

**Remarks**

إذا تم تعيين [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) أو [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--)، ستكون هذه الخاصية false.

**Returns:**
boolean
### isAutoStart() {#isAutoStart--}
```
public boolean isAutoStart()
```


يحصل على قيمة تشير إلى ما إذا كانت القيمة الابتدائية محددة تلقائيًا.

**Remarks**

إذا تم تعيين [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) أو [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--)، ستكون هذه الخاصية false.

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




### setAutoEnd(boolean value) {#setAutoEnd-boolean-}
```
public void setAutoEnd(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت القيمة النهائية محددة تلقائيًا.

**Remarks**

إذا تم تعيين [getEndNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndNumber--) أو [getEndDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getEndDate--)، ستكون هذه الخاصية false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoStart(boolean value) {#setAutoStart-boolean-}
```
public void setAutoStart(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت القيمة الابتدائية محددة تلقائيًا.

**Remarks**

إذا تم تعيين [getStartNumber()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartNumber--) أو [getStartDate()](../../com.aspose.cells/pivotfieldgroupoptions\#getStartDate--)، ستكون هذه الخاصية false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDiscreteGroupItems(DiscreteGroupItem[] value) {#setDiscreteGroupItems-com.aspose.cells.DiscreteGroupItem---}
```
public void setDiscreteGroupItems(DiscreteGroupItem[] value)
```


يضبط عناصر المجموعة المتقطعة.

**Remarks**

إذا تم تعيين هذه الخاصية،[getGroupType()](../../com.aspose.cells/pivotfieldgroupoptions\#getGroupType--)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DiscreteGroupItem\[\]](../../com.aspose.cells/discretegroupitem) |  |

### setEndDate(DateTime value) {#setEndDate-com.aspose.cells.DateTime-}
```
public void setEndDate(DateTime value)
```


يضبط القيمة النهائية لنطاق التجميع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setEndNumber(double value) {#setEndNumber-double-}
```
public void setEndNumber(double value)
```


يضبط القيمة النهائية لنطاق التجميع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setGroupType(int value) {#setGroupType-int-}
```
public void setGroupType(int value)
```


يضبط نوع التجميع لحقل المحور. فقط لتجميع حقل المحور التاريخ والوقت.

انظر [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setGroupTypes(int[] value) {#setGroupTypes-int---}
```
public void setGroupTypes(int[] value)
```


يضبط نوع التجميع لحقل المحور.

انظر [PivotGroupByType](../../com.aspose.cells/pivotgroupbytype).

**Remarks**

سيتم تجاهل الترتيب في هذه الخاصية. عند تحديد أنواع تجميع متعددة، سيتم إدراج حقول المجموعة الأساسية بترتيب تصاعدي وعرض حقل المجموعة إلى منطقة الصف/العمود بترتيب تنازلي (Years \\u922b?Quarters \\u922b?Months \\u922b?Days \\u922b?Hours \\u922b?Minutes \\u922b?Seconds).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int[] |  |

### setInterval(double value) {#setInterval-double-}
```
public void setInterval(double value)
```


يضبط حجم الفاصل لكل مجموعة.

**Remarks**

فقط لمجموعة الأرقام والأيام.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setNewPivotField(boolean value) {#setNewPivotField-boolean-}
```
public void setNewPivotField(boolean value)
```


يضبط قيمة تشير إلى ما إذا كان يجب إنشاء حقول محور جديدة بعد التجميع.

**Remarks**

إذا لم يتم تعيينه صراحةً، فإن القيمة الافتراضية هي false لتجميع الأرقام و true لتجميع التاريخ والوقت، true للمجموعة المتقطعة. يعمل فقط على أول حقل محور مجموعة جديد للحقل الأساسي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStartDate(DateTime value) {#setStartDate-com.aspose.cells.DateTime-}
```
public void setStartDate(DateTime value)
```


يضبط القيمة الابتدائية لنطاق التجميع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setStartNumber(double value) {#setStartNumber-double-}
```
public void setStartNumber(double value)
```


يضبط القيمة الابتدائية لنطاق التجميع.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

