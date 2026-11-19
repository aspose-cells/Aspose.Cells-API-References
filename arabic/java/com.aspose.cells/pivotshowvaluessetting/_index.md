---
title: "PivotShowValuesSetting"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الإعدادات المتعلقة بإظهار القيم كـ عندما يكون حساب ShowDataAs قيد الاستخدام."
type: docs
url: /ar/java/com.aspose.cells/pivotshowvaluessetting/
---

**Inheritance:**
java.lang.Object
```
public class PivotShowValuesSetting
```

يمثل الإعدادات المتعلقة بإظهار القيم كـ عندما يكون حساب ShowDataAs قيد الاستخدام.

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
 
         PivotField dataField = pivot.getDataFields().get(0);
         // Display value as percentage of the grand total
         dataField.showValuesAs(PivotShowValuesAsType.PERCENTAGE_OF_TOTAL, 0, PivotShowValuesSetting.NEXT_PIVOT_ITEM);
         // Get the display calculation setting of data field
         PivotShowValuesSetting settings = dataField.getShowValuesSetting();
         System.out.println(settings.getShowValuesAs());
 
          pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## حقول

| حقل | الوصف |
| --- | --- |
| [NEXT_PIVOT_ITEM](#NEXT-PIVOT-ITEM) | فهرس العنصر الأساسي الخاص: استخدم العنصر المحوري التالي. |
| [PREVIOUS_PIVOT_ITEM](#PREVIOUS-PIVOT-ITEM) | فهرس العنصر الأساسي الخاص: استخدم العنصر المحوري السابق. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBaseFieldIndex()](#getBaseFieldIndex--) | يمثل الحقل الأساسي لحساب ShowDataAs عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [getBaseFieldName()](#getBaseFieldName--) | يحصل على تسمية الحقل الأساسي للمحور. |
| [getBaseItemCaption()](#getBaseItemCaption--) | يحصل على تسمية العنصر المحوري في الحقل الأساسي. |
| [getBaseItemIndex()](#getBaseItemIndex--) | يمثل الفهرس المخصص للعنصر المحوري في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [getBaseItemPositionType()](#getBaseItemPositionType--) | يمثل نوع العنصر الأساسي للبيفوت في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [getCalculationType()](#getCalculationType--) | يمثل طريقة عرض قيم حقل البيانات في تقرير البيفوت. |
| [getClass()](#getClass--) |  |
| [getShowValuesAs()](#getShowValuesAs--) | يحصل على طريقة عرض قيم حقل البيانات في تقرير البيفوت. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBaseFieldIndex(int value)](#setBaseFieldIndex-int-) | يمثل الحقل الأساسي لحساب ShowDataAs عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [setBaseItemIndex(int value)](#setBaseItemIndex-int-) | يمثل الفهرس المخصص للعنصر المحوري في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [setBaseItemPositionType(int value)](#setBaseItemPositionType-int-) | يمثل نوع العنصر الأساسي للبيفوت في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام. |
| [setCalculationType(int value)](#setCalculationType-int-) | يمثل طريقة عرض قيم حقل البيانات في تقرير البيفوت. |
| [setShowValuesAs(int value)](#setShowValuesAs-int-) | يضبط طريقة عرض قيم حقل البيانات في تقرير البيفوت. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### NEXT_PIVOT_ITEM {#NEXT-PIVOT-ITEM}
```
public static final int NEXT_PIVOT_ITEM
```


فهرس العنصر الأساسي الخاص: استخدم عنصر البيفوت التالي. صالح لحسابات \"Show Values As\"؛ ساري في Excel 2010 وما بعده.

### PREVIOUS_PIVOT_ITEM {#PREVIOUS-PIVOT-ITEM}
```
public static final int PREVIOUS_PIVOT_ITEM
```


فهرس العنصر الأساسي الخاص: استخدم عنصر البيفوت السابق. صالح لحسابات \"Show Values As\"؛ ساري في Excel 2010 وما بعده.

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
### getBaseFieldIndex() {#getBaseFieldIndex--}
```
public int getBaseFieldIndex()
```


يمثل الحقل الأساسي لحساب ShowDataAs عندما يكون حساب ShowDataAs قيد الاستخدام.

**Returns:**
int
### getBaseFieldName() {#getBaseFieldName--}
```
public String getBaseFieldName()
```


يحصل على تسمية الحقل الأساسي للمحور.

**Returns:**
java.lang.String
### getBaseItemCaption() {#getBaseItemCaption--}
```
public String getBaseItemCaption()
```


يحصل على تسمية العنصر المحوري في الحقل الأساسي.

**Returns:**
java.lang.String
### getBaseItemIndex() {#getBaseItemIndex--}
```
public int getBaseItemIndex()
```


يمثل الفهرس المخصص للعنصر المحوري في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Returns:**
int
### getBaseItemPositionType() {#getBaseItemPositionType--}
```
public int getBaseItemPositionType()
```


يمثل نوع العنصر الأساسي للبيفوت في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام. لأن PivotItemPosition.Custom مخصص للقراءة فقط، إذا كنت بحاجة إلى تعيين PivotItemPosition.Custom، يرجى تعيين سمة PivotField.BaseItemIndex.

انظر [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotShowValuesSetting.BaseItem. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getCalculationType() {#getCalculationType--}
```
public int getCalculationType()
```


يمثل طريقة عرض قيم حقل البيانات في تقرير البيفوت.

انظر [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotShowValuesSetting.ShowValuesAs. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getShowValuesAs() {#getShowValuesAs--}
```
public int getShowValuesAs()
```


يحصل على طريقة عرض قيم حقل البيانات في تقرير البيفوت.

انظر [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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




### setBaseFieldIndex(int value) {#setBaseFieldIndex-int-}
```
public void setBaseFieldIndex(int value)
```


يمثل الحقل الأساسي لحساب ShowDataAs عندما يكون حساب ShowDataAs قيد الاستخدام.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBaseItemIndex(int value) {#setBaseItemIndex-int-}
```
public void setBaseItemIndex(int value)
```


يمثل الفهرس المخصص للعنصر المحوري في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام.

**Remarks**

[PREVIOUS\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#PREVIOUS-PIVOT-ITEM) (-1) for the preceding item, [NEXT\_PIVOT\_ITEM](../../com.aspose.cells/pivotshowvaluessetting\#NEXT-PIVOT-ITEM) (-2) for the succeeding item; non\\u9225\\u6182egative values denote the ordinal index of a specific pivot item.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBaseItemPositionType(int value) {#setBaseItemPositionType-int-}
```
public void setBaseItemPositionType(int value)
```


يمثل نوع العنصر الأساسي للبيفوت في الحقل الأساسي عندما يكون حساب ShowDataAs قيد الاستخدام. لأن PivotItemPosition.Custom مخصص للقراءة فقط، إذا كنت بحاجة إلى تعيين PivotItemPosition.Custom، يرجى تعيين سمة PivotField.BaseItemIndex.

انظر [PivotItemPositionType](../../com.aspose.cells/pivotitempositiontype).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotShowValuesSetting.BaseItem. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCalculationType(int value) {#setCalculationType-int-}
```
public void setCalculationType(int value)
```


يمثل طريقة عرض قيم حقل البيانات في تقرير البيفوت.

انظر [PivotFieldDataDisplayFormat](../../com.aspose.cells/pivotfielddatadisplayformat).

**Remarks**

ملاحظة: هذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام خاصية PivotShowValuesSetting.ShowValuesAs. سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ نوفمبر 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShowValuesAs(int value) {#setShowValuesAs-int-}
```
public void setShowValuesAs(int value)
```


يضبط طريقة عرض قيم حقل البيانات في تقرير البيفوت.

انظر [PivotShowValuesAsType](../../com.aspose.cells/pivotshowvaluesastype).

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

