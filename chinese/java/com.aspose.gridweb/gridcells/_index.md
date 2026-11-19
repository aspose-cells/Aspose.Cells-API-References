---
title: "GridCells"
second_title: "Aspose.Cells for Java API 参考"
description: "封装一个对象集合。"
type: docs
url: /zh/java/com.aspose.gridweb/gridcells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class GridCells implements Iterable
```

封装一个 [GridCell](../../com.aspose.gridweb/gridcell) 对象的集合。
## 方法

| 方法 | 描述 |
| --- | --- |
| [cellIndexToName(int row, int column)](#cellIndexToName-int-int-) | 根据行列索引获取单元格名称。 |
| [cellNameToIndex(String cellName, int row, int column)](#cellNameToIndex-java.lang.String-int-int-) | 根据其名称获取单元格的行列索引。 |
| [checkCell(int row, int column)](#checkCell-int-int-) | 获取在指定单元格行索引和列索引处的 [GridCell](../../com.aspose.gridweb/gridcell) 元素或 null。 |
| [checkColumn(int col)](#checkColumn-int-) | 获取在指定列索引处的 [GridColumn](../../com.aspose.gridweb/gridcolumn) 元素或 null。 |
| [checkRow(int i)](#checkRow-int-) | 获取在指定单元格行索引处的 [GridRow](../../com.aspose.gridweb/gridrow) 元素或 null。 |
| [clear()](#clear--) | 清除集合中的所有单元格。 |
| [clearContents(GridCellArea range)](#clearContents-com.aspose.gridweb.GridCellArea-) | 清除范围的内容。 |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | 清除范围的内容。 |
| [clearFormats(GridCellArea range)](#clearFormats-com.aspose.gridweb.GridCellArea-) | 清除范围的格式。 |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | 清除范围的格式。 |
| [clearRange(GridCellArea range)](#clearRange-com.aspose.gridweb.GridCellArea-) | 清除范围的内容和格式。 |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | 清除范围的内容和格式。 |
| [columnIndexToName(int column)](#columnIndexToName-int-) | 根据列索引获取列名称。 |
| [columnNameToIndex(String columnName)](#columnNameToIndex-java.lang.String-) | 根据列名称获取列索引。 |
| [copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.gridweb.GridCells-int-int-) | 复制整列的数据和格式。 |
| [copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.gridweb.GridCells-int-int-int-) | 复制整列的数据和格式。 |
| [copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.gridweb.GridCells-int-int-) | 复制整行的数据和格式。 |
| [copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.gridweb.GridCells-int-int-int-) | 复制若干整行的数据和格式。 |
| [deleteBlankColumns()](#deleteBlankColumns--) | 删除所有不包含任何数据的空列。 |
| [deleteBlankRows()](#deleteBlankRows--) | 删除所有不包含任何数据的空行。 |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | 删除一列。 |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | 删除一列。 |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | 删除多列。 |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | 删除一段单元格并根据移动选项移动单元格。 |
| [deleteRow(int rowIndex)](#deleteRow-int-) | 删除一行。 |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | 删除若干行。 |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | 删除工作表中的多行。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | 将 [GridCells](../../com.aspose.gridweb/gridcells) 集合中的数据导出为二维数组对象。 |
| [get(int row, int column)](#get-int-int-) | 获取指定单元格行索引和列索引处的 [GridCell](../../com.aspose.gridweb/gridcell) 元素。 |
| [get(String cellName)](#get-java.lang.String-) | 获取指定单元格名称处的 [GridCell](../../com.aspose.gridweb/gridcell) 元素。 |
| [getCell(int row, int column)](#getCell-int-int-) | 获取指定单元格行索引和列索引处的 [GridCell](../../com.aspose.gridweb/gridcell) 元素。 |
| [getClass()](#getClass--) |  |
| [getColumnWidth(int column)](#getColumnWidth-int-) | 获取指定列的宽度 |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | 获取指定列的宽度，单位为英寸。 |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | 获取指定列的宽度，单位为像素。 |
| [getColumns()](#getColumns--) | 获取表示此工作表中各个列的 [GridColumn](../../com.aspose.gridweb/gridcolumn) 对象集合。 |
| [getCount()](#getCount--) | 获取单元格的数量。 |
| [getFirstCell()](#getFirstCell--) | 获取此工作表中的第一个单元格。 |
| [getLastCell()](#getLastCell--) | 获取此工作表中的最后一个单元格。 |
| [getMaxColumn()](#getMaxColumn--) | 包含数据或样式的单元格的最大列索引。 |
| [getMaxDataColumn()](#getMaxDataColumn--) | 包含数据的单元格的最大列索引。 |
| [getMaxDataRow()](#getMaxDataRow--) | 包含数据的单元格的最大行索引。 |
| [getMaxRow()](#getMaxRow--) | 包含数据或样式的单元格的最大行索引。 |
| [getMergedCells()](#getMergedCells--) | 获取合并单元格的集合。 |
| [getMinColumn()](#getMinColumn--) | 集合中已实例化的单元格的最小列索引（不包括为整列定义了样式但未实例化任何单元格的列）。 |
| [getMinDataColumn()](#getMinDataColumn--) | 包含数据的单元格的最小列索引。 |
| [getMinDataRow()](#getMinDataRow--) | 包含数据的单元格的最小行索引。 |
| [getMinRow()](#getMinRow--) | 包含数据或样式的单元格的最小行索引。 |
| [getRow(int i)](#getRow-int-) | 获取指定单元格行索引处的 [GridRow](../../com.aspose.gridweb/gridrow) 元素。 |
| [getRowEnumerator()](#getRowEnumerator--) | 获取行枚举器 |
| [getRowHeight(int row)](#getRowHeight-int-) | 获取指定行的高度。 |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | 获取指定行的高度，单位为英寸。 |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | 获取指定行的高度，单位为像素。 |
| [getRowOutlineLevel(int rowIndex)](#getRowOutlineLevel-int-) | 获取行的轮廓级别。 |
| [getRows()](#getRows--) | 获取表示此工作表中各个行的 [GridRow](../../com.aspose.gridweb/gridrow) 对象集合。 |
| [getStandardHeight()](#getStandardHeight--) | 获取此工作表中默认的行高，单位为点。 |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | 获取此工作表中默认的行高，单位为像素。 |
| [getStandardWidth()](#getStandardWidth--) | 获取工作表中默认列宽，单位为字符。 |
| [getStandardWidthInch()](#getStandardWidthInch--) | 获取工作表的默认列宽，单位为英寸。 |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | 获取工作表的默认列宽，单位为像素。 |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | 获取不同视图类型下的宽度。 |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | 对列进行分组。 |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | 对列进行分组。 |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | 对行进行分组。 |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | 隐藏列。 |
| [hideRow(int row)](#hideRow-int-) | 隐藏行。 |
| [insertColumn(int columnIndex)](#insertColumn-int-) | 在工作表中插入新列。 |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | 在工作表中插入新列。 |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | 在工作表中插入若干列。 |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | 在工作表中插入若干列。 |
| [insertRange(GridCellArea area, int shiftType)](#insertRange-com.aspose.gridweb.GridCellArea-int-) | 插入一段单元格并根据移动选项移动单元格。 |
| [insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-) | 插入一段单元格并根据移动选项移动单元格。 |
| [insertRow(int rowIndex)](#insertRow-int-) | 在工作表中插入新行。 |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | 在工作表中插入多行。 |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | 在工作表中插入多行。 |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | 检查给定列是否为空（不包含任何数据）。 |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | 检查给定索引处的列是否隐藏。 |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | 检查给定索引处的行是否隐藏。 |
| [iterator()](#iterator--) | 获取行枚举器 |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | 将指定范围的单元格合并为一个单元格。 |
| [moveRange(GridCellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.gridweb.GridCellArea-int-int-) | 移动该范围。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | 删除范围内的重复值。 |
| [removeFormulas()](#removeFormulas--) | 删除所有公式并替换为公式的值。 |
| [setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)](#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-) | 为单元格范围设置边框。 |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | 设置指定列的宽度。 |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | 以英寸为单位设置列宽。 |
| [setColumnWidthPixel(int column, int pixel)](#setColumnWidthPixel-int-int-) | 以像素为单位设置列宽。 |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | 设置指定行的高度。 |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | 以英寸为单位设置行高。 |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | 以像素为单位设置行高。 |
| [setRowOutlineLevel(int rowIndex, int outlineLevel)](#setRowOutlineLevel-int-int-) | 设置行的轮廓级别。 |
| [setStandardHeight(double value)](#setStandardHeight-double-) | 设置此工作表中默认的行高，单位为点。 |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | 设置此工作表中默认的行高，单位为像素。 |
| [setStandardWidth(double value)](#setStandardWidth-double-) | 设置工作表中默认列宽，单位为字符。 |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | 以英寸为单位设置工作表的默认列宽。 |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | 以像素为单位设置工作表的默认列宽。 |
| [setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)](#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-) | 将样式设置为指定的单元格范围。 |
| [setStyle(String cellRange, GridTableItemStyle style)](#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-) | 将样式设置为指定的单元格范围。 |
| [sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)](#sort-int-int-int-int-int-boolean-boolean-boolean-) | 按指定列索引对工作表中范围内的数据进行自上而下的升序/降序排序。 |
| [sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)](#sort-int-int-int-int-int---int---int-boolean-) | 按指定列索引对工作表中范围内的数据进行自上而下的升序/降序排序。 |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | 取消合并指定范围的合并单元格。 |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | 取消分组列。 |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | 取消分组行。 |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | 取消隐藏列 |
| [unhideRow(int row)](#unhideRow-int-) | 取消隐藏行。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### cellIndexToName(int row, int column) {#cellIndexToName-int-int-}
```
public static String cellIndexToName(int row, int column)
```


根据行列索引获取单元格名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 单元格名称。
### cellNameToIndex(String cellName, int row, int column) {#cellNameToIndex-java.lang.String-int-int-}
```
public static void cellNameToIndex(String cellName, int row, int column)
```


根据其名称获取单元格的行列索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称。 |
| 行 | int | 输出行索引 |
| 列 | int | 输出列索引 |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public GridCell checkCell(int row, int column)
```


获取在指定单元格行索引和列索引处的 [GridCell](../../com.aspose.gridweb/gridcell) 元素或 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |
| 列 | int | 列索引 |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return GridCell object if a GridCell object exists. Return null if the GridCell does not exist.
### checkColumn(int col) {#checkColumn-int-}
```
public GridColumn checkColumn(int col)
```


获取在指定列索引处的 [GridColumn](../../com.aspose.gridweb/gridcolumn) 元素或 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

**Returns:**
[GridColumn](../../com.aspose.gridweb/gridcolumn) - The Column object.
### checkRow(int i) {#checkRow-int-}
```
public GridRow checkRow(int i)
```


获取在指定单元格行索引处的 [GridRow](../../com.aspose.gridweb/gridrow) 元素或 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| i | int | 行索引 |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - Returns [GridRow](../../com.aspose.gridweb/gridrow) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


清除集合中的所有单元格。

### clearContents(GridCellArea range) {#clearContents-com.aspose.gridweb.GridCellArea-}
```
public void clearContents(GridCellArea range)
```


清除范围的内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 要清除的范围。 |

### clearContents(int startRow, int startColumn, int endRow, int endColumn) {#clearContents-int-int-int-int-}
```
public void clearContents(int startRow, int startColumn, int endRow, int endColumn)
```


清除范围的内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| startColumn | int | 起始列索引。 |
| endRow | int | 结束行索引。 |
| endColumn | int | 结束列索引。 |

### clearFormats(GridCellArea range) {#clearFormats-com.aspose.gridweb.GridCellArea-}
```
public void clearFormats(GridCellArea range)
```


清除范围的格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 要清除的范围。 |

### clearFormats(int startRow, int startColumn, int endRow, int endColumn) {#clearFormats-int-int-int-int-}
```
public void clearFormats(int startRow, int startColumn, int endRow, int endColumn)
```


清除范围的格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| startColumn | int | 起始列索引。 |
| endRow | int | 结束行索引。 |
| endColumn | int | 结束列索引。 |

### clearRange(GridCellArea range) {#clearRange-com.aspose.gridweb.GridCellArea-}
```
public void clearRange(GridCellArea range)
```


清除范围的内容和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 要清除的范围。 |

### clearRange(int startRow, int startColumn, int endRow, int endColumn) {#clearRange-int-int-int-int-}
```
public void clearRange(int startRow, int startColumn, int endRow, int endColumn)
```


清除范围的内容和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| startColumn | int | 起始列索引。 |
| endRow | int | 结束行索引。 |
| endColumn | int | 结束列索引。 |

### columnIndexToName(int column) {#columnIndexToName-int-}
```
public static String columnIndexToName(int column)
```


根据列索引获取列名称。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

**Returns:**
java.lang.String - 列名称。
### columnNameToIndex(String columnName) {#columnNameToIndex-java.lang.String-}
```
public static int columnNameToIndex(String columnName)
```


根据列名称获取列索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnName | java.lang.String | 列名称。 |

**Returns:**
int - 列索引。
### copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.gridweb.GridCells-int-int-}
```
public void copyColumn(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


复制整列的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | 源 Cells 对象包含要复制的数据和格式。 |
| sourceColumnIndex | int | 源列索引。 |
| destinationColumnIndex | int | 目标列索引。 |

### copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyColumns(GridCells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


复制整列的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | 源 Cells 对象包含要复制的数据和格式。 |
| sourceColumnIndex | int | 源列索引。 |
| destinationColumnIndex | int | 目标列索引。 |
| columnNumber | int | 复制的列号。 |

### copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.gridweb.GridCells-int-int-}
```
public void copyRow(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


复制整行的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | 源 Cells 对象包含要复制的数据和格式。 |
| sourceRowIndex | int | 源行索引。 |
| destinationRowIndex | int | 目标行索引。 |

### copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.gridweb.GridCells-int-int-int-}
```
public void copyRows(GridCells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


复制若干整行的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [GridCells](../../com.aspose.gridweb/gridcells) | 源 Cells 对象包含要复制的数据和格式。 |
| sourceRowIndex | int | 源行索引。 |
| destinationRowIndex | int | 目标行索引。 |
| rowNumber | int | 复制的行号。 |

### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


删除所有不包含任何数据的空列。

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


删除所有不包含任何数据的空行。

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


删除一列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


删除一列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| updateReference | boolean | 指示是否更新其他工作表中的引用。 |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


删除多列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| totalColumns | int | 要删除的列数。 |
| updateReference | boolean | 指示是否更新其他工作表中的引用。 |

### deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType) {#deleteRange-int-int-int-int-int-}
```
public void deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)
```


删除一段单元格并根据移动选项移动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| startColumn | int | 起始列索引。 |
| endRow | int | 结束行索引。 |
| endColumn | int | 结束列索引。 |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype)。单元格移动选项。 |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


删除一行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


删除若干行。

**Remarks**

如果被删除的范围包含表格（ListObject）的顶部部分（而非整体），则无法删除该范围，且不会执行任何操作。其行为与 MS Excel 相同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 要删除的第一行的索引。 |
| totalRows | int | 要删除的行数。 |

**Returns:**
boolean
### deleteRows(int rowIndex, int totalRows, boolean updateReference) {#deleteRows-int-int-boolean-}
```
public boolean deleteRows(int rowIndex, int totalRows, boolean updateReference)
```


删除工作表中的多行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| totalRows | int | 要删除的行数。 |
| updateReference | boolean | 指示是否更新其他工作表中的引用。 |

**Returns:**
boolean -
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
### exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportArray-int-int-int-int-}
```
public Object[][] exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


将 [GridCells](../../com.aspose.gridweb/gridcells) 集合中的数据导出为二维数组对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 要导出的第一个单元格的行号。 |
| firstColumn | int | 要导出的第一个单元格的列号。 |
| totalRows | int | 要导出的行数 |
| totalColumns | int | 要导出的列数 |

**Returns:**
java.lang.Object[][] - 导出的单元格值数组对象。
### get(int row, int column) {#get-int-int-}
```
public GridCell get(int row, int column)
```


获取指定单元格行索引和列索引处的 [GridCell](../../com.aspose.gridweb/gridcell) 元素。

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
         //Gets the cell at "A1"
         GridCell cell = cells.get(0, 0);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The [GridCell](../../com.aspose.gridweb/gridcell) object.
### get(String cellName) {#get-java.lang.String-}
```
public GridCell get(String cellName)
```


获取指定单元格名称处的 [GridCell](../../com.aspose.gridweb/gridcell) 元素。

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
          GridCells cells = GridWeb1.getWorkSheets().get(0).getCells();
          GridCell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称，包括其列字母和行号，例如 A5。 |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - A [GridCell](../../com.aspose.gridweb/gridcell) object
### getCell(int row, int column) {#getCell-int-int-}
```
public GridCell getCell(int row, int column)
```


获取指定单元格行索引和列索引处的 [GridCell](../../com.aspose.gridweb/gridcell) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |
| 列 | int | 列索引 |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - Return Cell object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


获取指定列的宽度

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

**Returns:**
double - 列宽
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


获取指定列的宽度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

**Returns:**
double - 列宽
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


获取指定列的宽度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

**Returns:**
int - 正常视图下列的宽度。
### getColumns() {#getColumns--}
```
public GridColumnCollection getColumns()
```


获取表示此工作表中各个列的 [GridColumn](../../com.aspose.gridweb/gridcolumn) 对象集合。

**Returns:**
[GridColumnCollection](../../com.aspose.gridweb/gridcolumncollection)
### getCount() {#getCount--}
```
public int getCount()
```


获取单元格的数量。

**Returns:**
int
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


获取此工作表中的第一个单元格。

**Remarks**

如果工作表中没有数据，则返回 null。

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


获取此工作表中的最后一个单元格。

**Remarks**

如果工作表中没有数据，则返回 null。

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


包含数据或样式的单元格的最大列索引。

**Remarks**

如果不存在单元格则返回 -1。

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


包含数据的单元格的最大列索引。

**Remarks**

-1 将在没有包含数据的单元格时返回。此属性需要遍历并检查工作表中的所有单元格，因此耗时较长，不应重复调用。

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


包含数据的单元格的最大行索引。

**Remarks**

如果没有包含数据的单元格则返回 -1。

**Returns:**
int
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


包含数据或样式的单元格的最大行索引。

**Remarks**

如果工作表中没有包含数据或样式的单元格则返回 -1。

**Returns:**
int
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


获取合并单元格的集合。

**Remarks**

在此集合中，每个项都是一个 [GridCellArea](../../com.aspose.gridweb/gridcellarea) 结构，表示合并单元格的区域。

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


集合中已实例化的单元格的最小列索引（不包括为整列定义了样式但未实例化任何单元格的列）。

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


包含数据的单元格的最小列索引。

**Remarks**

-1 将在没有包含数据的单元格时返回。此属性需要遍历并检查工作表中的所有单元格，因此耗时较长，不应重复调用。

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


包含数据的单元格的最小行索引。

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


包含数据或样式的单元格的最小行索引。

**Returns:**
int
### getRow(int i) {#getRow-int-}
```
public GridRow getRow(int i)
```


获取指定单元格行索引处的 [GridRow](../../com.aspose.gridweb/gridrow) 元素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| i | int | 行索引 |

**Returns:**
[GridRow](../../com.aspose.gridweb/gridrow) - the row object
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


获取行枚举器

**Returns:**
java.util.Iterator - 行迭代器。
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


获取指定行的高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |

**Returns:**
double - 行高。
### getRowHeightInch(int row) {#getRowHeightInch-int-}
```
public double getRowHeightInch(int row)
```


获取指定行的高度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |

**Returns:**
double - 行高。
### getRowHeightPixel(int row) {#getRowHeightPixel-int-}
```
public int getRowHeightPixel(int row)
```


获取指定行的高度，单位为像素。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |

**Returns:**
int - 行的高度
### getRowOutlineLevel(int rowIndex) {#getRowOutlineLevel-int-}
```
public int getRowOutlineLevel(int rowIndex)
```


获取行的轮廓级别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |

**Returns:**
int - 大纲级别。
### getRows() {#getRows--}
```
public GridRowCollection getRows()
```


获取表示此工作表中各个行的 [GridRow](../../com.aspose.gridweb/gridrow) 对象集合。

**Returns:**
[GridRowCollection](../../com.aspose.gridweb/gridrowcollection)
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
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


获取工作表中默认列宽，单位为字符。

**Returns:**
double
### getStandardWidthInch() {#getStandardWidthInch--}
```
public double getStandardWidthInch()
```


获取工作表的默认列宽，单位为英寸。

**Returns:**
double
### getStandardWidthPixels() {#getStandardWidthPixels--}
```
public int getStandardWidthPixels()
```


获取工作表的默认列宽，单位为像素。

**Returns:**
int
### getViewColumnWidthPixel(int column) {#getViewColumnWidthPixel-int-}
```
public int getViewColumnWidthPixel(int column)
```


获取不同视图类型下的宽度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

**Returns:**
int - 列宽（单位为像素）
### groupColumns(int firstIndex, int lastIndex) {#groupColumns-int-int-}
```
public void groupColumns(int firstIndex, int lastIndex)
```


对列进行分组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要分组的第一列索引。 |
| lastIndex | int | 要分组的最后一列索引。 |

### groupColumns(int firstIndex, int lastIndex, boolean isHidden) {#groupColumns-int-int-boolean-}
```
public void groupColumns(int firstIndex, int lastIndex, boolean isHidden)
```


对列进行分组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要分组的第一列索引。 |
| lastIndex | int | 要分组的最后一列索引。 |
| isHidden | boolean | 指定分组的列是否隐藏。 |

### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


对行进行分组。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要分组的第一行索引。 |
| lastIndex | int | 要分组的最后一行索引。 |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


隐藏列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


隐藏行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |

### insertColumn(int columnIndex) {#insertColumn-int-}
```
public void insertColumn(int columnIndex)
```


在工作表中插入新列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |

### insertColumn(int columnIndex, boolean updateReference) {#insertColumn-int-boolean-}
```
public void insertColumn(int columnIndex, boolean updateReference)
```


在工作表中插入新列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| updateReference | boolean | 指示是否会更新其他工作表中的引用。 |

### insertColumns(int columnIndex, int totalColumns) {#insertColumns-int-int-}
```
public void insertColumns(int columnIndex, int totalColumns)
```


在工作表中插入若干列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| totalColumns | int | 列的数量。 |

### insertColumns(int columnIndex, int totalColumns, boolean updateReference) {#insertColumns-int-int-boolean-}
```
public void insertColumns(int columnIndex, int totalColumns, boolean updateReference)
```


在工作表中插入若干列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| totalColumns | int | 列的数量。 |
| updateReference | boolean | 指示是否会更新其他工作表中的引用。 |

### insertRange(GridCellArea area, int shiftType) {#insertRange-com.aspose.gridweb.GridCellArea-int-}
```
public void insertRange(GridCellArea area, int shiftType)
```


插入一段单元格并根据移动选项移动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 移动区域。 |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype)。单元格移动选项。 |

### insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.gridweb.GridCellArea-int-int-boolean-}
```
public void insertRange(GridCellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


插入一段单元格并根据移动选项移动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 移动区域。 |
| shiftNumber | int | 要插入的行数或列数。 |
| shiftType | int | [GridShiftType](../../com.aspose.gridweb/gridshifttype)。单元格移动选项。 |
| updateReference | boolean | 指示是否更新其他工作表中的引用。 |

### insertRow(int rowIndex) {#insertRow-int-}
```
public void insertRow(int rowIndex)
```


在工作表中插入新行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |

### insertRows(int rowIndex, int totalRows) {#insertRows-int-int-}
```
public void insertRows(int rowIndex, int totalRows)
```


在工作表中插入多行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| totalRows | int | 要插入的行数。 |

### insertRows(int rowIndex, int totalRows, boolean updateReference) {#insertRows-int-int-boolean-}
```
public void insertRows(int rowIndex, int totalRows, boolean updateReference)
```


在工作表中插入多行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| totalRows | int | 要插入的行数。 |
| updateReference | boolean | 指示是否会更新其他工作表中的引用。 |

### isBlankColumn(int columnIndex) {#isBlankColumn-int-}
```
public boolean isBlankColumn(int columnIndex)
```


检查给定列是否为空（不包含任何数据）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引 |

**Returns:**
布尔值 - 如果给定列不包含任何数据则为 true
### isColumnHidden(int columnIndex) {#isColumnHidden-int-}
```
public boolean isColumnHidden(int columnIndex)
```


检查给定索引处的列是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引 |

**Returns:**
boolean - 如果列被隐藏则为 true。
### isRowHidden(int rowIndex) {#isRowHidden-int-}
```
public boolean isRowHidden(int rowIndex)
```


检查给定索引处的行是否隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引 |

**Returns:**
boolean - 如果行被隐藏则为 true
### iterator() {#iterator--}
```
public Iterator iterator()
```


获取行枚举器

**Returns:**
java.util.Iterator - 行枚举器
### merge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#merge-int-int-int-int-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


将指定范围的单元格合并为一个单元格。

**Remarks**

通过范围左上角单元格的地址引用合并单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 此范围的第一行（零基）。 |
| firstColumn | int | 此范围的第一列（零基）。 |
| totalRows | int | 行数（从一开始计）。 |
| totalColumns | int | 列数（从一开始计）。 |

### moveRange(GridCellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.gridweb.GridCellArea-int-int-}
```
public void moveRange(GridCellArea sourceArea, int destRow, int destColumn)
```


移动该范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | 应移动的范围。 |
| destRow | int | 目标行。 |
| destColumn | int | 目标列。 |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn) {#removeDuplicates-int-int-int-int-}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)
```


删除范围内的重复值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行。 |
| startColumn | int | 起始列 |
| endRow | int | 结束行索引。 |
| endColumn | int | 结束列索引。 |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


删除所有公式并替换为公式的值。

### setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle) {#setBorders-int-int-int-int-int-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorders(int firstRow, int firstColumn, int rowNumber, int columnNumber, int position, WebBorderStyle borderStyle)
```


为单元格范围设置边框。

**Example**

```
           GridWeb GridWeb1 = new GridWeb();
           WebBorderStyle borderStyle1 = new WebBorderStyle();
         	 GridWeb1.getWorkSheets().get(0).getCells().setBorders(0, 0, 5, 8, SetBorderPosition.OUTLINE, borderStyle1);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 范围的第一行号（从零开始）。 |
| firstColumn | int | 范围的第一列号（从零开始）。 |
| rowNumber | int | 行数。 |
| columnNumber | int | 列数。 |
| position | int | [SetBorderPosition](../../com.aspose.gridweb/setborderposition)。边框位置。 |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | 边框样式。 |

### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


设置指定列的宽度。

**Remarks**

要隐藏列，将列宽设置为零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 宽度 | double | 列宽。列宽必须在 0 到 255 之间。 |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


以英寸为单位设置列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 英寸 | double | 英寸数。 |

### setColumnWidthPixel(int column, int pixel) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixel)
```


以像素为单位设置列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 像素 | int | 像素数。 |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


设置指定行的高度。

**Remarks**

要隐藏行，将行高设置为零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 高度 | double | 行高。单位为点，范围应在 0 到 409.5 之间。 |

### setRowHeightInch(int row, double inches) {#setRowHeightInch-int-double-}
```
public void setRowHeightInch(int row, double inches)
```


以英寸为单位设置行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 英寸 | double | 英寸数。它应在 0 到 409.5/72 之间。 |

### setRowHeightPixel(int row, int pixels) {#setRowHeightPixel-int-int-}
```
public void setRowHeightPixel(int row, int pixels)
```


以像素为单位设置行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 像素 | int | 像素数。 |

### setRowOutlineLevel(int rowIndex, int outlineLevel) {#setRowOutlineLevel-int-int-}
```
public void setRowOutlineLevel(int rowIndex, int outlineLevel)
```


设置行的轮廓级别。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| outlineLevel | int | 大纲级别。 |

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

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


设置工作表中默认列宽，单位为字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setStandardWidthInch(double value) {#setStandardWidthInch-double-}
```
public void setStandardWidthInch(double value)
```


以英寸为单位设置工作表的默认列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setStandardWidthPixels(int value) {#setStandardWidthPixels-int-}
```
public void setStandardWidthPixels(int value)
```


以像素为单位设置工作表的默认列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style) {#setStyle-int-int-int-int-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(int firstRow, int firstColumn, int rowNumber, int columnNumber, GridTableItemStyle style)
```


将样式设置为指定的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 此范围的第一行（零基）。 |
| firstColumn | int | 此范围的第一列（零基）。 |
| rowNumber | int | 行数（从一开始计）。 |
| columnNumber | int | 列数（从一开始计）。 |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | 要设置的样式对象 |

### setStyle(String cellRange, GridTableItemStyle style) {#setStyle-java.lang.String-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(String cellRange, GridTableItemStyle style)
```


将样式设置为指定的单元格范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellRange | java.lang.String | 单元格名称的范围，例如 "A1:D6" |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | 要设置的样式对象 |

### sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright) {#sort-int-int-int-int-int-boolean-boolean-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int index, boolean isAsending, boolean isCaseSensitive, boolean islefttoright)
```


在工作表的范围内，根据指定的列索引，将数据自上而下升序/降序排序。 在工作表的范围内，根据指定的行索引，将数据自左向右升序/降序排序。

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWeb1.getWorkSheets().get(0).getCells().sort(1,0,25,6,3,true,true,false);
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 要排序的第一个单元格的行号。 |
| startColumn | int | 要排序的第一个单元格的列号。 |
| 行 | int | 要导入的行数。 |
| 列 | int | 要导入的列数。 |
| 索引 | int | 指定排序列的列索引。如果排序方向为自上而下，则表示指定排序列的列索引。如果排序方向为自左向右，则表示指定排序行的行索引。 |
| isAsending | boolean | 排序顺序是否为升序。 |
| isCaseSensitive | boolean | 排序是否区分大小写。 |
| islefttoright | boolean | 排序方向是否为自左向右 |

### sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive) {#sort-int-int-int-int-int---int---int-boolean-}
```
public void sort(int startRow, int startColumn, int rows, int columns, int[] indexes, int[] orders, int orientation, boolean isCaseSensitive)
```


在工作表的范围内，根据指定的列索引，将数据自上而下升序/降序排序。 在工作表的范围内，根据指定的行索引，将数据自左向右升序/降序排序。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 要排序的第一个单元格的行号。 |
| startColumn | int | 要排序的第一个单元格的列号。 |
| 行 | int | 要导入的行数。 |
| 列 | int | 要导入的列数。 |
| indexes | int[] | 指定排序列的列索引数组。如果排序方向为自上而下，则表示指定排序列的列索引。如果排序方向为自左向右，则表示指定排序行的行索引。 |
| orders | int[] | [SortByOrder](../../com.aspose.gridweb/sortbyorder)。排序顺序数组。 |
| orientation | int | [SortOrientation](../../com.aspose.gridweb/sortorientation)。排序方向 |
| isCaseSensitive | boolean | 排序是否区分大小写。 |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns) {#unMerge-int-int-int-int-}
```
public void unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


取消合并指定范围的合并单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 此范围的第一行（零基）。 |
| firstColumn | int | 此范围的第一列（零基）。 |
| totalRows | int | 行数（从一开始计）。 |
| totalColumns | int | 列数（从一开始计）。 |

### ungroupColumns(int firstIndex, int lastIndex) {#ungroupColumns-int-int-}
```
public void ungroupColumns(int firstIndex, int lastIndex)
```


取消分组列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要取消分组的第一列索引。 |
| lastIndex | int | 要取消分组的最后一列索引。 |

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


取消分组行。

**Remarks**

仅删除外部组信息。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要取消分组的第一行索引。 |
| lastIndex | int | 要取消分组的最后一行索引。 |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


取消隐藏列

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 宽度 | double | 列宽..列宽必须在 0 到 255 之间 |

### unhideRow(int row) {#unhideRow-int-}
```
public void unhideRow(int row)
```


取消隐藏行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |

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

