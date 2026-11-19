---
title: "单元格"
second_title: "Aspose.Cells for Java API 参考"
description: "封装与单元格相关的对象集合，例如 ...等。"
type: docs
url: /zh/java/com.aspose.cells/cells/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class Cells implements Iterable
```

封装与单元格相关的对象集合，例如 [Cell](../../com.aspose.cells/cell)、[Row](../../com.aspose.cells/row) 等。

**Remarks**

**Example**

```
         Workbook excel = new Workbook();
         	Cells cells = excel.getWorksheets().get(0).getCells();
 
         	//Set default row height
         	cells.setStandardHeight(20);
         	//Set row height
         	cells.setRowHeight(2, 20.5);
 
         	//Set default colum width
         	cells.setStandardWidth(15);
         	//Set column width
         	cells.setColumnWidth(3, 12.57);
 
         	//Merge cells
         	cells.merge(5, 4, 2, 2);
 
         	//Put values to cells
         	cells.get(0, 0).putValue(true);
         	cells.get(0, 1).putValue(1);
         	cells.get(0, 2).putValue("abc");
 
         //Export data
         Object[][] arr = cells.exportArray(0, 0, 10, 10);
```
## 方法

| 方法 | 描述 |
| --- | --- |
| [addRange(Range rangeObject)](#addRange-com.aspose.cells.Range-) | 向单元格添加范围对象引用 |
| [applyColumnStyle(int column, Style style, StyleFlag flag)](#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | 对整列应用格式。 |
| [applyRowStyle(int row, Style style, StyleFlag flag)](#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | 对整行应用格式。 |
| [applyStyle(Style style, StyleFlag flag)](#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-) | 对整个工作表应用格式。 |
| [checkCell(int row, int column)](#checkCell-int-int-) | 获取指定单元格行索引和列索引处的 [Cell](../../com.aspose.cells/cell) 元素或 null。 |
| [checkColumn(int columnIndex)](#checkColumn-int-) | 获取指定列索引处的 [Column](../../com.aspose.cells/column) 元素或 null。 |
| [checkRow(int row)](#checkRow-int-) | 获取指定单元格行索引处的 [Row](../../com.aspose.cells/row) 元素或 null。 |
| [clear()](#clear--) | 清除工作表的所有数据。 |
| [clearContents(CellArea range)](#clearContents-com.aspose.cells.CellArea-) | 清除范围的内容。 |
| [clearContents(int startRow, int startColumn, int endRow, int endColumn)](#clearContents-int-int-int-int-) | 清除范围的内容。 |
| [clearFormats(CellArea range)](#clearFormats-com.aspose.cells.CellArea-) | 清除范围的格式。 |
| [clearFormats(int startRow, int startColumn, int endRow, int endColumn)](#clearFormats-int-int-int-int-) | 清除范围的格式。 |
| [clearMergedCells()](#clearMergedCells--) | 清除所有合并的范围。 |
| [clearRange(CellArea range)](#clearRange-com.aspose.cells.CellArea-) | 清除范围的内容和格式。 |
| [clearRange(int startRow, int startColumn, int endRow, int endColumn)](#clearRange-int-int-int-int-) | 清除范围的内容和格式。 |
| [convertStringToNumericValue()](#convertStringToNumericValue--) | 将工作表中的所有字符串数据（如果可能）转换为数值。 |
| [copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)](#copyColumn-com.aspose.cells.Cells-int-int-) | 复制整列的数据和格式。 |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)](#copyColumns-com.aspose.cells.Cells-int-int-int-) | 复制多列的数据和格式。 |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)](#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-) | 复制整列的数据和格式。 |
| [copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)](#copyColumns-com.aspose.cells.Cells-int-int-int-int-) | 复制所有列的数据和格式。 |
| [copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)](#copyRow-com.aspose.cells.Cells-int-int-) | 复制整行的数据和格式。 |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)](#copyRows-com.aspose.cells.Cells-int-int-int-) | 复制若干整行的数据和格式。 |
| [copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-) | 复制若干整行的数据和格式。 |
| [copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)](#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-) | 复制若干整行的数据和格式。 |
| [createRange(int firstIndex, int number, boolean isVertical)](#createRange-int-int-boolean-) | 从单元格的行或列创建一个 [Range](../../com.aspose.cells/range) 对象。 |
| [createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)](#createRange-int-int-int-int-) | 从单元格范围创建一个 [Range](../../com.aspose.cells/range) 对象。 |
| [createRange(String address)](#createRange-java.lang.String-) | 从范围地址创建一个 [Range](../../com.aspose.cells/range) 对象。 |
| [createRange(String upperLeftCell, String lowerRightCell)](#createRange-java.lang.String-java.lang.String-) | 从单元格范围创建一个 [Range](../../com.aspose.cells/range) 对象。 |
| [deleteBlankColumns()](#deleteBlankColumns--) | 删除所有不包含任何数据的空列。 |
| [deleteBlankColumns(DeleteOptions options)](#deleteBlankColumns-com.aspose.cells.DeleteOptions-) | 删除所有不包含任何数据的空列。 |
| [deleteBlankRows()](#deleteBlankRows--) | 删除所有不包含任何数据或其他对象的空行。 |
| [deleteBlankRows(DeleteOptions options)](#deleteBlankRows-com.aspose.cells.DeleteOptions-) | 删除所有不包含任何数据或某些特殊对象（如可见批注、数据透视表）的空行。 |
| [deleteColumn(int columnIndex)](#deleteColumn-int-) | 删除一列。 |
| [deleteColumn(int columnIndex, boolean updateReference)](#deleteColumn-int-boolean-) | 删除一列。 |
| [deleteColumns(int columnIndex, int totalColumns, boolean updateReference)](#deleteColumns-int-int-boolean-) | 删除多列。 |
| [deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)](#deleteColumns-int-int-com.aspose.cells.DeleteOptions-) | 删除多列。 |
| [deleteRange(int startRow, int startColumn, int endRow, int endColumn, int shiftType)](#deleteRange-int-int-int-int-int-) | 删除一段单元格并根据移动选项移动单元格。 |
| [deleteRow(int rowIndex)](#deleteRow-int-) | 删除一行。 |
| [deleteRow(int rowIndex, boolean updateReference)](#deleteRow-int-boolean-) | 删除一行。 |
| [deleteRows(int rowIndex, int totalRows)](#deleteRows-int-int-) | 删除多行。 |
| [deleteRows(int rowIndex, int totalRows, boolean updateReference)](#deleteRows-int-int-boolean-) | 删除工作表中的多行。 |
| [deleteRows(int rowIndex, int totalRows, DeleteOptions options)](#deleteRows-int-int-com.aspose.cells.DeleteOptions-) | 删除工作表中的多行。 |
| [dispose()](#dispose--) | 执行应用程序定义的任务，以释放、释放或重置非托管资源。 |
| [endCellInColumn(int columnIndex)](#endCellInColumn-int-) | 获取此列中的最后一个单元格。 |
| [endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)](#endCellInColumn-int-int-int-int-) | 获取此范围内列索引最大的最后一个单元格。 |
| [endCellInRow(int rowIndex)](#endCellInRow-int-) | 获取此行中的最后一个单元格。 |
| [endCellInRow(int startRow, int endRow, int startColumn, int endColumn)](#endCellInRow-int-int-int-int-) | 获取此范围内行索引最大的最后一个单元格。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [exportArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportArray-int-int-int-int-) | 将 [Cells](../../com.aspose.cells/cells) 集合中的数据导出为二维数组对象。 |
| [exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)](#exportTypeArray-int-int-int-int-) | 将 [Cells](../../com.aspose.cells/cells) 集合中的单元格值类型导出为二维数组对象。 |
| [find(Object what, Cell previousCell)](#find-java.lang.Object-com.aspose.cells.Cell-) | 查找包含输入对象的单元格。 |
| [find(Object what, Cell previousCell, FindOptions findOptions)](#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-) | 查找包含输入对象的单元格。 |
| [get(int row, int column)](#get-int-int-) | 获取指定单元格行索引和列索引处的 [Cell](../../com.aspose.cells/cell) 元素。 |
| [get(String cellName)](#get-java.lang.String-) | 获取指定单元格名称处的 [Cell](../../com.aspose.cells/cell) 元素。 |
| [getCellDisplayStyle(int row, int column)](#getCellDisplayStyle-int-int-) | 获取给定单元格的显示样式。 |
| [getCellDisplayStyle(int row, int column, int adjacentBorders)](#getCellDisplayStyle-int-int-int-) | 获取给定单元格的显示样式。 |
| [getCellStyle(int row, int column)](#getCellStyle-int-int-) | 获取给定单元格的样式。 |
| [getCellsWithPlaceInCellPicture()](#getCellsWithPlaceInCellPicture--) | 获取所有包含嵌入图片的单元格。 |
| [getClass()](#getClass--) |  |
| [getColumnOriginalWidthPoint(int column)](#getColumnOriginalWidthPoint-int-) | 如果列被隐藏，获取原始列的高度（单位为点）。 |
| [getColumnWidth(int column)](#getColumnWidth-int-) | 获取指定列在普通视图中的宽度（以字符为单位） |
| [getColumnWidth(int column, boolean isOriginal, int unitType)](#getColumnWidth-int-boolean-int-) | 获取列宽。 |
| [getColumnWidthInch(int column)](#getColumnWidthInch-int-) | 获取指定列在普通视图中的宽度（单位为英寸）。 |
| [getColumnWidthPixel(int column)](#getColumnWidthPixel-int-) | 获取指定列在普通视图中的宽度（单位为像素）。 |
| [getColumnWidthPixel(int column, boolean original)](#getColumnWidthPixel-int-boolean-) | 获取指定列在普通视图中的宽度（单位为像素）。 |
| [getColumns()](#getColumns--) | 获取表示此工作表中各列的 [Column](../../com.aspose.cells/column) 对象集合。 |
| [getCount()](#getCount--) | 获取已实例化的 Cell 对象的总数。 |
| [getCountLarge()](#getCountLarge--) | 获取已实例化的 Cell 对象的总数。 |
| [getDependents(boolean isAll, int row, int column)](#getDependents-boolean-int-int-) | 获取所有引用特定单元格的单元格。 |
| [getDependentsInCalculation(int row, int column, boolean recursive)](#getDependentsInCalculation-int-int-boolean-) | 获取所有其计算结果依赖于特定单元格的单元格。 |
| [getFirstCell()](#getFirstCell--) | 获取此工作表中的第一个单元格。 |
| [getFirstDataRow(int column)](#getFirstDataRow-int-) | 获取指定列中包含数据的单元格的第一行索引。 |
| [getGroupedColumnOutlineLevel(int columnIndex)](#getGroupedColumnOutlineLevel-int-) | 获取列的轮廓级别（从零开始计）。 |
| [getGroupedRowOutlineLevel(int rowIndex)](#getGroupedRowOutlineLevel-int-) | 获取行的轮廓级别（从零开始计）。 |
| [getLastCell()](#getLastCell--) | 获取此工作表中的最后一个单元格。 |
| [getLastDataRow(int column)](#getLastDataRow-int-) | 获取指定列中包含数据的单元格的最后一行索引。 |
| [getMaxColumn()](#getMaxColumn--) | 集合中已实例化的单元格的最大列索引（不包括为整列定义了样式但未实例化任何单元格的列）。 |
| [getMaxDataColumn()](#getMaxDataColumn--) | 包含数据的单元格的最大列索引。 |
| [getMaxDataRow()](#getMaxDataRow--) | 包含数据的单元格的最大行索引。 |
| [getMaxDisplayRange()](#getMaxDisplayRange--) | 获取包括数据、合并单元格和形状的最大范围。 |
| [getMaxGroupedColumnOutlineLevel()](#getMaxGroupedColumnOutlineLevel--) | 获取最大分组列的轮廓级别（从零开始计）。 |
| [getMaxGroupedRowOutlineLevel()](#getMaxGroupedRowOutlineLevel--) | 获取最大分组行的轮廓级别（从零开始计）。 |
| [getMaxRow()](#getMaxRow--) | 包含数据或样式的单元格的最大行索引。 |
| [getMemorySetting()](#getMemorySetting--) | 获取此单元格的内存使用选项。 |
| [getMergedAreas()](#getMergedAreas--) | 获取所有合并的单元格。 |
| [getMergedCells()](#getMergedCells--) | 获取合并单元格的集合。 |
| [getMinColumn()](#getMinColumn--) | 集合中已实例化的单元格的最小列索引（不包括为整列定义了样式但未实例化任何单元格的列）。 |
| [getMinDataColumn()](#getMinDataColumn--) | 包含数据的单元格的最小列索引。 |
| [getMinDataRow()](#getMinDataRow--) | 包含数据的单元格的最小行索引。 |
| [getMinRow()](#getMinRow--) | 包含数据或样式的单元格的最小行索引。 |
| [getMultiThreadReading()](#getMultiThreadReading--) | 获取单元格数据模型是否应支持 Multi-Thread 读取。 |
| [getOdsCellFields()](#getOdsCellFields--) | 获取 ods 的字段列表。 |
| [getPreserveString()](#getPreserveString--) | 获取一个值，指示是否所有工作表值都被保留为字符串。 |
| [getRanges()](#getRanges--) | 获取在运行时创建的 [Range](../../com.aspose.cells/range) 对象集合。 |
| [getRowEnumerator()](#getRowEnumerator--) | 获取行枚举器。 |
| [getRowHeight(int row)](#getRowHeight-int-) | 获取指定行的高度，单位为点。 |
| [getRowHeight(int row, boolean isOriginal, int unitType)](#getRowHeight-int-boolean-int-) | 获取行的高度。 |
| [getRowHeightInch(int row)](#getRowHeightInch-int-) | 获取指定行的高度，单位为英寸。 |
| [getRowHeightPixel(int row)](#getRowHeightPixel-int-) | 获取指定行的高度，单位为像素。 |
| [getRowOriginalHeightPoint(int row)](#getRowOriginalHeightPoint-int-) | 如果行被隐藏，获取原始行的高度，单位为点 |
| [getRows()](#getRows--) | 获取表示此工作表中各个行的 [Row](../../com.aspose.cells/row) 对象集合。 |
| [getStandardHeight()](#getStandardHeight--) | 获取此工作表的默认行高，单位为点。 |
| [getStandardHeightInch()](#getStandardHeightInch--) | 获取此工作表的默认行高，单位为英寸。 |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | 获取此工作表的默认行高，单位为像素。 |
| [getStandardWidth()](#getStandardWidth--) | 获取工作表的默认列宽，单位为字符。 |
| [getStandardWidthInch()](#getStandardWidthInch--) | 获取工作表的默认列宽，单位为英寸。 |
| [getStandardWidthPixels()](#getStandardWidthPixels--) | 获取工作表的默认列宽，单位为像素。 |
| [getStyle()](#getStyle--) | 获取工作表的默认样式。 |
| [getViewColumnWidthPixel(int column)](#getViewColumnWidthPixel-int-) | 获取不同视图类型下的宽度。 |
| [getViewRowHeight(int row)](#getViewRowHeight-int-) | 获取指定行的高度。 |
| [getViewRowHeightInch(int row)](#getViewRowHeightInch-int-) | 获取指定行的高度，单位为英寸。 |
| [groupColumns(int firstIndex, int lastIndex)](#groupColumns-int-int-) | 对列进行分组。 |
| [groupColumns(int firstIndex, int lastIndex, boolean isHidden)](#groupColumns-int-int-boolean-) | 对列进行分组。 |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | 对行进行分组。 |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | 对行进行分组。 |
| [hashCode()](#hashCode--) |  |
| [hideColumn(int column)](#hideColumn-int-) | 隐藏列。 |
| [hideColumns(int column, int totalColumns)](#hideColumns-int-int-) | 隐藏多列。 |
| [hideGroupDetail(boolean isVertical, int index)](#hideGroupDetail-boolean-int-) | 折叠已分组的行/列。 |
| [hideRow(int row)](#hideRow-int-) | 隐藏行。 |
| [hideRows(int row, int totalRows)](#hideRows-int-int-) | 隐藏多行。 |
| [importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-double---int-int-boolean-) | 将 double 数组导入工作表。 |
| [importArray(double[][] doubleArray, int firstRow, int firstColumn)](#importArray-double-----int-int-) | 将 double 类型的二维数组导入工作表。 |
| [importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-int---int-int-boolean-) | 将整数数组导入工作表。 |
| [importArray(int[][] intArray, int firstRow, int firstColumn)](#importArray-int-----int-int-) | 将整数的二维数组导入工作表。 |
| [importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importArray-java.lang.String---int-int-boolean-) | 将字符串数组导入工作表。 |
| [importArray(String[][] stringArray, int firstRow, int firstColumn)](#importArray-java.lang.String-----int-int-) | 将字符串的二维数组导入工作表。 |
| [importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)](#importArrayList-java.util.ArrayList-int-int-boolean-) | 将数据的 ArrayList 导入工作表。 |
| [importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-) | 将 CSV 文件导入单元格。 |
| [importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-) | 将 CSV 文件导入单元格。 |
| [importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)](#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-) | 将 CSV 文件导入单元格。 |
| [importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)](#importCSV-java.lang.String-java.lang.String-boolean-int-int-) | 将 CSV 文件导入单元格。 |
| [importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)](#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-) | 导入自定义对象。 |
| [importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)](#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-) | 导入自定义对象。 |
| [importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)](#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-) | 从自定义数据表导入数据。 |
| [importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)](#importFormulaArray-java.lang.String---int-int-boolean-) | 将公式数组导入工作表。 |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)](#importObjectArray-java.lang.Object---int-int-boolean-) | 将数据数组导入工作表。 |
| [importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)](#importObjectArray-java.lang.Object---int-int-boolean-int-) | 将数据数组导入工作表。 |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-boolean-) | 将 ResultSet 对象中的数据导入工作表。 |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-) | 将 ResultSet 对象中的数据导入工作表。 |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-) | 将 ResultSet 对象中的数据导入工作表。 |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-) | 将 ResultSet 对象中的数据导入工作表。 |
| [importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)](#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-) | 将 ResultSet 对象中的数据导入工作表。 |
| [importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-boolean-) | 将 ResultSet 对象中的数据导入工作表。 |
| [importResultSet(ResultSet rs, String startCell, ImportTableOptions options)](#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-) | 将 ResultSet 对象中的数据导入工作表。 |
| [importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)](#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-) | 将 ResultSet 对象中的数据导入工作表。 |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)](#importTwoDimensionArray-java.lang.Object-----int-int-) | 将数据的二维数组导入工作表。 |
| [importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----int-int-boolean-) | 将数据的二维数组导入工作表。 |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-) | 将数据的二维数组导入工作表。 |
| [importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)](#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-) | 将数据的二维数组导入工作表。 |
| [insertColumn(int columnIndex)](#insertColumn-int-) | 在工作表中插入新列。 |
| [insertColumn(int columnIndex, boolean updateReference)](#insertColumn-int-boolean-) | 在工作表中插入新列。 |
| [insertColumns(int columnIndex, int totalColumns)](#insertColumns-int-int-) | 在工作表中插入若干列。 |
| [insertColumns(int columnIndex, int totalColumns, boolean updateReference)](#insertColumns-int-int-boolean-) | 在工作表中插入若干列。 |
| [insertColumns(int columnIndex, int totalColumns, InsertOptions options)](#insertColumns-int-int-com.aspose.cells.InsertOptions-) | 在工作表中插入若干列。 |
| [insertCutCells(Range cutRange, int row, int column, int shiftType)](#insertCutCells-com.aspose.cells.Range-int-int-int-) | 插入剪切范围。 |
| [insertRange(CellArea area, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-) | 插入一段单元格并根据移动选项移动单元格。 |
| [insertRange(CellArea area, int shiftNumber, int shiftType)](#insertRange-com.aspose.cells.CellArea-int-int-) | 插入一段单元格并根据移动选项移动单元格。 |
| [insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)](#insertRange-com.aspose.cells.CellArea-int-int-boolean-) | 插入一段单元格并根据移动选项移动单元格。 |
| [insertRow(int rowIndex)](#insertRow-int-) | 在工作表中插入新行。 |
| [insertRows(int rowIndex, int totalRows)](#insertRows-int-int-) | 在工作表中插入多行。 |
| [insertRows(int rowIndex, int totalRows, boolean updateReference)](#insertRows-int-int-boolean-) | 在工作表中插入多行。 |
| [insertRows(int rowIndex, int totalRows, InsertOptions options)](#insertRows-int-int-com.aspose.cells.InsertOptions-) | 在工作表中插入多行。 |
| [isBlankColumn(int columnIndex)](#isBlankColumn-int-) | 检查给定列是否为空（不包含任何数据）。 |
| [isColumnHidden(int columnIndex)](#isColumnHidden-int-) | 检查给定索引处的列是否隐藏。 |
| [isDefaultColumnHidden()](#isDefaultColumnHidden--) |  |
| [isDefaultRowHeightMatched()](#isDefaultRowHeightMatched--) | 指示行高与默认字体高度匹配。 |
| [isDefaultRowHidden()](#isDefaultRowHidden--) | 指示该行是否默认隐藏。 |
| [isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)](#isDeletingRangeEnabled-int-int-int-int-) | 检查该范围是否可以删除。 |
| [isRowHidden(int rowIndex)](#isRowHidden-int-) | 检查给定索引处的行是否隐藏。 |
| [iterator()](#iterator--) | 获取单元格枚举器。 |
| [linkToXmlMap(String mapName, int row, int column, String path)](#linkToXmlMap-java.lang.String-int-int-java.lang.String-) | 链接到 XML 映射。 |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#merge-int-int-int-int-) | 将指定范围的单元格合并为一个单元格。 |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)](#merge-int-int-int-int-boolean-) | 将指定范围的单元格合并为一个单元格。 |
| [merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)](#merge-int-int-int-int-boolean-boolean-) | 将指定范围的单元格合并为一个单元格。 |
| [moveRange(CellArea sourceArea, int destRow, int destColumn)](#moveRange-com.aspose.cells.CellArea-int-int-) | 移动该范围。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeDuplicates()](#removeDuplicates--) | 删除工作表中的重复行。 |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn)](#removeDuplicates-int-int-int-int-) | 删除范围内的重复值。 |
| [removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)](#removeDuplicates-int-int-int-int-boolean-int---) | 删除范围的重复数据。 |
| [removeFormulas()](#removeFormulas--) | 删除所有公式并替换为公式的值。 |
| [retrieveSubtotalSetting(CellArea ca)](#retrieveSubtotalSetting-com.aspose.cells.CellArea-) | 检索范围的子计数设置。 |
| [setColumnWidth(int column, double width)](#setColumnWidth-int-double-) | 在普通视图中设置指定列的宽度。 |
| [setColumnWidthInch(int column, double inches)](#setColumnWidthInch-int-double-) | 在普通视图中以英寸为单位设置列宽。 |
| [setColumnWidthPixel(int column, int pixels)](#setColumnWidthPixel-int-int-) | 在普通视图中以像素为单位设置列宽。 |
| [setDefaultColumnHidden(boolean value)](#setDefaultColumnHidden-boolean-) |  |
| [setDefaultRowHeightMatched(boolean value)](#setDefaultRowHeightMatched-boolean-) | 指示行高与默认字体高度匹配。 |
| [setDefaultRowHidden(boolean value)](#setDefaultRowHidden-boolean-) | 指示该行是否默认隐藏。 |
| [setMemorySetting(int value)](#setMemorySetting-int-) | 设置此单元格的内存使用选项。 |
| [setMultiThreadReading(boolean value)](#setMultiThreadReading-boolean-) | 设置单元格数据模型是否应支持多线程读取。 |
| [setPreserveString(boolean value)](#setPreserveString-boolean-) | 设置一个值，指示是否将所有工作表值保留为字符串。 |
| [setRowHeight(int row, double height)](#setRowHeight-int-double-) | 设置指定行的高度。 |
| [setRowHeightInch(int row, double inches)](#setRowHeightInch-int-double-) | 以英寸为单位设置行高。 |
| [setRowHeightPixel(int row, int pixels)](#setRowHeightPixel-int-int-) | 以像素为单位设置行高。 |
| [setStandardHeight(double value)](#setStandardHeight-double-) | 以磅为单位设置此工作表的默认行高。 |
| [setStandardHeightInch(double value)](#setStandardHeightInch-double-) | 以英寸为单位设置此工作表的默认行高。 |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | 以像素为单位设置此工作表的默认行高。 |
| [setStandardWidth(double value)](#setStandardWidth-double-) | 以字符为单位设置工作表的默认列宽。 |
| [setStandardWidthInch(double value)](#setStandardWidthInch-double-) | 以英寸为单位设置工作表的默认列宽。 |
| [setStandardWidthPixels(int value)](#setStandardWidthPixels-int-) | 以像素为单位设置工作表的默认列宽。 |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | 设置工作表的默认样式。 |
| [setViewColumnWidthPixel(int column, int pixels)](#setViewColumnWidthPixel-int-int-) | 在不同视图中设置列的宽度。 |
| [showGroupDetail(boolean isVertical, int index)](#showGroupDetail-boolean-int-) | 展开分组的行/列。 |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList)](#subtotal-com.aspose.cells.CellArea-int-int-int---) | 为范围创建小计。 |
| [subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)](#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-) | 为范围创建小计。 |
| [textToColumns(int row, int column, int totalRows, TxtLoadOptions options)](#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-) | 将指定列中的内容拆分为多个列.. |
| [toString()](#toString--) |  |
| [unMerge(int firstRow, int firstColumn, int totalRows, int totalColumns)](#unMerge-int-int-int-int-) | 取消合并指定范围的合并单元格。 |
| [ungroupColumns(int firstIndex, int lastIndex)](#ungroupColumns-int-int-) | 取消分组列。 |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | 取消分组行。 |
| [ungroupRows(int firstIndex, int lastIndex, boolean isAll)](#ungroupRows-int-int-boolean-) | 取消分组行。 |
| [unhideColumn(int column, double width)](#unhideColumn-int-double-) | 取消隐藏列 |
| [unhideColumns(int column, int totalColumns, double width)](#unhideColumns-int-int-double-) | 取消隐藏多个列。 |
| [unhideRow(int row, double height)](#unhideRow-int-double-) | 取消隐藏行。 |
| [unhideRows(int row, int totalRows, double height)](#unhideRows-int-int-double-) | 取消隐藏隐藏的行。 |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(Range rangeObject) {#addRange-com.aspose.cells.Range-}
```
public void addRange(Range rangeObject)
```


向单元格添加范围对象引用

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rangeObject | [Range](../../com.aspose.cells/range) | 范围对象将包含在单元格中 |

### applyColumnStyle(int column, Style style, StyleFlag flag) {#applyColumnStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyColumnStyle(int column, Style style, StyleFlag flag)
```


对整列应用格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| style | [Style](../../com.aspose.cells/style) | 将要应用的样式对象。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 指示已应用格式属性的标志。 |

### applyRowStyle(int row, Style style, StyleFlag flag) {#applyRowStyle-int-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyRowStyle(int row, Style style, StyleFlag flag)
```


对整行应用格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| style | [Style](../../com.aspose.cells/style) | 将要应用的样式对象。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 指示已应用格式属性的标志。 |

### applyStyle(Style style, StyleFlag flag) {#applyStyle-com.aspose.cells.Style-com.aspose.cells.StyleFlag-}
```
public void applyStyle(Style style, StyleFlag flag)
```


对整个工作表应用格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) | 将要应用的样式对象。 |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | 指示已应用格式属性的标志。 |

### checkCell(int row, int column) {#checkCell-int-int-}
```
public Cell checkCell(int row, int column)
```


获取指定单元格行索引和列索引处的 [Cell](../../com.aspose.cells/cell) 元素或 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |
| 列 | int | 列索引 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Return Cell object if a Cell object exists. Return null if the cell does not exist.
### checkColumn(int columnIndex) {#checkColumn-int-}
```
public Column checkColumn(int columnIndex)
```


获取指定列索引处的 [Column](../../com.aspose.cells/column) 元素或 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |

**Returns:**
[Column](../../com.aspose.cells/column) - The Column object.
### checkRow(int row) {#checkRow-int-}
```
public Row checkRow(int row)
```


获取指定单元格行索引处的 [Row](../../com.aspose.cells/row) 元素或 null。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |

**Returns:**
[Row](../../com.aspose.cells/row) - Returns [Row](../../com.aspose.cells/row) object If the row object does exist, otherwise returns null.
### clear() {#clear--}
```
public void clear()
```


清除工作表的所有数据。

### clearContents(CellArea range) {#clearContents-com.aspose.cells.CellArea-}
```
public void clearContents(CellArea range)
```


清除范围的内容。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | 要清除的范围。 |

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

### clearFormats(CellArea range) {#clearFormats-com.aspose.cells.CellArea-}
```
public void clearFormats(CellArea range)
```


清除范围的格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | 要清除的范围。 |

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

### clearMergedCells() {#clearMergedCells--}
```
public void clearMergedCells()
```


清除所有合并的范围。

### clearRange(CellArea range) {#clearRange-com.aspose.cells.CellArea-}
```
public void clearRange(CellArea range)
```


清除范围的内容和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| range | [CellArea](../../com.aspose.cells/cellarea) | 要清除的范围。 |

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

### convertStringToNumericValue() {#convertStringToNumericValue--}
```
public void convertStringToNumericValue()
```


将工作表中的所有字符串数据（如果可能）转换为数值。

### copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex) {#copyColumn-com.aspose.cells.Cells-int-int-}
```
public void copyColumn(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex)
```


复制整列的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells 对象包含要复制的数据和格式。 |
| sourceColumnIndex | int | 源列索引。 |
| destinationColumnIndex | int | 目标列索引。 |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber) {#copyColumns-com.aspose.cells.Cells-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber)
```


复制多列的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells 对象包含要复制的数据和格式。 |
| sourceColumnIndex | int | 源列索引。 |
| destinationColumnIndex | int | 目标列索引。 |
| columnNumber | int | 复制的列号。 |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions) {#copyColumns-com.aspose.cells.Cells-int-int-int-com.aspose.cells.PasteOptions-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int destinationColumnIndex, int columnNumber, PasteOptions pasteOptions)
```


复制整列的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells 对象包含要复制的数据和格式。 |
| sourceColumnIndex | int | 源列索引。 |
| destinationColumnIndex | int | 目标列索引。 |
| columnNumber | int | 复制的列号。 |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | 粘贴的选项。 |

### copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns) {#copyColumns-com.aspose.cells.Cells-int-int-int-int-}
```
public void copyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, int destinationColumnIndex, int destinationTotalColumns)
```


复制所有列的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells 对象包含要复制的数据和格式。 |
| sourceColumnIndex | int | 源列索引。 |
| sourceTotalColumns | int | 源列的数量。 |
| destinationColumnIndex | int | 目标列索引。 |
| destinationTotalColumns | int | 目标列的数量。 |

### copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex) {#copyRow-com.aspose.cells.Cells-int-int-}
```
public void copyRow(Cells sourceCells, int sourceRowIndex, int destinationRowIndex)
```


复制整行的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells 对象包含要复制的数据和格式。 |
| sourceRowIndex | int | 源行索引。 |
| destinationRowIndex | int | 目标行索引。 |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber) {#copyRows-com.aspose.cells.Cells-int-int-int-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```


复制若干整行的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells 对象包含要复制的数据和格式。 |
| sourceRowIndex | int | 源行索引。 |
| destinationRowIndex | int | 目标行索引。 |
| rowNumber | int | 复制的行号。 |

### copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-}
```
public void copyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions)
```


复制若干整行的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells | [Cells](../../com.aspose.cells/cells) | Source Cells 对象包含要复制的数据和格式。 |
| sourceRowIndex | int | 源行索引。 |
| destinationRowIndex | int | 目标行索引。 |
| rowNumber | int | 复制的行号。 |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | 复制选项。 |

### copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions) {#copyRows-com.aspose.cells.Cells-int-int-int-com.aspose.cells.CopyOptions-com.aspose.cells.PasteOptions-}
```
public void copyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```


复制若干整行的数据和格式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceCells0 | [Cells](../../com.aspose.cells/cells) | Source Cells 对象包含要复制的数据和格式。 |
| sourceRowIndex | int | 源行索引。 |
| destinationRowIndex | int | 目标行索引。 |
| rowNumber | int | 复制的行号。 |
| copyOptions | [CopyOptions](../../com.aspose.cells/copyoptions) | 复制选项。 |
| pasteOptions | [PasteOptions](../../com.aspose.cells/pasteoptions) | 粘贴的选项。 |

### createRange(int firstIndex, int number, boolean isVertical) {#createRange-int-int-boolean-}
```
public Range createRange(int firstIndex, int number, boolean isVertical)
```


从单元格的行或列创建一个 [Range](../../com.aspose.cells/range) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 第一行索引或第一列索引，零基。 |
| number | int | 行或列的总数，一基。 |
| isVertical | boolean | True - 范围由单元格的列创建。False - 范围由单元格的行创建。 |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object.
### createRange(int firstRow, int firstColumn, int totalRows, int totalColumns) {#createRange-int-int-int-int-}
```
public Range createRange(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


从单元格范围创建一个 [Range](../../com.aspose.cells/range) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 此范围的第一行 |
| firstColumn | int | 此范围的第一列 |
| totalRows | int | 行数 |
| totalColumns | int | 列数 |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String address) {#createRange-java.lang.String-}
```
public Range createRange(String address)
```


从范围地址创建一个 [Range](../../com.aspose.cells/range) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 地址 | java.lang.String | 范围的地址. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createRange(String upperLeftCell, String lowerRightCell) {#createRange-java.lang.String-java.lang.String-}
```
public Range createRange(String upperLeftCell, String lowerRightCell)
```


从单元格范围创建一个 [Range](../../com.aspose.cells/range) 对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| upperLeftCell | java.lang.String | 左上单元格名称。 |
| lowerRightCell | java.lang.String | 右下单元格名称。 |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### deleteBlankColumns() {#deleteBlankColumns--}
```
public void deleteBlankColumns()
```


删除所有不包含任何数据的空列。

### deleteBlankColumns(DeleteOptions options) {#deleteBlankColumns-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankColumns(DeleteOptions options)
```


删除所有不包含任何数据的空列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | 删除范围的选项。 |

### deleteBlankRows() {#deleteBlankRows--}
```
public void deleteBlankRows()
```


删除所有不包含任何数据或其他对象的空行。

### deleteBlankRows(DeleteOptions options) {#deleteBlankRows-com.aspose.cells.DeleteOptions-}
```
public void deleteBlankRows(DeleteOptions options)
```


删除所有不包含任何数据或某些特殊对象（如可见批注、数据透视表）的空行。

**Remarks**

对于将被删除的空白行，不仅要求 [Row.isBlank()](../../com.aspose.cells/row\#isBlank--) 为 true，还必须没有为这些行中的任何单元格定义可见的注释，并且没有其范围与这些行相交的数据透视表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | 删除范围的选项。 |

### deleteColumn(int columnIndex) {#deleteColumn-int-}
```
public void deleteColumn(int columnIndex)
```


删除一列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 要删除的列的索引。 |

### deleteColumn(int columnIndex, boolean updateReference) {#deleteColumn-int-boolean-}
```
public void deleteColumn(int columnIndex, boolean updateReference)
```


删除一列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 要删除的列的索引。 |
| updateReference | boolean | 指示是否在其他工作表中更新引用。 |

### deleteColumns(int columnIndex, int totalColumns, boolean updateReference) {#deleteColumns-int-int-boolean-}
```
public void deleteColumns(int columnIndex, int totalColumns, boolean updateReference)
```


删除多列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 要删除的第一列的索引。 |
| totalColumns | int | 要删除的列数。 |
| updateReference | boolean | 指示是否在其他工作表中更新引用。 |

### deleteColumns(int columnIndex, int totalColumns, DeleteOptions options) {#deleteColumns-int-int-com.aspose.cells.DeleteOptions-}
```
public void deleteColumns(int columnIndex, int totalColumns, DeleteOptions options)
```


删除多列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 要删除的第一列的索引。 |
| totalColumns | int | 要删除的列数。 |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | 删除操作的选项 |

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
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype)。移动单元格选项。 |

### deleteRow(int rowIndex) {#deleteRow-int-}
```
public void deleteRow(int rowIndex)
```


删除一行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 要删除的行的索引。 |

### deleteRow(int rowIndex, boolean updateReference) {#deleteRow-int-boolean-}
```
public void deleteRow(int rowIndex, boolean updateReference)
```


删除一行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 要删除的行的索引。 |
| updateReference | boolean | 指示是否在其他工作表中更新引用。 |

### deleteRows(int rowIndex, int totalRows) {#deleteRows-int-int-}
```
public boolean deleteRows(int rowIndex, int totalRows)
```


删除多行。

**Remarks**

如果被删除的范围包含表格（ListObject）的顶部部分（而不是全部），则该范围无法被删除，且不会执行任何操作。这在 MS Excel 中的表现相同。

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
| rowIndex | int | 要删除的第一行的索引。 |
| totalRows | int | 要删除的行数。 |
| updateReference | boolean | 指示是否在其他工作表中更新引用。 |

**Returns:**
boolean -
### deleteRows(int rowIndex, int totalRows, DeleteOptions options) {#deleteRows-int-int-com.aspose.cells.DeleteOptions-}
```
public boolean deleteRows(int rowIndex, int totalRows, DeleteOptions options)
```


删除工作表中的多行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 要删除的第一行的索引。 |
| totalRows | int | 要删除的行数。 |
| options | [DeleteOptions](../../com.aspose.cells/deleteoptions) | 删除操作的选项 |

**Returns:**
boolean -
### dispose() {#dispose--}
```
public void dispose()
```


执行应用程序定义的任务，以释放、释放或重置非托管资源。

### endCellInColumn(int columnIndex) {#endCellInColumn-int-}
```
public Cell endCellInColumn(int columnIndex)
```


获取此列中的最后一个单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInColumn(int startRow, int endRow, int startColumn, int endColumn) {#endCellInColumn-int-int-int-int-}
```
public Cell endCellInColumn(int startRow, int endRow, int startColumn, int endColumn)
```


获取此范围内列索引最大的最后一个单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| endRow | int | 结束行索引。 |
| startColumn | int | 起始列索引。 |
| endColumn | int | 结束列索引。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int rowIndex) {#endCellInRow-int-}
```
public Cell endCellInRow(int rowIndex)
```


获取此行中的最后一个单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### endCellInRow(int startRow, int endRow, int startColumn, int endColumn) {#endCellInRow-int-int-int-int-}
```
public Cell endCellInRow(int startRow, int endRow, int startColumn, int endColumn)
```


获取此范围内行索引最大的最后一个单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行索引。 |
| endRow | int | 结束行索引。 |
| startColumn | int | 起始列索引。 |
| endColumn | int | 结束列索引。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
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


将 [Cells](../../com.aspose.cells/cells) 集合中的数据导出为二维数组对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 要导出的第一个单元格的行号。 |
| firstColumn | int | 要导出的第一个单元格的列号。 |
| totalRows | int | 要导出的行数 |
| totalColumns | int | 要导出的列数 |

**Returns:**
java.lang.Object[][] - 导出的单元格值数组对象。
### exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns) {#exportTypeArray-int-int-int-int-}
```
public int[][] exportTypeArray(int firstRow, int firstColumn, int totalRows, int totalColumns)
```


将 [Cells](../../com.aspose.cells/cells) 集合中的单元格值类型导出为二维数组对象。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 要导出的第一个单元格的行号。 |
| firstColumn | int | 要导出的第一个单元格的列号。 |
| totalRows | int | 要导出的行数。 |
| totalColumns | int | 要导出的列数。 |

**Returns:**
int[][] - [CellValueType](../../com.aspose.cells/cellvaluetype)。表示单元格值类型的导出数组对象。
### find(Object what, Cell previousCell) {#find-java.lang.Object-com.aspose.cells.Cell-}
```
public Cell find(Object what, Cell previousCell)
```


查找包含输入对象的单元格。

**Remarks**

如果未找到单元格，则返回 null（Nothing）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 什么 | java.lang.Object | 要搜索的对象。类型应为 int、double、DateTime、string、bool。 |
| previousCell | [Cell](../../com.aspose.cells/cell) | 具有相同对象的前一个单元格。如果从头开始搜索，此参数可以设为 null。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### find(Object what, Cell previousCell, FindOptions findOptions) {#find-java.lang.Object-com.aspose.cells.Cell-com.aspose.cells.FindOptions-}
```
public Cell find(Object what, Cell previousCell, FindOptions findOptions)
```


查找包含输入对象的单元格。

**Remarks**

如果未找到单元格，则返回 null（Nothing）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 什么 | java.lang.Object | 要搜索的对象。类型应为 int、double、DateTime、string、bool。 |
| previousCell | [Cell](../../com.aspose.cells/cell) | 具有相同对象的前一个单元格。如果从头开始搜索，此参数可以设为 null。 |
| findOptions | [FindOptions](../../com.aspose.cells/findoptions) | 查找选项 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - Cell object.
### get(int row, int column) {#get-int-int-}
```
public Cell get(int row, int column)
```


获取指定单元格行索引和列索引处的 [Cell](../../com.aspose.cells/cell) 元素。

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get(0, 0);	//Gets the cell at "A1"
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - The [Cell](../../com.aspose.cells/cell) object.
### get(String cellName) {#get-java.lang.String-}
```
public Cell get(String cellName)
```


获取指定单元格名称处的 [Cell](../../com.aspose.cells/cell) 元素。

**Example**

```
         Workbook excel = new Workbook();
         Cells cells = excel.getWorksheets().get(0).getCells();
         Cell cell = cells.get("A1");	//Gets the cell at "A1"
```

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cellName | java.lang.String | 单元格名称，包括其列字母和行号，例如 A5。 |

**Returns:**
[Cell](../../com.aspose.cells/cell) - A [Cell](../../com.aspose.cells/cell) object
### getCellDisplayStyle(int row, int column) {#getCellDisplayStyle-int-int-}
```
public Style getCellDisplayStyle(int row, int column)
```


获取给定单元格的显示样式。

**Remarks**

与 [Cell.getDisplayStyle()](../../com.aspose.cells/cell\#getDisplayStyle--) 相同，使用 [BorderType.SIDE\_BORDERS](../../com.aspose.cells/bordertype\#SIDE-BORDERS) 对于 [getCellDisplayStyle(int,int,int)](../../com.aspose.cells/cells\#getCellDisplayStyle-int-int-int-) 也是相同的。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 给定单元格的行索引 |
| 列 | int | 给定单元格的列 |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellDisplayStyle(int row, int column, int adjacentBorders) {#getCellDisplayStyle-int-int-int-}
```
public Style getCellDisplayStyle(int row, int column, int adjacentBorders)
```


获取给定单元格的显示样式。

**Remarks**

如果单元格还受到其他设置的影响，例如条件格式、列表对象等，则显示样式可能与 [getCellStyle(int,int)](../../com.aspose.cells/cells\#getCellStyle-int-int-) 不同。而且由于这些设置也可能应用于空（不存在）的单元格，使用此方法可以避免实例化这些空单元格，从而性能优于从 Cells 获取 Cell 实例后再调用 [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 给定单元格的行索引 |
| 列 | int | 给定单元格的列 |
| adjacentBorders | int | [BorderType](../../com.aspose.cells/bordertype)。指示需要根据相邻单元格的边框检查和调整的边框。请参阅 [Cell.getDisplayStyle(int)](../../com.aspose.cells/cell\#getDisplayStyle-int-) 参数的描述。 |

**Returns:**
[Style](../../com.aspose.cells/style) - the display style of given cell.
### getCellStyle(int row, int column) {#getCellStyle-int-int-}
```
public Style getCellStyle(int row, int column)
```


获取给定单元格的样式。

**Remarks**

返回的样式仅为单元格设置的样式或从单元格所在的行/列继承的样式，不包括其他设置（如条件格式）所应用的属性。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |
| 列 | int | 列 |

**Returns:**
[Style](../../com.aspose.cells/style) - the style of given cell.
### getCellsWithPlaceInCellPicture() {#getCellsWithPlaceInCellPicture--}
```
public Iterator getCellsWithPlaceInCellPicture()
```


获取所有包含嵌入图片的单元格。

**Remarks**

如果此工作表中没有设置为“放置在单元格”的图片，则返回 null。

**Returns:**
java.util.Iterator - 用于枚举所有包含嵌入图片的 Cell 对象的枚举器
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnOriginalWidthPoint(int column) {#getColumnOriginalWidthPoint-int-}
```
public double getColumnOriginalWidthPoint(int column)
```


如果列被隐藏，获取原始列的高度（单位为点）。

**Remarks**

注意：此方法现已过时。请改用 Cells.GetColumnWidth(int ,bool , CellsUnitType ) 方法。该方法将在自 2024 年 4 月起的 12 个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 行索引。 |

**Returns:**
double - 正常视图下列的宽度。
### getColumnWidth(int column) {#getColumnWidth-int-}
```
public double getColumnWidth(int column)
```


获取指定列在普通视图中的宽度（以字符为单位）

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

**Returns:**
double - 列的宽度。对于电子表格，列宽以在普通样式字体中渲染的数字 0~9 的最大数字宽度对应的字符数来衡量。
### getColumnWidth(int column, boolean isOriginal, int unitType) {#getColumnWidth-int-boolean-int-}
```
public double getColumnWidth(int column, boolean isOriginal, int unitType)
```


获取列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| isOriginal | boolean | 指示是否获取原始宽度。 |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype)。 |

**Returns:**
double -
### getColumnWidthInch(int column) {#getColumnWidthInch-int-}
```
public double getColumnWidthInch(int column)
```


获取指定列在普通视图中的宽度（单位为英寸）。

**Remarks**

注意：此方法现已过时。请改用 Cells.GetColumnWidth(int ,bool , CellsUnitType ) 方法。该方法将在自 2024 年 4 月起的 12 个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

**Returns:**
double - 正常视图下列的宽度。
### getColumnWidthPixel(int column) {#getColumnWidthPixel-int-}
```
public int getColumnWidthPixel(int column)
```


获取指定列在普通视图中的宽度（单位为像素）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |

**Returns:**
int - 正常视图下列的宽度。
### getColumnWidthPixel(int column, boolean original) {#getColumnWidthPixel-int-boolean-}
```
public int getColumnWidthPixel(int column, boolean original)
```


获取指定列在普通视图中的宽度（单位为像素）。

**Remarks**

注意：此方法现已过时。请改用 Cells.GetColumnWidth(int ,bool , CellsUnitType ) 方法。该方法将在自 2024 年 4 月起的 12 个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引 |
| 原始 | boolean | 指示即使列被隐藏也返回原始宽度 |

**Returns:**
int - 正常视图下列的宽度。
### getColumns() {#getColumns--}
```
public ColumnCollection getColumns()
```


获取表示此工作表中各列的 [Column](../../com.aspose.cells/column) 对象集合。

**Returns:**
[ColumnCollection](../../com.aspose.cells/columncollection)
### getCount() {#getCount--}
```
public int getCount()
```


获取已实例化的 Cell 对象的总数。

**Returns:**
int
### getCountLarge() {#getCountLarge--}
```
public long getCountLarge()
```


获取已实例化的 Cell 对象的总数。

**Returns:**
long
### getDependents(boolean isAll, int row, int column) {#getDependents-boolean-int-int-}
```
public Cell[] getDependents(boolean isAll, int row, int column)
```


获取所有引用特定单元格的单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isAll | boolean | 指示是否检查其他工作表 |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |

**Returns:**
com.aspose.cells.Cell[] -
### getDependentsInCalculation(int row, int column, boolean recursive) {#getDependentsInCalculation-int-int-boolean-}
```
public Iterator getDependentsInCalculation(int row, int column, boolean recursive)
```


获取所有其计算结果依赖于特定单元格的单元格。

**Remarks**

要使用此方法，请确保工作簿已将 [FormulaSettings.getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) 设置为 true，并已使用此设置完成全部计算。如果没有对该单元格的公式引用，则返回 null。有关更多详细信息和示例，请参阅 [Cell.getDependentsInCalculation(boolean)](../../com.aspose.cells/cell\#getDependentsInCalculation-boolean-)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 特定单元格的行索引 |
| 列 | int | 特定单元格的列索引。 |
| recursive | boolean | 指示是否返回那些未直接引用特定单元格但引用该单元格其他叶子节点的依赖项。 |

**Returns:**
java.util.Iterator - 用于枚举所有从属项（单元格对象）的枚举器
### getFirstCell() {#getFirstCell--}
```
public Cell getFirstCell()
```


获取此工作表中的第一个单元格。

**Remarks**

如果工作表中没有数据，则返回 null。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getFirstDataRow(int column) {#getFirstDataRow-int-}
```
public int getFirstDataRow(int column)
```


获取指定列中包含数据的单元格的第一行索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

**Returns:**
int - 第一个行索引。
### getGroupedColumnOutlineLevel(int columnIndex) {#getGroupedColumnOutlineLevel-int-}
```
public int getGroupedColumnOutlineLevel(int columnIndex)
```


获取列的轮廓级别（从零开始计）。

**Remarks**

如果列未分组，则返回零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引 |

**Returns:**
int - 列的大纲级别
### getGroupedRowOutlineLevel(int rowIndex) {#getGroupedRowOutlineLevel-int-}
```
public int getGroupedRowOutlineLevel(int rowIndex)
```


获取行的轮廓级别（从零开始计）。

**Remarks**

如果行未分组，则返回零。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |

**Returns:**
int - 行的大纲级别（从零开始）。
### getLastCell() {#getLastCell--}
```
public Cell getLastCell()
```


获取此工作表中的最后一个单元格。

**Remarks**

如果工作表中没有数据，则返回 null。

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getLastDataRow(int column) {#getLastDataRow-int-}
```
public int getLastDataRow(int column)
```


获取指定列中包含数据的单元格的最后一行索引。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

**Returns:**
int - 最后行索引。
### getMaxColumn() {#getMaxColumn--}
```
public int getMaxColumn()
```


集合中已实例化的单元格的最大列索引（不包括为整列定义了样式但未实例化任何单元格的列）。

**Remarks**

如果没有已实例化的单元格，则返回 -1。

**Returns:**
int
### getMaxDataColumn() {#getMaxDataColumn--}
```
public int getMaxDataColumn()
```


包含数据的单元格的最大列索引。

**Remarks**

-1 将在没有包含数据的单元格时返回。此属性需要动态遍历并检查工作表中的所有单元格，因此这是一个耗时的过程，不应重复调用，例如在循环中直接将其用作条件。

**Returns:**
int
### getMaxDataRow() {#getMaxDataRow--}
```
public int getMaxDataRow()
```


包含数据的单元格的最大行索引。

**Remarks**

如果没有包含数据的单元格，则返回 -1。此属性需要动态遍历并检查单元格和行，因此这是一个耗时的过程，不应重复调用，例如在循环中直接将其用作条件。

**Returns:**
int
### getMaxDisplayRange() {#getMaxDisplayRange--}
```
public Range getMaxDisplayRange()
```


获取包括数据、合并单元格和形状的最大范围。

**Remarks**

如果工作表为空，则返回 null（自 Aspose.Cells 21.5.2 起）。

**Returns:**
[Range](../../com.aspose.cells/range)
### getMaxGroupedColumnOutlineLevel() {#getMaxGroupedColumnOutlineLevel--}
```
public int getMaxGroupedColumnOutlineLevel()
```


获取最大分组列的轮廓级别（从零开始计）。

**Returns:**
int - 最大分组列大纲级别（零基）。
### getMaxGroupedRowOutlineLevel() {#getMaxGroupedRowOutlineLevel--}
```
public int getMaxGroupedRowOutlineLevel()
```


获取最大分组行的轮廓级别（从零开始计）。

**Returns:**
int - 最大分组行大纲级别（零基）。
### getMaxRow() {#getMaxRow--}
```
public int getMaxRow()
```


包含数据或样式的单元格的最大行索引。

**Remarks**

如果工作表中没有包含数据或样式的单元格，则返回 -1。此属性需要动态遍历并检查单元格和行，因此这是一个耗时的过程，不应重复调用，例如在循环中直接将其用作条件。

**Returns:**
int
### getMemorySetting() {#getMemorySetting--}
```
public int getMemorySetting()
```


获取此单元格的内存使用选项。

参见 [MemorySetting](../../com.aspose.cells/memorysetting)。

**Remarks**

某些模式的显著限制和推荐操作：

| 模式 | 备注 | 支持 |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | 当在同一工作簿的任何工作表中使用此模式时，应在工作结束时调用[Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--)以释放所有资源，例如临时文件。 |
 
随机访问单元格会导致性能下降，因为数据需要随机且反复读取/更新（因此文件指针会相应改变，并且需要重复的 IO 操作）。如果可能，请始终顺序访问数据（逐行）。
 
当某一行/单元格的数据被更改时，其他单元格/行的数据可能也会受到影响（例如数据被移位/移动到其他位置以为更改后的数据分配足够的空间）。因此，每一次数据的更改都需要同步其他已有对象（例如 Row 或 Cell 对象）。为了获得更好的性能，请不要同时维护多个 Row/Cell。逐个处理它们可以减少数据同步，从而略微提升性能。 | v25.7     |

**Returns:**
int
### getMergedAreas() {#getMergedAreas--}
```
public CellArea[] getMergedAreas()
```


获取所有合并的单元格。

**Returns:**
com.aspose.cells.CellArea[]
### getMergedCells() {#getMergedCells--}
```
public ArrayList getMergedCells()
```


获取合并单元格的集合。

**Remarks**

注意：此方法现已过时。请改用 Cells.GetMergedAreas() 方法。该方法将在自 2023 年 11 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.util.ArrayList
### getMinColumn() {#getMinColumn--}
```
public int getMinColumn()
```


集合中已实例化的单元格的最小列索引（不包括为整列定义了样式但未实例化任何单元格的列）。

**Remarks**

此属性需要动态遍历并检查单元格和行，因此这是一个耗时的过程，不应重复调用，例如在循环中直接将其用作条件。

**Returns:**
int
### getMinDataColumn() {#getMinDataColumn--}
```
public int getMinDataColumn()
```


包含数据的单元格的最小列索引。

**Remarks**

-1 将在没有包含数据的单元格时返回。此属性需要动态遍历并检查工作表中的所有单元格，因此这是一个耗时的过程，不应重复调用，例如在循环中直接将其用作条件。

**Returns:**
int
### getMinDataRow() {#getMinDataRow--}
```
public int getMinDataRow()
```


包含数据的单元格的最小行索引。

**Remarks**

如果没有包含数据的单元格，则返回 -1。此属性需要动态遍历并检查单元格和行，因此这是一个耗时的过程，不应重复调用，例如在循环中直接将其用作条件。

**Returns:**
int
### getMinRow() {#getMinRow--}
```
public int getMinRow()
```


包含数据或样式的单元格的最小行索引。

**Remarks**

此属性需要动态遍历并检查单元格和行，因此这是一个耗时的过程，不应重复调用，例如在循环中直接将其用作条件。

**Returns:**
int
### getMultiThreadReading() {#getMultiThreadReading--}
```
public boolean getMultiThreadReading()
```


获取单元格数据模型是否应支持多线程读取。此属性的默认值为 false。

**Remarks**

如果有多个线程并发读取此集合中的 Row/Cell 对象，则应将此属性设为 true，否则可能产生意外结果。支持多线程读取可能会降低访问此集合中 Row/Cell 对象的性能。请注意，某些功能无法支持多线程读取，例如格式化值（通过 [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)、[Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--) 等）。因此，即使此属性被设为 true，这些 API 在多线程读取时仍可能产生意外结果。

**Returns:**
boolean
### getOdsCellFields() {#getOdsCellFields--}
```
public OdsCellFieldCollection getOdsCellFields()
```


获取 ods 的字段列表。

**Returns:**
[OdsCellFieldCollection](../../com.aspose.cells/odscellfieldcollection)
### getPreserveString() {#getPreserveString--}
```
public boolean getPreserveString()
```


获取一个值，指示是否将所有工作表值保留为字符串。默认值为 false。

**Returns:**
boolean
### getRanges() {#getRanges--}
```
public RangeCollection getRanges()
```


获取在运行时创建的 [Range](../../com.aspose.cells/range) 对象集合。

**Returns:**
[RangeCollection](../../com.aspose.cells/rangecollection)
### getRowEnumerator() {#getRowEnumerator--}
```
public Iterator getRowEnumerator()
```


获取行枚举器。

**Remarks**

注意：此成员现已过时。请改用 RowCollection.GetEnumerator() 方法。该方法将在自 2023 年 5 月起的 12 个月后被移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.util.Iterator - 行枚举器。
### getRowHeight(int row) {#getRowHeight-int-}
```
public double getRowHeight(int row)
```


获取指定行的高度，单位为点。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |

**Returns:**
double - 行高。
### getRowHeight(int row, boolean isOriginal, int unitType) {#getRowHeight-int-boolean-int-}
```
public double getRowHeight(int row, boolean isOriginal, int unitType)
```


获取行的高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| isOriginal | boolean | 是否返回原始行高，隐藏行则返回 0。 |
| unitType | int | [CellsUnitType](../../com.aspose.cells/cellsunittype)。返回的高度值的单位类型 |

**Returns:**
double - 行的高度
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
### getRowOriginalHeightPoint(int row) {#getRowOriginalHeightPoint-int-}
```
public double getRowOriginalHeightPoint(int row)
```


如果行被隐藏，获取原始行的高度，单位为点

**Remarks**

注意：此成员已过时。请改用 Cells.GetRowHeight(int,bool,CellsUnitType) 方法。此方法将在自2024年4月起的12个月后被移除。Aspose 对给您带来的任何不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |

**Returns:**
double -
### getRows() {#getRows--}
```
public RowCollection getRows()
```


获取表示此工作表中各个行的 [Row](../../com.aspose.cells/row) 对象集合。

**Returns:**
[RowCollection](../../com.aspose.cells/rowcollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


获取此工作表的默认行高，单位为点。

**Returns:**
double
### getStandardHeightInch() {#getStandardHeightInch--}
```
public double getStandardHeightInch()
```


获取此工作表的默认行高，单位为英寸。

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


获取此工作表的默认行高，单位为像素。

**Returns:**
int
### getStandardWidth() {#getStandardWidth--}
```
public double getStandardWidth()
```


获取工作表的默认列宽，单位为字符。

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
### getStyle() {#getStyle--}
```
public Style getStyle()
```


获取工作表的默认样式。

**Returns:**
[Style](../../com.aspose.cells/style)
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
### getViewRowHeight(int row) {#getViewRowHeight-int-}
```
public double getViewRowHeight(int row)
```


获取指定行的高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |

**Returns:**
double - 行的高度。
### getViewRowHeightInch(int row) {#getViewRowHeightInch-int-}
```
public double getViewRowHeightInch(int row)
```


获取指定行的高度，单位为英寸。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引 |

**Returns:**
double - 行高。
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
### hideColumn(int column) {#hideColumn-int-}
```
public void hideColumn(int column)
```


隐藏列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |

### hideColumns(int column, int totalColumns) {#hideColumns-int-int-}
```
public void hideColumns(int column, int totalColumns)
```


隐藏多列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| totalColumns | int | 列号。 |

### hideGroupDetail(boolean isVertical, int index) {#hideGroupDetail-boolean-int-}
```
public void hideGroupDetail(boolean isVertical, int index)
```


折叠已分组的行/列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isVertical | boolean | True，折叠分组的行。 |
| 索引 | int | 行/列索引 |

### hideRow(int row) {#hideRow-int-}
```
public void hideRow(int row)
```


隐藏行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |

### hideRows(int row, int totalRows) {#hideRows-int-int-}
```
public void hideRows(int row, int totalRows)
```


隐藏多行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| totalRows | int | 行号。 |

### importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-double---int-int-boolean-}
```
public void importArray(double[] doubleArray, int firstRow, int firstColumn, boolean isVertical)
```


将 double 数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| doubleArray | double[] | 双精度数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| isVertical | boolean | 指定以垂直或水平方式导入数据。 |

### importArray(double[][] doubleArray, int firstRow, int firstColumn) {#importArray-double-----int-int-}
```
public void importArray(double[][] doubleArray, int firstRow, int firstColumn)
```


将 double 类型的二维数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| doubleArray | double[][] | 二维双精度数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |

### importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-int---int-int-boolean-}
```
public void importArray(int[] intArray, int firstRow, int firstColumn, boolean isVertical)
```


将整数数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| intArray | int[] | 整数数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| isVertical | boolean | 指定以垂直或水平方式导入数据。 |

### importArray(int[][] intArray, int firstRow, int firstColumn) {#importArray-int-----int-int-}
```
public void importArray(int[][] intArray, int firstRow, int firstColumn)
```


将整数的二维数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| intArray | int[][] | 二维整数数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |

### importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importArray-java.lang.String---int-int-boolean-}
```
public void importArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


将字符串数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringArray | java.lang.String[] | 字符串数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| isVertical | boolean | 指定以垂直或水平方式导入数据。 |

### importArray(String[][] stringArray, int firstRow, int firstColumn) {#importArray-java.lang.String-----int-int-}
```
public void importArray(String[][] stringArray, int firstRow, int firstColumn)
```


将字符串的二维数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringArray | java.lang.String[][] | 二维字符串数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |

### importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical) {#importArrayList-java.util.ArrayList-int-int-boolean-}
```
public void importArrayList(ArrayList arrayList, int firstRow, int firstColumn, boolean isVertical)
```


将数据的 ArrayList 导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arrayList | java.util.ArrayList | 数据 arraylist。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| isVertical | boolean | 指定以垂直或水平方式导入数据。 |

### importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(InputStream stream, TxtLoadOptions options, int firstRow, int firstColumn)
```


将 CSV 文件导入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | CSV 文件流。 |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | 读取文本文件的加载选项 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |

### importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.io.InputStream-java.lang.String-boolean-int-int-}
```
public void importCSV(InputStream stream, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


将 CSV 文件导入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stream | java.io.InputStream | CSV 文件流。 |
| splitter | java.lang.String | 分割器 |
| convertNumericData | boolean | 文本文件中的字符串是否转换为数值数据。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |

### importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn) {#importCSV-java.lang.String-com.aspose.cells.TxtLoadOptions-int-int-}
```
public void importCSV(String fileName, TxtLoadOptions options, int firstRow, int firstColumn)
```


将 CSV 文件导入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | CSV 文件名。 |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | 读取文本文件的加载选项 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |

### importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn) {#importCSV-java.lang.String-java.lang.String-boolean-int-int-}
```
public void importCSV(String fileName, String splitter, boolean convertNumericData, int firstRow, int firstColumn)
```


将 CSV 文件导入单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| fileName | java.lang.String | CSV 文件名。 |
| splitter | java.lang.String | 分割器 |
| convertNumericData | boolean | 文本文件中的字符串是否转换为数值数据。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |

### importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options) {#importCustomObjects-java.util.Collection-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importCustomObjects(Collection list, int firstRow, int firstColumn, ImportTableOptions options)
```


导入自定义对象。

**Remarks**

自定义对象应具有相同的类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| list | java.util.Collection | 自定义对象 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | 导入选项。 |

**Returns:**
int - 导入的总行数。
### importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber) {#importCustomObjects-java.util.Collection-java.lang.String---boolean-int-int-int-boolean-java.lang.String-boolean-}
```
public int importCustomObjects(Collection list, String[] propertyNames, boolean isPropertyNameShown, int firstRow, int firstColumn, int rowNumber, boolean insertRows, String dateFormatString, boolean convertStringToNumber)
```


导入自定义对象。

**Remarks**

自定义对象应具有相同的类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| list | java.util.Collection | 自定义对象 |
| propertyNames | java.lang.String[] | 属性名称。如果为 null，我们将导入对象的所有属性。 |
| isPropertyNameShown | boolean | 指示属性名称是否将导入到第一行。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| rowNumber | int | 要导入的行数。 |
| insertRows | boolean | 指示是否添加额外的行以适应数据。 |
| dateFormatString | java.lang.String | 单元格的日期格式字符串。 |
| convertStringToNumber | boolean | 指示此方法是否会尝试将字符串转换为数字。 |

**Returns:**
int - 导入的总行数。
### importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options) {#importData-com.aspose.cells.ICellsDataTable-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importData(ICellsDataTable table, int firstRow, int firstColumn, ImportTableOptions options)
```


从自定义数据表导入数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| table | [ICellsDataTable](../../com.aspose.cells/icellsdatatable) | 自定义数据表。 |
| firstRow | int | 第一行索引。 |
| firstColumn | int | 第一列索引。 |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | 导入选项 |

**Returns:**
int -
### importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical) {#importFormulaArray-java.lang.String---int-int-boolean-}
```
public void importFormulaArray(String[] stringArray, int firstRow, int firstColumn, boolean isVertical)
```


将公式数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| stringArray | java.lang.String[] | 公式数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| isVertical | boolean | 指定以垂直或水平方式导入数据。 |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical) {#importObjectArray-java.lang.Object---int-int-boolean-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical)
```


将数据数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| objArray | java.lang.Object[] | 数据数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| isVertical | boolean | 指定以垂直或水平方式导入数据。 |

### importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip) {#importObjectArray-java.lang.Object---int-int-boolean-int-}
```
public void importObjectArray(Object[] objArray, int firstRow, int firstColumn, boolean isVertical, int skip)
```


将数据数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| objArray | java.lang.Object[] | 数据数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| isVertical | boolean | 指定以垂直或水平方式导入数据。 |
| skip | int | 已跳过的行或列数。 |

### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown)
```


将 ResultSet 对象中的数据导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 要导入的 ResultSet 对象。 |
| rowIndex | int | 工作表中的起始行索引。 |
| columnIndex | int | 工作表中的起始列索引。 |
| isFieldNameShown | boolean | 指示结果集的字段名称是否将导入到第一行。 |

**Returns:**
int - 实际导入的行数。
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


将 ResultSet 对象中的数据导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 要导入的 ResultSet 对象。 |
| rowIndex | int | 工作表中的起始行索引。 |
| columnIndex | int | 工作表中的起始列索引。 |
| isFieldNameShown | boolean | 指示结果集的字段名称是否将导入到第一行。 |
| customDateFormatString | java.lang.String | 用于包含日期值的单元格的日期格式字符串。 |
| convertStringToNumber | boolean | 指示此方法是否会尝试将字符串转换为数字。 |

**Returns:**
int - 实际导入的行数。
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-int-int-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, ImportTableOptions options)
```


将 ResultSet 对象中的数据导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 要导入的 ResultSet 对象。 |
| rowIndex | int | 工作表中的起始行索引。 |
| columnIndex | int | 工作表中的起始列索引。 |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | 导入选项 |

**Returns:**
int - 实际导入的行数。
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown)
```


将 ResultSet 对象中的数据导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 要导入的 ResultSet 对象。 |
| rowIndex | int | 工作表中的起始行索引。 |
| columnIndex | int | 工作表中的起始列索引。 |
| rowNum | int | 要导入的行数。-1 表示导入给定结果集中的所有记录。 |
| columnNum | int | 要导入的列数。-1 表示导入给定结果集中的所有列。 |
| isFieldNameShown | boolean | 指示结果集的字段名称是否将导入到第一行。 |

**Returns:**
int - 实际导入的行数。
### importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber) {#importResultSet-java.sql.ResultSet-int-int-int-int-boolean-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, int rowIndex, int columnIndex, int rowNum, int columnNum, boolean isFieldNameShown, String customDateFormatString, boolean convertStringToNumber)
```


将 ResultSet 对象中的数据导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 要导入的 ResultSet 对象。 |
| rowIndex | int | 工作表中的起始行索引。 |
| columnIndex | int | 工作表中的起始列索引。 |
| rowNum | int | 要导入的行数。-1 表示导入给定结果集中的所有记录。 |
| columnNum | int | 要导入的列数。-1 表示导入给定结果集中的所有列。 |
| isFieldNameShown | boolean | 指示结果集的字段名称是否将导入到第一行。 |
| customDateFormatString | java.lang.String | 用于包含日期值的单元格的日期格式字符串。 |
| convertStringToNumber | boolean | 指示此方法是否会尝试将字符串转换为数字。 |

**Returns:**
int - 实际导入的行数。
### importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, boolean isFieldNameShown)
```


将 ResultSet 对象中的数据导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 要导入的 ResultSet 对象。 |
| startCell | java.lang.String | 插入结果集的起始单元格名称，例如 "A1"。 |
| isFieldNameShown | boolean | 指示结果集的字段名称是否将导入到第一行。 |

**Returns:**
int - 实际导入的行数。
### importResultSet(ResultSet rs, String startCell, ImportTableOptions options) {#importResultSet-java.sql.ResultSet-java.lang.String-com.aspose.cells.ImportTableOptions-}
```
public int importResultSet(ResultSet rs, String startCell, ImportTableOptions options)
```


将 ResultSet 对象中的数据导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 要导入的 ResultSet 对象。 |
| startCell | java.lang.String | 插入结果集的起始单元格名称，例如 "A1"。 |
| options | [ImportTableOptions](../../com.aspose.cells/importtableoptions) | 导入选项 |

**Returns:**
int - 实际导入的行数。
### importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown) {#importResultSet-java.sql.ResultSet-java.lang.String-int-int-boolean-}
```
public int importResultSet(ResultSet rs, String startCell, int rowNum, int columnNum, boolean isFieldNameShown)
```


将 ResultSet 对象中的数据导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rs | java.sql.ResultSet | 要导入的 ResultSet 对象。 |
| startCell | java.lang.String | 插入结果集的起始单元格名称，例如 "A1"。 |
| rowNum | int | 要导入的行数。-1 表示导入给定结果集中的所有记录。 |
| columnNum | int | 要导入的列数。-1 表示导入给定结果集中的所有列。 |
| isFieldNameShown | boolean | 指示结果集的字段名称是否将导入到第一行。 |

**Returns:**
int - 实际导入的行数。
### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn) {#importTwoDimensionArray-java.lang.Object-----int-int-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn)
```


将数据的二维数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| objArray | java.lang.Object[][] | 二维数据数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |

### importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, int firstRow, int firstColumn, boolean convertStringToNumber)
```


将数据的二维数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| objArray | java.lang.Object[][] | 二维数据数组。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| convertStringToNumber | boolean | 指示此方法是否会尝试将字符串转换为数字。 |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-boolean-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, boolean convertStringToNumber)
```


将数据的二维数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| objArray | java.lang.Object[][] | 二维数据数组。 |
| 样式 | java.lang.Object[][] | 二维数据样式。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| convertStringToNumber | boolean | 指示此方法是否会尝试将字符串转换为数字。 |

### importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts) {#importTwoDimensionArray-java.lang.Object-----java.lang.Object-----int-int-com.aspose.cells.TxtLoadOptions-}
```
public void importTwoDimensionArray(Object[][] objArray, Object[][] styles, int firstRow, int firstColumn, TxtLoadOptions opts)
```


将数据的二维数组导入工作表。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| objArray | java.lang.Object[][] | 二维数据数组。 |
| 样式 | java.lang.Object[][] | 二维数据样式。 |
| firstRow | int | 要导入的第一个单元格所在的行号。 |
| firstColumn | int | 要导入的第一个单元格所在的列号。 |
| opts | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | 字符串值转换选项 |

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

### insertColumns(int columnIndex, int totalColumns, InsertOptions options) {#insertColumns-int-int-com.aspose.cells.InsertOptions-}
```
public void insertColumns(int columnIndex, int totalColumns, InsertOptions options)
```


在工作表中插入若干列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| columnIndex | int | 列索引。 |
| totalColumns | int | 列的数量。 |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | 插入操作的选项。 |

### insertCutCells(Range cutRange, int row, int column, int shiftType) {#insertCutCells-com.aspose.cells.Range-int-int-int-}
```
public void insertCutCells(Range cutRange, int row, int column, int shiftType)
```


插入剪切范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| cutRange | [Range](../../com.aspose.cells/range) | 剪切范围。 |
| 行 | int | 行。 |
| 列 | int | 列。 |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype)。指示在插入剪切范围时如何移动目标范围的其他对象。 |

### insertRange(CellArea area, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-}
```
public void insertRange(CellArea area, int shiftType)
```


插入一段单元格并根据移动选项移动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | 移动区域。 |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype)。移动单元格选项。 |

### insertRange(CellArea area, int shiftNumber, int shiftType) {#insertRange-com.aspose.cells.CellArea-int-int-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType)
```


插入一段单元格并根据移动选项移动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | 移动区域。 |
| shiftNumber | int | 要插入的行数或列数。 |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype)。移动单元格选项。 |

### insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference) {#insertRange-com.aspose.cells.CellArea-int-int-boolean-}
```
public void insertRange(CellArea area, int shiftNumber, int shiftType, boolean updateReference)
```


插入一段单元格并根据移动选项移动单元格。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| area | [CellArea](../../com.aspose.cells/cellarea) | 移动区域。 |
| shiftNumber | int | 要插入的行数或列数。 |
| shiftType | int | [ShiftType](../../com.aspose.cells/shifttype)。移动单元格选项。 |
| updateReference | boolean | 指示是否在其他工作表中更新引用。 |

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

### insertRows(int rowIndex, int totalRows, InsertOptions options) {#insertRows-int-int-com.aspose.cells.InsertOptions-}
```
public void insertRows(int rowIndex, int totalRows, InsertOptions options)
```


在工作表中插入多行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| rowIndex | int | 行索引。 |
| totalRows | int | 要插入的行数。 |
| options | [InsertOptions](../../com.aspose.cells/insertoptions) | 插入操作的选项。 |

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
### isDefaultColumnHidden() {#isDefaultColumnHidden--}
```
public boolean isDefaultColumnHidden()
```




**Returns:**
boolean
### isDefaultRowHeightMatched() {#isDefaultRowHeightMatched--}
```
public boolean isDefaultRowHeightMatched()
```


指示行高与默认字体高度匹配。

**Returns:**
boolean
### isDefaultRowHidden() {#isDefaultRowHidden--}
```
public boolean isDefaultRowHidden()
```


指示该行是否默认隐藏。

**Returns:**
boolean
### isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns) {#isDeletingRangeEnabled-int-int-int-int-}
```
public boolean isDeletingRangeEnabled(int startRow, int startColumn, int totalRows, int totalColumns)
```


检查该范围是否可以删除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 范围的起始行索引。 |
| startColumn | int | 范围的起始列索引。 |
| totalRows | int | 范围内的行数。 |
| totalColumns | int | 范围内的列数。 |

**Returns:**
boolean -
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


获取单元格枚举器。

**Remarks**

在使用返回的 Enumerator 遍历元素时，不应修改 cells 集合（例如会导致新建 Cell/Row 或删除现有 Cell/Row 的操作）。否则 Enumerator 可能无法正确遍历所有单元格（某些元素可能被重复遍历或被跳过）。

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.iterator();
         	while (en.hasNext())
         	{
         	    Cell cell = (Cell)en.next();
         	    System.out.println(cell.getName() + ": " + cell.getValue());
         	}
```

**Returns:**
java.util.Iterator - cells 枚举器
### linkToXmlMap(String mapName, int row, int column, String path) {#linkToXmlMap-java.lang.String-int-int-java.lang.String-}
```
public void linkToXmlMap(String mapName, int row, int column, String path)
```


链接到 XML 映射。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| mapName | java.lang.String | xml 映射的名称 |
| 行 | int | 目标单元格的行 |
| 列 | int | 目标单元格的列 |
| 路径 | java.lang.String | xml 映射中 xml 元素的路径 |

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

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict) {#merge-int-int-int-int-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean mergeConflict)
```


将指定范围的单元格合并为一个单元格。

**Remarks**

通过范围左上角单元格的地址引用合并单元格。如果 mergeConflict 为 true 且合并范围与其他合并单元格冲突，则其他合并单元格将被自动移除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 此范围的第一行（零基）。 |
| firstColumn | int | 此范围的第一列（零基）。 |
| totalRows | int | 行数（从一开始计）。 |
| totalColumns | int | 列数（从一开始计）。 |
| mergeConflict | boolean | 合并冲突的合并范围。 |

### merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict) {#merge-int-int-int-int-boolean-boolean-}
```
public void merge(int firstRow, int firstColumn, int totalRows, int totalColumns, boolean checkConflict, boolean mergeConflict)
```


将指定范围的单元格合并为一个单元格。

**Remarks**

通过范围左上角单元格的地址引用合并单元格。如果 mergeConflict 为 true 且合并范围与其他合并单元格冲突，则其他合并单元格将被自动移除。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstRow | int | 此范围的第一行（零基）。 |
| firstColumn | int | 此范围的第一列（零基）。 |
| totalRows | int | 行数（从一开始计）。 |
| totalColumns | int | 列数（从一开始计）。 |
| checkConflict | boolean | 指示是否检查合并单元格是否与其他合并单元格相交 |
| mergeConflict | boolean | 合并冲突的合并范围。 |

### moveRange(CellArea sourceArea, int destRow, int destColumn) {#moveRange-com.aspose.cells.CellArea-int-int-}
```
public void moveRange(CellArea sourceArea, int destRow, int destColumn)
```


移动该范围。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| sourceArea | [CellArea](../../com.aspose.cells/cellarea) | 应移动的范围。 |
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




### removeDuplicates() {#removeDuplicates--}
```
public void removeDuplicates()
```


删除工作表中的重复行。

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

### removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets) {#removeDuplicates-int-int-int-int-boolean-int---}
```
public void removeDuplicates(int startRow, int startColumn, int endRow, int endColumn, boolean hasHeaders, int[] columnOffsets)
```


删除范围的重复数据。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| startRow | int | 起始行。 |
| startColumn | int | 起始列 |
| endRow | int | 结束行索引。 |
| endColumn | int | 结束列索引。 |
| hasHeaders | boolean | 指示该范围是否包含标题。 |
| columnOffsets | int[] | 列偏移量。 |

### removeFormulas() {#removeFormulas--}
```
public void removeFormulas()
```


删除所有公式并替换为公式的值。

### retrieveSubtotalSetting(CellArea ca) {#retrieveSubtotalSetting-com.aspose.cells.CellArea-}
```
public SubtotalSetting retrieveSubtotalSetting(CellArea ca)
```


检索范围的子计数设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 范围 |

**Returns:**
[SubtotalSetting](../../com.aspose.cells/subtotalsetting) - 
### setColumnWidth(int column, double width) {#setColumnWidth-int-double-}
```
public void setColumnWidth(int column, double width)
```


在普通视图中设置指定列的宽度。

**Remarks**

对于电子表格，列宽以普通样式字体中数字 0~9 的最大数字宽度对应的字符数来衡量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 宽度 | double | 列宽的单位为字符。列宽必须在 0 到 255 之间。 |

### setColumnWidthInch(int column, double inches) {#setColumnWidthInch-int-double-}
```
public void setColumnWidthInch(int column, double inches)
```


在普通视图中以英寸为单位设置列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 英寸 | double | 英寸数。 |

### setColumnWidthPixel(int column, int pixels) {#setColumnWidthPixel-int-int-}
```
public void setColumnWidthPixel(int column, int pixels)
```


在普通视图中以像素为单位设置列宽。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 像素 | int | 像素数。 |

### setDefaultColumnHidden(boolean value) {#setDefaultColumnHidden-boolean-}
```
public void setDefaultColumnHidden(boolean value)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDefaultRowHeightMatched(boolean value) {#setDefaultRowHeightMatched-boolean-}
```
public void setDefaultRowHeightMatched(boolean value)
```


指示行高与默认字体高度匹配。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setDefaultRowHidden(boolean value) {#setDefaultRowHidden-boolean-}
```
public void setDefaultRowHidden(boolean value)
```


指示该行是否默认隐藏。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMemorySetting(int value) {#setMemorySetting-int-}
```
public void setMemorySetting(int value)
```


设置此单元格的内存使用选项。

参见 [MemorySetting](../../com.aspose.cells/memorysetting)。

**Remarks**

某些模式的显著限制和推荐操作：

| 模式 | 备注 | 支持 |
| ------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------- |
| [MemorySetting.MEMORY\_PREFERENCE](../../com.aspose.cells/memorysetting\#MEMORY-PREFERENCE) | Cells data will be maintained in compact format to decrease the memory cost. On other hand, the compact data also may cause higher time cost, especially when updating the cells data, or accessing cells/rows randomly | v8.0.0 |
|  | [MemorySetting.FILE\_CACHE](../../com.aspose.cells/memorysetting\#FILE-CACHE) | 当在同一工作簿的任何工作表中使用此模式时，应在工作结束时调用[Workbook.dispose()](../../com.aspose.cells/workbook\#dispose--)以释放所有资源，例如临时文件。 |
 
随机访问单元格会导致性能下降，因为数据需要随机且反复读取/更新（因此文件指针会相应改变，并且需要重复的 IO 操作）。如果可能，请始终顺序访问数据（逐行）。
 
当某一行/单元格的数据被更改时，其他单元格/行的数据可能也会受到影响（例如数据被移位/移动到其他位置以为更改后的数据分配足够的空间）。因此，每一次数据的更改都需要同步其他已有对象（例如 Row 或 Cell 对象）。为了获得更好的性能，请不要同时维护多个 Row/Cell。逐个处理它们可以减少数据同步，从而略微提升性能。 | v25.7     |

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setMultiThreadReading(boolean value) {#setMultiThreadReading-boolean-}
```
public void setMultiThreadReading(boolean value)
```


设置单元格数据模型是否应支持多线程读取。此属性的默认值为 false。

**Remarks**

如果有多个线程并发读取此集合中的 Row/Cell 对象，则应将此属性设为 true，否则可能产生意外结果。支持多线程读取可能会降低访问此集合中 Row/Cell 对象的性能。请注意，某些功能无法支持多线程读取，例如格式化值（通过 [Cell.getStringValue()](../../com.aspose.cells/cell\#getStringValue--)、[Cell.getDisplayStringValue()](../../com.aspose.cells/cell\#getDisplayStringValue--) 等）。因此，即使此属性被设为 true，这些 API 在多线程读取时仍可能产生意外结果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPreserveString(boolean value) {#setPreserveString-boolean-}
```
public void setPreserveString(boolean value)
```


设置一个值，指示是否将所有工作表值保留为字符串。默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRowHeight(int row, double height) {#setRowHeight-int-double-}
```
public void setRowHeight(int row, double height)
```


设置指定行的高度。

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
| 英寸 | double | 英寸数。应在 0 到 409.5/72 之间。 |

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

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


以磅为单位设置此工作表的默认行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setStandardHeightInch(double value) {#setStandardHeightInch-double-}
```
public void setStandardHeightInch(double value)
```


以英寸为单位设置此工作表的默认行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


以像素为单位设置此工作表的默认行高。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setStandardWidth(double value) {#setStandardWidth-double-}
```
public void setStandardWidth(double value)
```


以字符为单位设置工作表的默认列宽。

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

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


设置工作表的默认样式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setViewColumnWidthPixel(int column, int pixels) {#setViewColumnWidthPixel-int-int-}
```
public void setViewColumnWidthPixel(int column, int pixels)
```


在不同视图中设置列的宽度。

**Remarks**

如果当前视图类型是 [ViewType.PAGE\_LAYOUT\_VIEW](../../com.aspose.cells/viewtype\#PAGE-LAYOUT-VIEW)，列宽与打印宽度相同。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 像素 | int | 宽度的单位为像素。 |

### showGroupDetail(boolean isVertical, int index) {#showGroupDetail-boolean-int-}
```
public void showGroupDetail(boolean isVertical, int index)
```


展开分组的行/列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| isVertical | boolean | True，展开分组的行。 |
| 索引 | int | 行/列索引 |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList) {#subtotal-com.aspose.cells.CellArea-int-int-int---}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList)
```


为范围创建小计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 范围 |
| groupBy | int | 用于分组的字段，零基整数偏移。 |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction)。小计函数。 |
| totalList | int[] | 零基字段偏移数组，指示向哪些字段添加小计。 |

### subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData) {#subtotal-com.aspose.cells.CellArea-int-int-int---boolean-boolean-boolean-}
```
public void subtotal(CellArea ca, int groupBy, int function, int[] totalList, boolean replace, boolean pageBreaks, boolean summaryBelowData)
```


为范围创建小计。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | 范围 |
| groupBy | int | 用于分组的字段，零基整数偏移。 |
| function | int | [ConsolidationFunction](../../com.aspose.cells/consolidationfunction)。小计函数。 |
| totalList | int[] | 零基字段偏移数组，指示向哪些字段添加小计。 |
| replace | boolean | 指示是否替换当前小计。 |
| pageBreaks | boolean | 指示是否在组之间添加分页符 |
| summaryBelowData | boolean | 指示是否在数据下方添加摘要。 |

### textToColumns(int row, int column, int totalRows, TxtLoadOptions options) {#textToColumns-int-int-int-com.aspose.cells.TxtLoadOptions-}
```
public int textToColumns(int row, int column, int totalRows, TxtLoadOptions options)
```


将指定列中的内容拆分为多个列..

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 列 | int | 列索引。 |
| totalRows | int | 行数。 |
| options | [TxtLoadOptions](../../com.aspose.cells/txtloadoptions) | 拆分选项。 |

**Returns:**
int - 拆分值的总列数。
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

### ungroupRows(int firstIndex, int lastIndex, boolean isAll) {#ungroupRows-int-int-boolean-}
```
public void ungroupRows(int firstIndex, int lastIndex, boolean isAll)
```


取消分组行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| firstIndex | int | 要取消分组的第一行索引。 |
| lastIndex | int | 要取消分组的最后一行索引。 |
| isAll | boolean | True，删除所有分组信息。否则，删除外部组信息。 |

### unhideColumn(int column, double width) {#unhideColumn-int-double-}
```
public void unhideColumn(int column, double width)
```


取消隐藏列

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| 宽度 | double | 列宽。 |

### unhideColumns(int column, int totalColumns, double width) {#unhideColumns-int-int-double-}
```
public void unhideColumns(int column, int totalColumns, double width)
```


取消隐藏多个列。

**Remarks**

仅将列宽应用于隐藏列。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 列 | int | 列索引。 |
| totalColumns | int | 列号 |
| 宽度 | double | 列宽。 |

### unhideRow(int row, double height) {#unhideRow-int-double-}
```
public void unhideRow(int row, double height)
```


取消隐藏行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| 高度 | double | 行高。仅当行被隐藏且给定的高度值为正时，行高才会被更改。 |

### unhideRows(int row, int totalRows, double height) {#unhideRows-int-int-double-}
```
public void unhideRows(int row, int totalRows, double height)
```


取消隐藏隐藏的行。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 行 | int | 行索引。 |
| totalRows | int | 行号。 |
| 高度 | double | 行高。仅当行被隐藏且给定的高度值为正时，行高才会被更改。 |

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

