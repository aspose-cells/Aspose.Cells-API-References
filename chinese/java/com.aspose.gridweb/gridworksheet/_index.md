---
title: "GridWorksheet"
second_title: "Aspose.Cells for Java API 参考"
description: "封装表示单个工作表的对象。"
type: docs
url: /zh/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

封装表示单个工作表的对象。
## 方法

| 方法 | 描述 |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | 设置指定自动筛选适用的范围。 |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | 为指定行添加自定义过滤器。 |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | 自动调整列宽。 |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | 自动调整列宽。 |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | 自动调整行高。 |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | 自动调整行高。 |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | 在矩形范围内自动调整行高。 |
| [autoFitRows()](#autoFitRows--) | 自动调整此工作表中所有行的高度。 |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | 自动调整此工作表中所有行的高度。 |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | 在范围内自动调整行高。 |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | 计算一个公式。 |
| [clearComments()](#clearComments--) | 清除设计器电子表格中的所有批注。 |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | 复制来自另一个工作表的内容和格式。 |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | 在工作表中创建小计。 |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | 在工作表中创建小计。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | 为列设置过滤器。注意，我们应在调用 filterString 之前调用 AddAutoFilter。过滤条件字符串。注意我们使用逗号 -> \",\" 作为分隔符，因此要过滤的单元格值不能包含逗号。filterString(10,\"123,456\") 表示第 10 列应包含 123 或 456，filterString(10,\"123\") 表示第 10 列应包含 123。列索引值使用逗号分隔，例如 123,456,789 或 abc |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | 在工作表中指定的单元格处冻结窗格。 |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | 在工作表中指定的单元格处冻结窗格。 |
| [getActiveCell()](#getActiveCell--) | 获取工作表中的活动单元格。 |
| [getBackgroundImage()](#getBackgroundImage--) | 获取工作表的背景图像。 |
| [getCells()](#getCells--) | 获取 [GridCell](../../com.aspose.gridweb/gridcell) 集合。 |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | 表示工作表代码名称。 |
| [getColumnCaption(int column)](#getColumnCaption-int-) | 获取列标题。 |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | 获取列标题的工具提示文本。 |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | 获取列是否为只读。 |
| [getComments()](#getComments--) | 获取 [GridComment](../../com.aspose.gridweb/gridcomment) 集合。 |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | 指示指定的工作表是从右向左显示还是从左向右显示。 |
| [getDisplayZeros()](#getDisplayZeros--) | 如果显示零值，则为 True。 |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | 表示第一个可见列的索引。 |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | 表示第一个可见行的索引。 |
| [getFreezedPanes()](#getFreezedPanes--) | 获取冻结窗格。 |
| [getGridActiveCell()](#getGridActiveCell--) | 获取工作表中的活动单元格。 |
| [getHyperlinks()](#getHyperlinks--) | 获取 [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection) 集合。 |
| [getIndex()](#getIndex--) | 获取工作表集合中工作表的索引。 |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | 获取单元格是否为只读。这是 GridWeb 的扩展属性，实际 Excel 文件中不会保留。 |
| [getName()](#getName--) | 获取工作表的名称。 |
| [getOutlineShown()](#getOutlineShown--) | 指示是否显示大纲。 |
| [getPictures()](#getPictures--) | 获取一个 [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) 集合。 |
| [getPivotTables()](#getPivotTables--) | 获取工作表中的数据透视表。 |
| [getRowCaption(int row)](#getRowCaption-int-) | 获取行标题。 |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | 获取行标题的工具提示文本。 |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | 获取行是否为只读。 |
| [getSelected()](#getSelected--) | 指示打开工作簿时是否选中此工作表。 |
| [getShapes()](#getShapes--) | 获取一个 [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) 集合。 |
| [getStandardHeight()](#getStandardHeight--) | 获取此工作表中默认的行高，单位为点。 |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | 获取此工作表中默认的行高，单位为像素。 |
| [getTabColor()](#getTabColor--) | 表示工作表选项卡颜色。 |
| [getUniqueID()](#getUniqueID--) | 获取控件中的唯一标识符。 |
| [getValidations()](#getValidations--) | 获取工作表中的数据验证设置集合。 |
| [getVisible()](#getVisible--) | 指示此工作表的名称是否显示在控件的工作表标签中。 |
| [getWorkbook()](#getWorkbook--) | 获取工作表集合的 [GridWorkbook](../../com.aspose.gridweb/gridworkbook) 对象。 |
| [getZoom()](#getZoom--) | 表示以百分比计的缩放因子。 |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | 对行进行分组。 |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | 获取一个值，指示网格线是否可见。默认值为 true。 |
| [isProtected()](#isProtected--) | 指示工作表是否受保护。 |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | 指示在大纲中汇总行是否会位于明细行的下方。 |
| [moveTo(int index)](#moveTo-int-) | 将工作表移动到电子表格中的其他位置。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | 刷新自动筛选以隐藏或显示行。 |
| [removeAutoFilter()](#removeAutoFilter--) | 移除工作表的自动筛选。 |
| [removeSubtotal()](#removeSubtotal--) | 移除工作表中由 CreateSubtotal 方法创建的小计。 |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | 要应用的字段的整数偏移量，基于第一个筛选列（从列表左侧开始；最左侧的字段为字段 0）。 |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | 设置工作表中的活动单元格。 |
| [setAllCellsEditable()](#setAllCellsEditable--) | 使所有单元格可编辑。这是扩展属性。 |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | 使所有单元格只读。这是扩展属性，注意此属性在实际单元格中无法保留，如果想保持保护，请使用 setProtect。 |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | 设置工作表的背景图像。 |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | 设置列的标题。请注意，这是一个扩展属性，不能保存在 Excel 文件中。 |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | 设置列标题的工具提示文本。 |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | 将列设为只读，以便用户无法从客户端删除它。 |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | 指示指定的工作表是从右向左显示还是从左向右显示。 |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | 如果显示零值，则为 True。 |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | 使一组单元格可编辑。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 通过调用 SetAllCellsReadonly 方法将所有单元格设为只读。 |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | 表示第一个可见列的索引。 |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | 表示第一个可见行的索引。 |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | 设置工作表中的活动单元格。 |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | 设置一个值，指示网格线是否可见。默认值为 true。 |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | 设置单元格是否为只读。这是 GridWeb 的扩展属性，实际的 Excel 文件中不会保留。 |
| [setName(String value)](#setName-java.lang.String-) | 设置工作表的名称。 |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | 指示是否显示大纲。 |
| [setProtect()](#setProtect--) | 保护工作表。 |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | 将一组单元格设为只读。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 首先通过调用 SetAllCellsEditable 方法将所有单元格设为可编辑。 |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | 设置行的标题。 |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | 设置行标题的工具提示文本。 |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | 将行设为只读，以便用户无法从客户端删除它。 |
| [setSelected(boolean value)](#setSelected-boolean-) | 指示打开工作簿时是否选中此工作表。 |
| [setStandardHeight(double value)](#setStandardHeight-double-) | 设置此工作表中默认的行高，单位为点。 |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | 设置此工作表中默认的行高，单位为像素。 |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | 指示在大纲中汇总行是否会位于明细行的下方。 |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | 表示工作表选项卡颜色。 |
| [setVisible(boolean value)](#setVisible-boolean-) | 指示此工作表的名称是否显示在控件的工作表标签中。 |
| [setZoom(int value)](#setZoom-int-) | 表示以百分比计的缩放因子。 |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | 取消冻结工作表中的窗格。 |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | 取消分组行。 |
| [unProtect()](#unProtect--) | 取消保护工作表。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


设置指定自动筛选适用的范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| startColumn | int | 起始列索引。 |
| endColumn | int | 结束列索引。 |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


为指定行添加自定义过滤器。

**Remarks**

过滤条件字符串。注意我们使用 , 和 ; 作为分隔符，因此单元格值不能包含这些分隔符。以下是条件字符串示例 //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int |  |
| 标准 | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


自动调整列宽。

**Remarks**

AutoFitColumn is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


自动调整列宽。

**Remarks**

此方法根据行内单元格范围的内容自动调整行的大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| firstRow | int | 第一行索引。 |
| lastRow | int | 最后一行索引。 |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


自动调整行高。

**Remarks**

AutoFitRow is an imprecise function.

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


自动调整行高。

**Remarks**

此方法根据行内单元格范围的内容自动调整行的大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| firstColumn | int | 第一列索引。 |
| lastColumn | int | 最后一列索引。 |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


在矩形范围内自动调整行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| endRow | int | 结束行索引。 |
| startColumn | int | 起始列索引。 |
| endColumn | int | 结束列索引。 |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


自动调整此工作表中所有行的高度。

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


自动调整此工作表中所有行的高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| onlyAuto | boolean | True，仅在行高未自定义时自动适配行高。 |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


在范围内自动调整行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| endRow | int | 结束行索引。 |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


计算一个公式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object - 
### clearComments() {#clearComments--}
```
public void clearComments()
```


清除设计器电子表格中的所有批注。

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


复制来自另一个工作表的内容和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | 源工作表。 |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


在工作表中创建小计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnNameRowIndex | int | 列名行的行索引。 |
| dataRows | int | 数据行的数量。 |
| groupByColumnIndex | int | 要分组的列的列索引。 |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction)。小计函数类型。 |
| subtotalColumnIndexList | int[] | 需要进行小计的列索引。 |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


在工作表中创建小计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnNameRowIndex | int | 列名行的行索引。 |
| dataRows | int | 数据行的数量。 |
| groupByColumnIndex | int | 要分组的列的列索引。 |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction)。小计函数类型。 |
| subtotalColumnIndexList | int[] | 需要进行小计的列索引。 |
| functionLabel | java.lang.String | 小计函数的标签。 |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | 总计行的样式。 |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | 小计行的样式。 |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype)。小计结果单元格的数字类型。 |
| customString | java.lang.String | 小计结果单元格的自定义格式字符串。可以为 null。 |

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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


为列设置过滤器。注意，我们应在调用 filterString 之前调用 AddAutoFilter。过滤条件字符串。注意我们使用逗号 -> \",\" 作为分隔符，因此要过滤的单元格值不能包含逗号。filterString(10,\"123,456\") 表示第 10 列应包含 123 或 456，filterString(10,\"123\") 表示第 10 列应包含 123。列索引值使用逗号分隔，例如 123,456,789 或 abc

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int |  |
| 条件 | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


在工作表中指定的单元格处冻结窗格。

**Remarks**

行索引和列索引不能全部为零。行数和列数也不能全部为零。

前两个参数指定冻结位置，后两个参数指定左上窗格中冻结的区域。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |
| freezedRows | int | 顶部窗格中可见行数，不超过行索引。 |
| freezedColumns | int | 左侧窗格中可见列数，不超过列索引。 |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


在工作表中指定的单元格处冻结窗格。

**Remarks**

行索引和列索引不能全部为零。行数和列数也不能全部为零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |
| freezedRows | int | 顶部窗格中可见行数，不超过行索引。 |
| freezedColumns | int | 左侧窗格中可见列数，不超过列索引。 |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


获取工作表中的活动单元格。

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


获取工作表的背景图像。

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


获取 [GridCell](../../com.aspose.gridweb/gridcell) 集合。

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


表示工作表代码名称。

**Remarks**

当模板文件包含 VBA/macro 时，不能更改代码名称。

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


获取列标题。如果标题未设置，返回空字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 列标题。如果标题未设置，返回空字符串。
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


获取列标题的工具提示文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| colIndex | int | 列的索引。 |

**Returns:**
java.lang.String - 工具提示文本。
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


获取列是否为只读。这是 GridWeb 的扩展方法，实际 Excel 文件中不会保留或生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |

**Returns:**
boolean - 如果只读则返回 true。
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


获取 [GridComment](../../com.aspose.gridweb/gridcomment) 集合。

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


指示指定的工作表是否从右向左显示，而不是从左向右。默认值为 false。

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


如果显示零值，则为 True。

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


表示第一个可见列的索引。

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


表示第一个可见行的索引。

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


获取冻结窗格。

**Returns:**
int[] - 返回 null 表示工作表未冻结 0:行索引;1:列;2:冻结行;3:冻结行
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


获取工作表中的活动单元格。

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


获取 [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection) 集合。

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


获取工作表集合中工作表的索引。

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


获取单元格是否为只读。这是 GridWeb 的扩展属性，实际 Excel 文件中不会保留。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int |  |
| 列 | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


获取工作表的名称。

**Remarks**

工作表名称的最大长度为 31。且不能为两个工作表分配相同的名称（不区分大小写）。例如，您不能将 "SheetName1" 设置为第一个工作表，同时将 "SHEETNAME1" 设置为第二个工作表。

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


指示是否显示大纲。

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


获取一个 [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) 集合。

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


获取工作表中的数据透视表。

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


获取行标题。如果标题未设置，返回空字符串。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |

**Returns:**
java.lang.String - 行标题。如果标题未设置，返回空字符串。
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


获取行标题的工具提示文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行的索引。 |

**Returns:**
java.lang.String - 工具提示文本。
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


获取行是否为只读。这是 GridWeb 的扩展方法，实际 Excel 文件中不会保留或生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |

**Returns:**
boolean - 如果只读则返回 true。
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


指示打开工作簿时是否选中此工作表。

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


获取一个 [getPictures()](../../com.aspose.gridweb/gridworksheet\#getPictures--) 集合。

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


获取此工作表中默认的行高，单位为点。

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


获取此工作表中默认的行高，单位为像素。

**Returns:**
int
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


表示工作表选项卡颜色。

**Remarks**

此功能仅在 ExcelXP（Excel2002）及以上版本中受支持。如果将文件另存为 Excel97 或 Excel2000 格式，将被省略。

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


获取控件中的唯一标识符。

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


获取工作表中的数据验证设置集合。

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


指示此工作表的名称是否显示在控件的工作表标签中。

**Returns:**
boolean
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


获取工作表集合的 [GridWorkbook](../../com.aspose.gridweb/gridworkbook) 对象。

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


表示百分比的缩放因子。应在 10 到 400 之间。

**Returns:**
int
### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


对行进行分组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要分组的第一行索引。 |
| lastIndex | int | 要分组的最后一行索引。 |
| isHidden | boolean | 指定分组的行是否隐藏。 |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


获取一个值，指示网格线是否可见。默认值为 true。

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


指示工作表是否受保护。

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


指示在大纲中汇总行是否会位于明细行的下方。

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


将工作表移动到电子表格中的其他位置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 索引 | int | 目标工作表索引。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


刷新自动筛选以隐藏或显示行。

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


移除工作表的自动筛选。

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


移除工作表中由 CreateSubtotal 方法创建的小计。

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


要应用的字段的整数偏移量，基于第一个筛选列（从列表左侧开始；最左侧的字段为字段 0）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


设置工作表中的活动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


使所有单元格可编辑。这是扩展属性。

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


使所有单元格只读。这是扩展属性，注意此属性在实际单元格中无法保留，如果想保持保护，请使用 setProtect。

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


设置工作表的背景图像。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


设置列的标题。请注意，这是一个扩展属性，不能保存在 Excel 文件中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| caption | java.lang.String | 列标题。如果想取消标题，请传入 null 或空字符串。 |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


设置列标题的工具提示文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| colIndex | int | 列的索引。 |
| toolTip | java.lang.String | 工具提示文本。 |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


将列设为只读，使用户无法从客户端删除它。这是 GridWeb 的扩展方法，实际 Excel 文件中不会保留或生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| isReadonly | boolean | 真或假。 |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


指示指定的工作表是否从右向左显示，而不是从左向右。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


如果显示零值，则为 True。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


将一系列单元格设为可编辑。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 通过调用 SetAllCellsReadonly 方法将所有单元格设为只读。然后调用此方法来指定要可编辑的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 范围的起始行。 |
| startColumn | int | 范围的起始列。 |
| 行 | int | 行的数量。 |
| 列 | int | 列的数量。 |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


表示第一个可见列的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


表示第一个可见行的索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


设置工作表中的活动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


设置一个值，指示网格线是否可见。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


设置单元格是否为只读。这是 GridWeb 的扩展属性，实际的 Excel 文件中不会保留。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int |  |
| 列 | int |  |
| 值 | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


设置工作表的名称。

**Remarks**

工作表名称的最大长度为 31。且不能为两个工作表分配相同的名称（不区分大小写）。例如，您不能将 "SheetName1" 设置为第一个工作表，同时将 "SHEETNAME1" 设置为第二个工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


指示是否显示大纲。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


保护工作表。

**Remarks**

此方法在不使用密码的情况下保护工作表。它可以在所有版本的 Excel 文件中保护工作表。

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


将一系列单元格设为只读。 http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells 首先通过调用 SetAllCellsEditable 方法将所有单元格设为可编辑。然后调用此方法来指定要设为只读的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 范围的起始行。 |
| startColumn | int | 范围的起始列。 |
| 行 | int | 行的数量。 |
| 列 | int | 列的数量。 |

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


设置行的标题。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| caption | java.lang.String | 行标题。如果想取消标题，请传入 null 或空字符串。 |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


设置行标题的工具提示文本。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行的索引。 |
| toolTip | java.lang.String | 工具提示文本。 |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


将行设为只读，使用户无法从客户端删除它。这是针对 GridWeb 的扩展方法，且不会保存在实际的 Excel 文件中并产生影响。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| isReadonly | boolean | 真或假。 |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


指示打开工作簿时是否选中此工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


设置此工作表中默认的行高，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


设置此工作表中默认的行高，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


指示在大纲中汇总行是否会位于明细行的下方。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


表示工作表选项卡颜色。

**Remarks**

此功能仅在 ExcelXP（Excel2002）及以上版本中受支持。如果将文件另存为 Excel97 或 Excel2000 格式，将被省略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


指示此工作表的名称是否显示在控件的工作表标签中。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


表示百分比的缩放因子。应在 10 到 400 之间。

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
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


取消冻结工作表中的窗格。

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


取消分组行。

**Remarks**

仅删除外部组信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要取消分组的第一行索引。 |
| lastIndex | int | 要取消分组的最后一行索引。 |

### unProtect() {#unProtect--}
```
public void unProtect()
```


取消保护工作表。

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

