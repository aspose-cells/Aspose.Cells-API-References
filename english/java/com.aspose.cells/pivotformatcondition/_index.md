---
title: PivotFormatCondition
second_title: Aspose.Cells for Java API Reference
description: Represents a PivotTable Format Condition in PivotFormatCondition Collection.
type: docs
url: /java/com.aspose.cells/pivotformatcondition/
---

**Inheritance:**
java.lang.Object
```
public class PivotFormatCondition
```

Represents a PivotTable Format Condition in PivotFormatCondition Collection.

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
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getPivotFormatConditions().add();
         PivotFormatCondition pfc = pivot.getPivotFormatConditions().get(formatIndex);
         FormatConditionCollection fcc = pfc.getFormatConditions();
         fcc.addArea(pivot.getDataBodyRange());
         int idx = fcc.addCondition(FormatConditionType.CELL_VALUE);
         FormatCondition fc = fcc.get(idx);
         fc.setFormula1("100");
         fc.setOperator(OperatorType.GREATER_OR_EQUAL);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.refreshData();
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Methods

| Method | Description |
| --- | --- |
| [addColumnAreaCondition(PivotField columnField)](#addColumnAreaCondition-com.aspose.cells.PivotField-) | Adds PivotTable conditional format limit in the column fields. |
| [addColumnAreaCondition(String fieldName)](#addColumnAreaCondition-java.lang.String-) | Adds PivotTable conditional format limit in the column fields. |
| [addDataAreaCondition(PivotField dataField)](#addDataAreaCondition-com.aspose.cells.PivotField-) | Adds PivotTable conditional format limit in the data fields. |
| [addDataAreaCondition(String fieldName)](#addDataAreaCondition-java.lang.String-) | Adds PivotTable conditional format limit in the data fields. |
| [addRowAreaCondition(PivotField rowField)](#addRowAreaCondition-com.aspose.cells.PivotField-) | Adds PivotTable conditional format limit in the row fields. |
| [addRowAreaCondition(String fieldName)](#addRowAreaCondition-java.lang.String-) | Adds PivotTable conditional format limit in the row fields. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Get formatconditions for the pivot table condition format . |
| [getRuleType()](#getRuleType--) | Gets rule type for the pivot table condition format . |
| [getScopeType()](#getScopeType--) | Gets scope type for the pivot table condition format . |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setConditionalAreas()](#setConditionalAreas--) | Sets conditional areas of PivotFormatCondition object. |
| [setRuleType(int value)](#setRuleType-int-) | Sets rule type for the pivot table condition format . |
| [setScopeType(int value)](#setScopeType-int-) | Sets scope type for the pivot table condition format . |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColumnAreaCondition(PivotField columnField) {#addColumnAreaCondition-com.aspose.cells.PivotField-}
```
public void addColumnAreaCondition(PivotField columnField)
```


Adds PivotTable conditional format limit in the column fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in the column fields. |

### addColumnAreaCondition(String fieldName) {#addColumnAreaCondition-java.lang.String-}
```
public void addColumnAreaCondition(String fieldName)
```


Adds PivotTable conditional format limit in the column fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | The name of PivotField. |

### addDataAreaCondition(PivotField dataField) {#addDataAreaCondition-com.aspose.cells.PivotField-}
```
public void addDataAreaCondition(PivotField dataField)
```


Adds PivotTable conditional format limit in the data fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in the data fields. |

### addDataAreaCondition(String fieldName) {#addDataAreaCondition-java.lang.String-}
```
public void addDataAreaCondition(String fieldName)
```


Adds PivotTable conditional format limit in the data fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | The name of PivotField. |

### addRowAreaCondition(PivotField rowField) {#addRowAreaCondition-com.aspose.cells.PivotField-}
```
public void addRowAreaCondition(PivotField rowField)
```


Adds PivotTable conditional format limit in the row fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowField | [PivotField](../../com.aspose.cells/pivotfield) | The PivotField in the row fields. |

### addRowAreaCondition(String fieldName) {#addRowAreaCondition-java.lang.String-}
```
public void addRowAreaCondition(String fieldName)
```


Adds PivotTable conditional format limit in the row fields.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | java.lang.String | The name of PivotField. |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```


Get formatconditions for the pivot table condition format .

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


Gets rule type for the pivot table condition format .

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


Gets scope type for the pivot table condition format .

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




### setConditionalAreas() {#setConditionalAreas--}
```
public void setConditionalAreas()
```


Sets conditional areas of PivotFormatCondition object.

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


Sets rule type for the pivot table condition format .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


Sets scope type for the pivot table condition format .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

