---
title: "PivotFieldSortSetting"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الإعداد لفرز حقول pivot fields."
type: docs
url: /ar/java/com.aspose.cells/pivotfieldsortsetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotFieldSortSetting
```

يمثل الإعداد لفرز حقول pivot fields.

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
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Sort by the first data field ascending.
         rowField.sortBy(SortOrder.ASCENDING, 0, null);
 
         //Gets sort settings of the pivot field.
         PivotFieldSortSetting sortSetting = rowField.getSortSetting();
         System.out.println(sortSetting.getSortType());
         //do your business
 
         pivot.calculateData();
         book.save("out.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | يتم الفرز حسب القيم في أي صف أو عمود. |
| [getClass()](#getClass--) |  |
| [getFieldIndex()](#getFieldIndex--) | يمثل فهرس الحقل الذي يتم فرزه حسبه |
| [getLineTypeSortedBy()](#getLineTypeSortedBy--) | نوع سطر المحور الذي يتم فرزه حسبه. |
| [getSortBy()](#getSortBy--) | يمثل فهرس الحقل الذي يتم فرزه حسبه. |
| [getSortType()](#getSortType--) | يمثل الـ [SortOrder](../../com.aspose.cells/sortorder). |
| [hashCode()](#hashCode--) |  |
| [isSimpleSort()](#isSimpleSort--) | يشير إلى ما إذا كان سيتم تطبيق عملية فرز بيانات بسيطة. |
| [isSortByLabels()](#isSortByLabels--) | يشير إلى ما إذا كان سيتم فرز الحقل بنفسه أو بحقل البيانات. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFieldIndex(int value)](#setFieldIndex-int-) | يمثل فهرس الحقل الذي يتم فرزه حسبه |
| [setSimpleSort(boolean value)](#setSimpleSort-boolean-) | يشير إلى ما إذا كان سيتم تطبيق عملية فرز بيانات بسيطة. |
| [setSortBy(int value)](#setSortBy-int-) | يمثل فهرس الحقل الذي يتم فرزه حسبه. |
| [setSortType(int value)](#setSortType-int-) | يمثل الـ [SortOrder](../../com.aspose.cells/sortorder). |
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
### getCell() {#getCell--}
```
public String getCell()
```


يتم الفرز حسب القيم في أي صف أو عمود.

**Returns:**
java.lang.String
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


يمثل فهرس الحقل الذي يتم فرزه حسبه. -1 يعني فرز PivotField حسب التسميات، والقيم الأخرى تعني الفرز حسب حقل البيانات.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotFieldSortSetting.SortBy. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getLineTypeSortedBy() {#getLineTypeSortedBy--}
```
public int getLineTypeSortedBy()
```


نوع سطر المحور الذي يتم فرزه حسبه.

انظر إلى [PivotLineType](../../com.aspose.cells/pivotlinetype).

**Remarks**

يعمل فقط عندما لا يتم فرز هذا الحقل حسب التسميات.

**Returns:**
int
### getSortBy() {#getSortBy--}
```
public int getSortBy()
```


يمثل فهرس الحقل الذي يتم فرزه حسبه. قيمة -1 تشير إلى الفرز حسب قيم العنصر المحوري نفسه. عندما تكون القيمة أكبر من أو تساوي الصفر، فإنها تمثل فهرس حقل البيانات في منطقة البيانات.

**Returns:**
int
### getSortType() {#getSortType--}
```
public int getSortType()
```


يمثل الـ [SortOrder](../../com.aspose.cells/sortorder).

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isSimpleSort() {#isSimpleSort--}
```
public boolean isSimpleSort()
```


يشير إلى ما إذا كان سيتم تطبيق عملية فرز بيانات بسيطة.

**Remarks**

القيمة الافتراضية هي true.

**Returns:**
boolean
### isSortByLabels() {#isSortByLabels--}
```
public boolean isSortByLabels()
```


يشير إلى ما إذا كان سيتم فرز الحقل بنفسه أو بحقل البيانات.

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




### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


يمثل فهرس الحقل الذي يتم فرزه حسبه. -1 يعني فرز PivotField حسب التسميات، والقيم الأخرى تعني الفرز حسب حقل البيانات.

**Remarks**

ملاحظة: هذه الخاصية الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية PivotFieldSortSetting.SortBy. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ سبتمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSimpleSort(boolean value) {#setSimpleSort-boolean-}
```
public void setSimpleSort(boolean value)
```


يشير إلى ما إذا كان سيتم تطبيق عملية فرز بيانات بسيطة.

**Remarks**

القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setSortBy(int value) {#setSortBy-int-}
```
public void setSortBy(int value)
```


يمثل فهرس الحقل الذي يتم فرزه حسبه. قيمة -1 تشير إلى الفرز حسب قيم العنصر المحوري نفسه. عندما تكون القيمة أكبر من أو تساوي الصفر، فإنها تمثل فهرس حقل البيانات في منطقة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSortType(int value) {#setSortType-int-}
```
public void setSortType(int value)
```


يمثل الـ [SortOrder](../../com.aspose.cells/sortorder).

انظر إلى [SortOrder](../../com.aspose.cells/sortorder).

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

