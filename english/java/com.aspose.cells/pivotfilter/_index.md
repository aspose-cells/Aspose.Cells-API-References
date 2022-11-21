---
title: PivotFilter
second_title: Aspose.Cells for Java API Reference
description: Represents a PivotFilter in PivotFilter Collection.
type: docs
weight: 401
url: /java/com.aspose.cells/pivotfilter/
---

**Inheritance:**
java.lang.Object
```
public class PivotFilter
```

Represents a PivotFilter in PivotFilter Collection.

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
 
         int pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable");
         PivotTable pivot = pivots.get(pivotIndex);
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Add PivotFilter
         int index = pivot.getPivotFilters().add(0, PivotFilterType.COUNT);
         PivotFilter filter = pivot.getPivotFilters().get(index);
         filter.getAutoFilter().filterTop10(0, false, false, 2);
 
         pivot.refreshData();
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFilter()](#getAutoFilter--) | Gets the autofilter of the pivot filter. |
| [getClass()](#getClass--) |  |
| [getEvaluationOrder()](#getEvaluationOrder--) | Gets the Evaluation Order of the pivot filter. |
| [getFieldIndex()](#getFieldIndex--) | Gets the field index of the pivot filter. |
| [getFilterType()](#getFilterType--) | Gets the autofilter type of the pivot filter. |
| [getMeasureFldIndex()](#getMeasureFldIndex--) | Gets the measure field index of the pivot filter. |
| [getMemberPropertyFieldIndex()](#getMemberPropertyFieldIndex--) | Gets the member property field index of the pivot filter. |
| [getName()](#getName--) | Gets the name of the pivot filter. |
| [getValue1()](#getValue1--) | Gets the string value1 of the label pivot filter. |
| [getValue2()](#getValue2--) | Gets the string value2 of the label pivot filter. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setEvaluationOrder(int value)](#setEvaluationOrder-int-) | For the description of this property, please see [getEvaluationOrder()](../../com.aspose.cells/pivotfilter\#getEvaluationOrder--) |
| [setMeasureFldIndex(int value)](#setMeasureFldIndex-int-) | For the description of this property, please see [getMeasureFldIndex()](../../com.aspose.cells/pivotfilter\#getMeasureFldIndex--) |
| [setMemberPropertyFieldIndex(int value)](#setMemberPropertyFieldIndex-int-) | For the description of this property, please see [getMemberPropertyFieldIndex()](../../com.aspose.cells/pivotfilter\#getMemberPropertyFieldIndex--) |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see [getName()](../../com.aspose.cells/pivotfilter\#getName--) |
| [setValue1(String value)](#setValue1-java.lang.String-) | For the description of this property, please see [getValue1()](../../com.aspose.cells/pivotfilter\#getValue1--) |
| [setValue2(String value)](#setValue2-java.lang.String-) | For the description of this property, please see [getValue2()](../../com.aspose.cells/pivotfilter\#getValue2--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAutoFilter() {#getAutoFilter--}
```
public AutoFilter getAutoFilter()
```


Gets the autofilter of the pivot filter.

**Returns:**
[AutoFilter](../../com.aspose.cells/autofilter)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEvaluationOrder() {#getEvaluationOrder--}
```
public int getEvaluationOrder()
```


Gets the Evaluation Order of the pivot filter.

**Returns:**
int
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


Gets the field index of the pivot filter.

**Returns:**
int
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


Gets the autofilter type of the pivot filter.

**Returns:**
int
### getMeasureFldIndex() {#getMeasureFldIndex--}
```
public int getMeasureFldIndex()
```


Gets the measure field index of the pivot filter.

**Returns:**
int
### getMemberPropertyFieldIndex() {#getMemberPropertyFieldIndex--}
```
public int getMemberPropertyFieldIndex()
```


Gets the member property field index of the pivot filter.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Gets the name of the pivot filter.

**Returns:**
java.lang.String
### getValue1() {#getValue1--}
```
public String getValue1()
```


Gets the string value1 of the label pivot filter.

**Returns:**
java.lang.String
### getValue2() {#getValue2--}
```
public String getValue2()
```


Gets the string value2 of the label pivot filter.

**Returns:**
java.lang.String
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


For the description of this property, please see [getEvaluationOrder()](../../com.aspose.cells/pivotfilter\#getEvaluationOrder--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMeasureFldIndex(int value) {#setMeasureFldIndex-int-}
```
public void setMeasureFldIndex(int value)
```


For the description of this property, please see [getMeasureFldIndex()](../../com.aspose.cells/pivotfilter\#getMeasureFldIndex--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMemberPropertyFieldIndex(int value) {#setMemberPropertyFieldIndex-int-}
```
public void setMemberPropertyFieldIndex(int value)
```


For the description of this property, please see [getMemberPropertyFieldIndex()](../../com.aspose.cells/pivotfilter\#getMemberPropertyFieldIndex--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


For the description of this property, please see [getName()](../../com.aspose.cells/pivotfilter\#getName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setValue1(String value) {#setValue1-java.lang.String-}
```
public void setValue1(String value)
```


For the description of this property, please see [getValue1()](../../com.aspose.cells/pivotfilter\#getValue1--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setValue2(String value) {#setValue2-java.lang.String-}
```
public void setValue2(String value)
```


For the description of this property, please see [getValue2()](../../com.aspose.cells/pivotfilter\#getValue2--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

