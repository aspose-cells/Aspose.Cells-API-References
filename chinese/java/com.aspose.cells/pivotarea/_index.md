---
title: "PivotArea"
second_title: "Aspose.Cells for Java API 参考"
description: "呈现数据透视表的选定区域。"
type: docs
url: /zh/java/com.aspose.cells/pivotarea/
---

**Inheritance:**
java.lang.Object
```
public class PivotArea
```

呈现数据透视表的选定区域。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | 呈现 PivotTable 的选定区域。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | 获取此规则适用的 PivotTable 区域。 |
| [getCellAreas()](#getCellAreas--) | 获取此 PivotArea 的单元格区域。 |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | 获取此 PivotArea 的所有筛选器。 |
| [getOnlyData()](#getOnlyData--) | 指示是否仅选择项目选择的数据值（视图的数据区域），且不包括项目标签。 |
| [getOnlyLabel()](#getOnlyLabel--) | 指示是否仅选择项目选择的数据标签。 |
| [getRuleType()](#getRuleType--) | 获取选择规则的类型。 |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | 指示是否包括列总计。 |
| [isOutline()](#isOutline--) | 指示规则是否引用处于大纲模式的区域。 |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | 指示是否包括行总计。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | 选择带有筛选器的区域。 |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | 将区域中的字段选择为区域。 |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | 将区域中的字段选择为区域。 |
| [setAxisType(int value)](#setAxisType-int-) | 设置此规则适用的 PivotTable 区域。 |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | 指示是否包括列总计。 |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | 指示是否仅选择项目选择的数据值（视图的数据区域），且不包括项目标签。 |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | 指示是否仅选择项目选择的数据标签。 |
| [setOutline(boolean value)](#setOutline-boolean-) | 指示规则是否引用处于大纲模式的区域。 |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | 指示是否包括行总计。 |
| [setRuleType(int value)](#setRuleType-int-) | 设置选择规则的类型。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```


呈现 PivotTable 的选定区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |

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
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```


获取此规则适用的 PivotTable 区域。

请参阅 [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。

**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```


获取此 PivotArea 的单元格区域。

**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilters() {#getFilters--}
```
public PivotAreaFilterCollection getFilters()
```


获取此 PivotArea 的所有筛选器。

**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```


指示是否仅选择项目选择的数据值（视图的数据区域），且不包括项目标签。

**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```


指示是否仅选择项目选择的数据标签。

**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```


获取选择规则的类型。

查看 [PivotAreaType](../../com.aspose.cells/pivotareatype)。

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isColumnGrandIncluded() {#isColumnGrandIncluded--}
```
public boolean isColumnGrandIncluded()
```


指示是否包括列总计。

**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```


指示规则是否引用处于大纲模式的区域。

**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```


指示是否包括行总计。

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




### select(int axisType, int fieldPosition, int selectionType) {#select-int-int-int-}
```
public void select(int axisType, int fieldPosition, int selectionType)
```


选择带有筛选器的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。此规则适用于 PivotTable 的区域。 |
| fieldPosition | int | 此规则适用的轴内字段的位置。 |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype)。指定在结构化选择期间可以在 PivotTable 中选择的内容。 |

### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```


将区域中的字段选择为区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。区域类型。 |
| field | [PivotField](../../com.aspose.cells/pivotfield) | 透视字段。 |

### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```


将区域中的字段选择为区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。区域类型。 |
| fieldName | java.lang.String | 透视字段的名称。 |

### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```


设置此规则适用的 PivotTable 区域。

请参阅 [PivotFieldType](../../com.aspose.cells/pivotfieldtype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```


指示是否包括列总计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```


指示是否仅选择项目选择的数据值（视图的数据区域），且不包括项目标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```


指示是否仅选择项目选择的数据标签。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```


指示规则是否引用处于大纲模式的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```


指示是否包括行总计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```


设置选择规则的类型。

查看 [PivotAreaType](../../com.aspose.cells/pivotareatype)。

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

