---
title: "PivotConditionalFormat"
second_title: "Aspose.Cells for Java API 参考"
description: "表示数据透视表的条件格式。"
type: docs
url: /zh/java/com.aspose.cells/pivotconditionalformat/
---

**Inheritance:**
java.lang.Object
```
public class PivotConditionalFormat
```

表示数据透视表的条件格式。

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
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
 
 
         //do your business
 
          pivot.calculateData();
 
         book.save("out.xlsx");
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addCellArea(CellArea ca)](#addCellArea-com.aspose.cells.CellArea-) | 基于数据透视表视图添加一个区域。 |
| [addFieldArea(int axisType, PivotField field)](#addFieldArea-int-com.aspose.cells.PivotField-) | 添加数据透视字段的区域。 |
| [addFieldArea(int axisType, String fieldName)](#addFieldArea-int-java.lang.String-) | 添加数据透视字段的区域。 |
| [applyTo(int row, int column, int scope)](#applyTo-int-int-int-) | 将条件格式应用于必须位于数据区域的范围。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellAreas()](#getCellAreas--) | 获取此条件格式适用的所有单元格区域。 |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | 获取数据透视表条件格式的条件。 |
| [getPivotAreas()](#getPivotAreas--) | 获取所有数据透视区域。 |
| [getRuleType()](#getRuleType--) | 获取数据透视表条件格式的规则类型。 |
| [getScopeType()](#getScopeType--) | 获取数据透视表条件格式的作用域类型。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRuleType(int value)](#setRuleType-int-) | 设置数据透视表条件格式的规则类型。 |
| [setScopeType(int value)](#setScopeType-int-) | 设置数据透视表条件格式的作用域类型。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCellArea(CellArea ca) {#addCellArea-com.aspose.cells.CellArea-}
```
public void addCellArea(CellArea ca)
```


基于数据透视表视图添加一个区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 单元格区域。 |

### addFieldArea(int axisType, PivotField field) {#addFieldArea-int-com.aspose.cells.PivotField-}
```
public void addFieldArea(int axisType, PivotField field)
```


添加数据透视字段的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。区域类型。 |
| field | [PivotField](../../com.aspose.cells/pivotfield) | 透视字段。 |

### addFieldArea(int axisType, String fieldName) {#addFieldArea-int-java.lang.String-}
```
public void addFieldArea(int axisType, String fieldName)
```


添加数据透视字段的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。区域类型。 |
| fieldName | java.lang.String | 透视字段的名称。 |

### applyTo(int row, int column, int scope) {#applyTo-int-int-int-}
```
public void applyTo(int row, int column, int scope)
```


将条件格式应用于必须位于数据区域的范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 选定的行。 |
| 列 | int | 选定的列。 |
| scope | int | [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype). 范围 |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


获取此条件格式适用的所有单元格区域。

**Returns:**
com.aspose.cells.CellArea[] -
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


获取数据透视表条件格式的条件。

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getPivotAreas() {#getPivotAreas--}
```
public PivotAreaCollection getPivotAreas()
```


获取所有数据透视区域。

**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


获取数据透视表条件格式的规则类型。

参见 [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```


获取数据透视表条件格式的作用域类型。

参见 [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

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




### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


设置数据透视表条件格式的规则类型。

参见 [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```


设置数据透视表条件格式的作用域类型。

参见 [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

