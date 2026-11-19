---
title: "SettablePivotGlobalizationSettings"
second_title: "Aspose.Cells for Java API Reference"
description: "تنفيذ PivotGlobalizationSettings الذي يدعم المستخدم لتعيين/تغيير النصوص المعرفة مسبقًا."
type: docs
url: /ar/java/com.aspose.cells/settablepivotglobalizationsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)
```
public class SettablePivotGlobalizationSettings extends PivotGlobalizationSettings
```

تنفيذ PivotGlobalizationSettings الذي يدعم المستخدم لتعيين/تغيير النصوص المعرفة مسبقًا.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [SettablePivotGlobalizationSettings()](#SettablePivotGlobalizationSettings--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatOfDayGroup()](#getFormatOfDayGroup--) | يحصل على تنسيق الرقم لمجموعة أيام المحور. |
| [getNameOfDataField(int function, String name)](#getNameOfDataField-int-java.lang.String-) | يحصل على اسم العرض لحقل محور البيانات. |
| [getShortTextOf12Months()](#getShortTextOf12Months--) | يحصل على جميع السلاسل القصيرة المنسقة لـ 12 شهرًا. |
| [getTextOf24Hours()](#getTextOf24Hours--) | يحصل على جميع السلاسل المنسقة محليًا لـ 24 ساعة. |
| [getTextOf4Quarters()](#getTextOf4Quarters--) | يحصل على النص المحلي لـ 4 أرباع. |
| [getTextOf4Quaters()](#getTextOf4Quaters--) | يحصل على النص المحلي لـ 4 أرباع. |
| [getTextOfAll()](#getTextOfAll--) | يحصل على نص التسمية "(All)" في جدول المحور. |
| [getTextOfAllPeriods()](#getTextOfAllPeriods--) | يحصل على النص المترجم لـ "All Periods". |
| [getTextOfColumnLabels()](#getTextOfColumnLabels--) | يحصل على نص التسمية "Column Labels" في جدول المحور. |
| [getTextOfDataFieldHeader()](#getTextOfDataFieldHeader--) | يحصل على النص الخاص برأس حقل منطقة القيمة في جدول PivotTable. |
| [getTextOfDays()](#getTextOfDays--) | يحصل على النص المحلي لـ "Days". |
| [getTextOfEmptyData()](#getTextOfEmptyData--) | يحصل على نص التسمية "(blank)" في جدول PivotTable. |
| [getTextOfGrandTotal()](#getTextOfGrandTotal--) | يحصل على نص التسمية "Grand Total" في جدول PivotTable. |
| [getTextOfHours()](#getTextOfHours--) | يحصل على النص المحلي لـ "Hours". |
| [getTextOfMinutes()](#getTextOfMinutes--) | يحصل على النص المحلي لـ "Minutes". |
| [getTextOfMonths()](#getTextOfMonths--) | يحصل على النص المحلي لـ "Months". |
| [getTextOfMultipleItems()](#getTextOfMultipleItems--) | يحصل على نص التسمية "(Multiple Items)" في جدول PivotTable. |
| [getTextOfOr()](#getTextOfOr--) | يحصل على جميع السلاسل المنسقة محليًا لـ "or". |
| [getTextOfProtectedName(String protectedName)](#getTextOfProtectedName-java.lang.String-) | يحصل على النص للاسم المحمي المحدد. |
| [getTextOfProtection()](#getTextOfProtection--) | يحصل على اسم الحماية في PivotTable. |
| [getTextOfQuarters()](#getTextOfQuarters--) | احصل على النص المحلي لـ "Quarters". |
| [getTextOfRange()](#getTextOfRange--) | يحصل على النص المحلي لـ "Range" |
| [getTextOfRowLabels()](#getTextOfRowLabels--) | يحصل على نص التسمية "Row Labels" في جدول PivotTable. |
| [getTextOfSeconds()](#getTextOfSeconds--) | يحصل على النص المحلي لـ "Seconds" |
| [getTextOfSubTotal(int subTotalType)](#getTextOfSubTotal-int-) | يحصل على نص نوع [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) في جدول PivotTable. |
| [getTextOfTotal()](#getTextOfTotal--) | يحصل على نص التسمية "Total" في جدول PivotTable. |
| [getTextOfYears()](#getTextOfYears--) | يحصل على النص المحلي لـ "Years". |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setTextOfAll(String text)](#setTextOfAll-java.lang.String-) | يضبط نص التسمية "(All)" في PivotTable. |
| [setTextOfColumnLabels(String text)](#setTextOfColumnLabels-java.lang.String-) | يحصل على نص التسمية "Column Labels" في جدول المحور. |
| [setTextOfDataFieldHeader(String text)](#setTextOfDataFieldHeader-java.lang.String-) | يضبط نص عنوان حقل منطقة القيمة في PivotTable. |
| [setTextOfEmptyData(String text)](#setTextOfEmptyData-java.lang.String-) | يضبط نص التسمية "(blank)" في PivotTable. |
| [setTextOfGrandTotal(String text)](#setTextOfGrandTotal-java.lang.String-) | يضبط نص التسمية "Grand Total" في PivotTable. |
| [setTextOfMultipleItems(String text)](#setTextOfMultipleItems-java.lang.String-) | يضبط نص التسمية "(Multiple Items)" في PivotTable. |
| [setTextOfProtectedName(String protectedName, String text)](#setTextOfProtectedName-java.lang.String-java.lang.String-) | يضبط النص لاسم محمي محدد. |
| [setTextOfRowLabels(String text)](#setTextOfRowLabels-java.lang.String-) | يضبط نص التسمية "Row Labels" في PivotTable. |
| [setTextOfSubTotal(int subTotalType, String text)](#setTextOfSubTotal-int-java.lang.String-) | يضبط نص النوع [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) في PivotTable. |
| [setTextOfTotal(String text)](#setTextOfTotal-java.lang.String-) | يضبط نص التسمية "Total" في PivotTable. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SettablePivotGlobalizationSettings() {#SettablePivotGlobalizationSettings--}
```
public SettablePivotGlobalizationSettings()
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
### getFormatOfDayGroup() {#getFormatOfDayGroup--}
```
public String getFormatOfDayGroup()
```


يحصل على تنسيق الرقم لمجموعة أيام المحور. يُستخدم فقط عند تجميع حقل المحور حسب الأيام. القيمة الافتراضية هي "d-MMM";

**Returns:**
java.lang.String -
### getNameOfDataField(int function, String name) {#getNameOfDataField-int-java.lang.String-}
```
public String getNameOfDataField(int function, String name)
```


يحصل على الاسم المعروض لحقل بيانات المحور. التنسيق الافتراضي هو "Sum Of Field".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction). الدالة تُستخدم لتلخيص قيم حقل المحور. |
| name | java.lang.String | الاسم الأصلي لحقل المحور. |

**Returns:**
java.lang.String -
### getShortTextOf12Months() {#getShortTextOf12Months--}
```
public String[] getShortTextOf12Months()
```


يحصل على جميع السلاسل القصيرة المنسقة لـ 12 شهرًا.

**Returns:**
java.lang.String[] -
### getTextOf24Hours() {#getTextOf24Hours--}
```
public String[] getTextOf24Hours()
```


يحصل على جميع السلاسل المنسقة محليًا لـ 24 ساعة. القيمة الافتراضية هي 12 ص, 1 ص, 2 ص, 3 ص, 4 ص, 5 ص, 6 ص, 7 ص, 8 ص, 9 ص, 10 ص, 11 ص, 12 م, 1 م, 2 م, 3 م, 4 م, 5 م, 6 م, 7 م, 8 م, 9 م, 10 م, 11 م.

**Returns:**
java.lang.String[] -
### getTextOf4Quarters() {#getTextOf4Quarters--}
```
public String[] getTextOf4Quarters()
```


يحصل على النص المحلي لـ 4 أرباع.

**Remarks**

إفتراضيًا يُرجع Quarter1, Quarter2, Quarter3, Quarter4 قبل الإصدار 26.9. إفتراضيًا يُرجع Qtr1, Qtr2, Qtr3, Qtr4 منذ الإصدار 26.9.

**Returns:**
java.lang.String[] -
### getTextOf4Quaters() {#getTextOf4Quaters--}
```
public String[] getTextOf4Quaters()
```


يحصل على النص المحلي لـ 4 أرباع.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetTextOf4Quarters() method. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String[] -
### getTextOfAll() {#getTextOfAll--}
```
public String getTextOfAll()
```


يحصل على نص التسمية "(All)" في جدول المحور.

**Returns:**
java.lang.String - النص الخاص بوسم "(All)"
### getTextOfAllPeriods() {#getTextOfAllPeriods--}
```
public String getTextOfAllPeriods()
```


يحصل على النص المترجم لـ "All Periods".

**Returns:**
java.lang.String -
### getTextOfColumnLabels() {#getTextOfColumnLabels--}
```
public String getTextOfColumnLabels()
```


يحصل على نص التسمية "Column Labels" في جدول المحور.

**Returns:**
java.lang.String - النص الخاص بتسميات الأعمدة
### getTextOfDataFieldHeader() {#getTextOfDataFieldHeader--}
```
public String getTextOfDataFieldHeader()
```


يحصل على النص الخاص برأس حقل منطقة القيمة في جدول PivotTable.

**Returns:**
java.lang.String - النص الخاص باسم رأس حقل البيانات
### getTextOfDays() {#getTextOfDays--}
```
public String getTextOfDays()
```


يحصل على النص المحلي لـ "Days".

**Returns:**
java.lang.String -
### getTextOfEmptyData() {#getTextOfEmptyData--}
```
public String getTextOfEmptyData()
```


يحصل على نص التسمية "(blank)" في جدول PivotTable.

**Returns:**
java.lang.String - النص الخاص بالبيانات الفارغة
### getTextOfGrandTotal() {#getTextOfGrandTotal--}
```
public String getTextOfGrandTotal()
```


يحصل على نص التسمية "Grand Total" في جدول PivotTable.

**Returns:**
java.lang.String - النص الخاص بوسم "Grand Total"
### getTextOfHours() {#getTextOfHours--}
```
public String getTextOfHours()
```


يحصل على النص المحلي لـ "Hours".

**Returns:**
java.lang.String -
### getTextOfMinutes() {#getTextOfMinutes--}
```
public String getTextOfMinutes()
```


يحصل على النص المحلي لـ "Minutes".

**Returns:**
java.lang.String -
### getTextOfMonths() {#getTextOfMonths--}
```
public String getTextOfMonths()
```


يحصل على النص المحلي لـ "Months".

**Returns:**
java.lang.String -
### getTextOfMultipleItems() {#getTextOfMultipleItems--}
```
public String getTextOfMultipleItems()
```


يحصل على نص التسمية "(Multiple Items)" في جدول PivotTable.

**Returns:**
java.lang.String - النص الخاص بوسم "(Multiple Items)"
### getTextOfOr() {#getTextOfOr--}
```
public String getTextOfOr()
```


يحصل على جميع السلاسل المنسقة محليًا لـ "or".

**Returns:**
java.lang.String -
### getTextOfProtectedName(String protectedName) {#getTextOfProtectedName-java.lang.String-}
```
public String getTextOfProtectedName(String protectedName)
```


يحصل على النص للاسم المحمي المحدد.

**Remarks**

في برنامج Ms Excel، لا يُسمح باستخدام بعض الأسماء كأسماء لحقول PivotFields في PivotTable. هي مختلفة حسب المنطقة، قد يحدد المستخدمها صراحةً وفقًا للمنطقة المستخدمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| protectedName | java.lang.String | الاسم المحمي في PivotTable. |

**Returns:**
java.lang.String - الأسماء المحمية المحلية لـ PivotTable.
### getTextOfProtection() {#getTextOfProtection--}
```
public String getTextOfProtection()
```


يحصل على اسم الحماية في PivotTable.

**Remarks**

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام طريقة PivotGlobalizationSettings.GetTextOfProtectedName(string). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.String - اسم الحماية لـ PivotTable
### getTextOfQuarters() {#getTextOfQuarters--}
```
public String getTextOfQuarters()
```


احصل على النص المحلي لـ "Quarters".

**Returns:**
java.lang.String -
### getTextOfRange() {#getTextOfRange--}
```
public String getTextOfRange()
```


يحصل على النص المحلي لـ "Range"

**Returns:**
java.lang.String -
### getTextOfRowLabels() {#getTextOfRowLabels--}
```
public String getTextOfRowLabels()
```


يحصل على نص التسمية "Row Labels" في جدول PivotTable.

**Returns:**
java.lang.String - النص الخاص بتسميات الصفوف
### getTextOfSeconds() {#getTextOfSeconds--}
```
public String getTextOfSeconds()
```


يحصل على النص المحلي لـ "Seconds"

**Returns:**
java.lang.String -
### getTextOfSubTotal(int subTotalType) {#getTextOfSubTotal-int-}
```
public String getTextOfSubTotal(int subTotalType)
```


يحصل على نص نوع [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) في جدول PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). ال [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |

**Returns:**
java.lang.String - النص الخاص بالنوع المعطى
### getTextOfTotal() {#getTextOfTotal--}
```
public String getTextOfTotal()
```


يحصل على النص الخاص بوسم "Total" في PivotTable. تحتاج إلى تجاوز هذه الطريقة عندما يحتوي PivotTable على حقلين PivotFields أو أكثر في منطقة البيانات.

**Returns:**
java.lang.String - النص الخاص بوسم "Total"
### getTextOfYears() {#getTextOfYears--}
```
public String getTextOfYears()
```


يحصل على النص المحلي لـ "Years".

**Returns:**
java.lang.String -
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




### setTextOfAll(String text) {#setTextOfAll-java.lang.String-}
```
public void setTextOfAll(String text)
```


يضبط نص التسمية "(All)" في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص مخصص |

### setTextOfColumnLabels(String text) {#setTextOfColumnLabels-java.lang.String-}
```
public void setTextOfColumnLabels(String text)
```


يحصل على نص التسمية "Column Labels" في جدول المحور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص تسميات الأعمدة |

### setTextOfDataFieldHeader(String text) {#setTextOfDataFieldHeader-java.lang.String-}
```
public void setTextOfDataFieldHeader(String text)
```


يضبط نص عنوان حقل منطقة القيمة في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص اسم رأس حقل البيانات |

### setTextOfEmptyData(String text) {#setTextOfEmptyData-java.lang.String-}
```
public void setTextOfEmptyData(String text)
```


يضبط نص التسمية "(blank)" في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص البيانات الفارغة |

### setTextOfGrandTotal(String text) {#setTextOfGrandTotal-java.lang.String-}
```
public void setTextOfGrandTotal(String text)
```


يضبط نص التسمية "Grand Total" في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص مخصص |

### setTextOfMultipleItems(String text) {#setTextOfMultipleItems-java.lang.String-}
```
public void setTextOfMultipleItems(String text)
```


يضبط نص التسمية "(Multiple Items)" في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص مخصص |

### setTextOfProtectedName(String protectedName, String text) {#setTextOfProtectedName-java.lang.String-java.lang.String-}
```
public void setTextOfProtectedName(String protectedName, String text)
```


يضبط النص لاسم محمي محدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| protectedName | java.lang.String | الاسم المحمي في PivotTable. |
| نص | java.lang.String | الأسماء المحلية المحمية لجدول PivotTable. |

### setTextOfRowLabels(String text) {#setTextOfRowLabels-java.lang.String-}
```
public void setTextOfRowLabels(String text)
```


يضبط نص التسمية "Row Labels" في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص تسميات الصفوف |

### setTextOfSubTotal(int subTotalType, String text) {#setTextOfSubTotal-int-java.lang.String-}
```
public void setTextOfSubTotal(int subTotalType, String text)
```


يضبط نص النوع [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| subTotalType | int | [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype). ال [PivotFieldSubtotalType](../../com.aspose.cells/pivotfieldsubtotaltype) |
| نص | java.lang.String | نص النوع المعطى |

### setTextOfTotal(String text) {#setTextOfTotal-java.lang.String-}
```
public void setTextOfTotal(String text)
```


يضبط نص التسمية "Total" في PivotTable.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص مخصص |

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

