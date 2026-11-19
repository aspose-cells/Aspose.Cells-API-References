---
title: "PivotFilter"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل PivotFilter في مجموعة PivotFilter."
type: docs
url: /ar/java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

يمثل PivotFilter في مجموعة PivotFilter.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Add top 10 filter
          pivot.getBaseFields().get(0).filterTop10(0, PivotFilterType.COUNT,false,2);
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | يحصل على الفلتر التلقائي للـ pivot filter. |
| [getClass()](#getClass--) |  |
| [getDateTimeValues()](#getDateTimeValues--) | يحصل على قيم الفلتر الرقمي. |
| [getEvaluationOrder()](#getEvaluationOrder--) | يحصل على ترتيب التقييم للـ pivot filter. |
| [getFieldIndex()](#getFieldIndex--) | يحصل على فهرس حقل المصدر الذي يُطبق عليه هذا الـ pivot filter. |
| [getFilterCategory()](#getFilterCategory--) | يحصل على فئة هذا الفلتر. |
| [getFilterType()](#getFilterType--) | يحصل على نوع الفلتر للـ pivot filter. |
| [getLabels()](#getLabels--) | يحصل على تسميات فلتر العنوان. |
| [getMeasureCubeFieldIndex()](#getMeasureCubeFieldIndex--) | يحدد فهرس حقل مكعب القياس. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | يحصل على فهرس حقل القياس للـ pivot filter. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | يحصل على فهرس حقل خاصية العضو للـ pivot filter. |
| [getName()](#getName--) | يحصل على اسم الـ pivot filter. |
| [getNumberValues()](#getNumberValues--) | يحصل على قيم الفلتر الرقمي. |
| [getTop10Value()](#getTop10Value--) | يحصل على إعداد أعلى 10 للفلتر. |
| [getUseWholeDay()](#getUseWholeDay--) | يشير إلى ما إذا كان يجب استخدام أيام كاملة في معايير تصفية التاريخ. |
| [getValue1()](#getValue1--) | يحصل على القيمة النصية value1 لفلتر التسمية pivot. |
| [getValue2()](#getValue2--) | يحصل على القيمة النصية value2 لفلتر التسمية pivot. |
| [getValueFieldIndex()](#getValueFieldIndex--) | يحصل على فهرس حقل القيمة في منطقة القيمة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | يحصل على ترتيب التقييم للـ pivot filter. |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | يحصل على فهرس حقل القياس للـ pivot filter. |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | يحصل على فهرس حقل خاصية العضو للـ pivot filter. |
| [setName(String value)](#setName-java.lang.String-) | يحصل على اسم الـ pivot filter. |
| [setUseWholeDay(boolean value)](#setUseWholeDay-boolean-) | يشير إلى ما إذا كان يجب استخدام أيام كاملة في معايير تصفية التاريخ. |
| [setValue1(String value)](#setValue1-java.lang.String-) | يحصل على القيمة النصية value1 لفلتر التسمية pivot. |
| [setValue2(String value)](#setValue2-java.lang.String-) | يحصل على القيمة النصية value2 لفلتر التسمية pivot. |
| [setValueFieldIndex(int value)](#setValueFieldIndex-int-) | يحصل على فهرس حقل القيمة في منطقة القيمة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


يحصل على الفلتر التلقائي للـ pivot filter.

**Remarks**

ملاحظة: هذه الطريقة أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة FilterLabel أو FilterValue أو FilterDate أو FilterTop10. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDateTimeValues() {#getDateTimeValues--}
```
public DateTime[] getDateTimeValues()
```


يحصل على قيم الفلتر الرقمي.

**Returns:**
com.aspose.cells.DateTime[] -
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


يحصل على ترتيب التقييم للـ pivot filter.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


يحصل على فهرس حقل المصدر الذي يُطبق عليه هذا الـ pivot filter.

**Returns:**
int
### getFilterCategory() {#getFilterCategory--}
```
public int getFilterCategory()
```


يحصل على فئة هذا الفلتر.

انظر [FilterCategory](../../com.aspose.cells/filtercategory).

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


يحصل على نوع الفلتر للـ pivot filter.

انظر [PivotFilterType](../../com.aspose.cells/pivotfiltertype).

**Returns:**
int
### getLabels() {#getLabels--}
```
public String[] getLabels()
```


يحصل على تسميات فلتر العنوان.

**Returns:**
java.lang.String[] -
### getMeasureCubeFieldIndex() {#getMeasureCubeFieldIndex--}
```
public int getMeasureCubeFieldIndex()
```


يحدد فهرس حقل مكعب القياس. تُستخدم هذه الخاصية فقط بواسطة عوامل التصفية في محاور OLAP وتحدد على أي قياس يجب تطبيق مرشح القيمة.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


يحصل على فهرس حقل القياس للـ pivot filter.

**Remarks**

ملاحظة: هذه الطريقة الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotFilter.ValueFieldIndex. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


يحصل على فهرس حقل خاصية العضو للـ pivot filter.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الـ pivot filter.

**Returns:**
java.lang.String
### getNumberValues() {#getNumberValues--}
```
public double[] getNumberValues()
```


يحصل على قيم الفلتر الرقمي.

**Returns:**
double[] -
### getTop10Value() {#getTop10Value--}
```
public Top10Filter getTop10Value()
```


يحصل على إعداد أعلى 10 للفلتر.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### getUseWholeDay() {#getUseWholeDay--}
```
public boolean getUseWholeDay()
```


يشير إلى ما إذا كان يجب استخدام أيام كاملة في معايير تصفية التاريخ.

**Returns:**
boolean
### getValue1() {#getValue1--}
```
public String getValue1()
```


يحصل على القيمة النصية value1 لفلتر التسمية pivot.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


يحصل على القيمة النصية value2 لفلتر التسمية pivot.

**Returns:**
java.lang.String
### getValueFieldIndex() {#getValueFieldIndex--}
```
public int getValueFieldIndex()
```


يحصل على فهرس حقل القيمة في منطقة القيمة.

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




### setEvaluationOrder(int value) {#setEvaluationOrder-int-}
```
public void setEvaluationOrder(int value)
```


يحصل على ترتيب التقييم للـ pivot filter.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


يحصل على فهرس حقل القياس للـ pivot filter.

**Remarks**

ملاحظة: هذه الطريقة الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotFilter.ValueFieldIndex. سيتم إزالة هذه الطريقة بعد 12 شهرًا اعتبارًا من نوفمبر 2024. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


يحصل على فهرس حقل خاصية العضو للـ pivot filter.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يحصل على اسم الـ pivot filter.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setUseWholeDay(boolean value) {#setUseWholeDay-boolean-}
```
public void setUseWholeDay(boolean value)
```


يشير إلى ما إذا كان يجب استخدام أيام كاملة في معايير تصفية التاريخ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


يحصل على القيمة النصية value1 لفلتر التسمية pivot.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


يحصل على القيمة النصية value2 لفلتر التسمية pivot.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setValueFieldIndex(int value) {#setValueFieldIndex-int-}
```
public void setValueFieldIndex(int value)
```


يحصل على فهرس حقل القيمة في منطقة القيمة.

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

