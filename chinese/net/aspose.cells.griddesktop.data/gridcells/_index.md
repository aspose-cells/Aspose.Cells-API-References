---
title: GridCells
second_title: Aspose.Cells for .NET API 参考
description: 封装了一个集合Cell对象.
type: docs
weight: 410
url: /zh/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

封装了一个集合Cell对象.

```csharp
public class GridCells : IEnumerable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count) { get; } | 获取单元格数。 |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item) { get; } | 获取Cell工作表中的项目 (3 indexers) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn) { get; } | 包含数据或样式的单元格的最大列索引。 |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow) { get; } | 包含数据或样式的单元格的最大行索引。 |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells) { get; } | 获取合并单元格的集合。 |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator) { get; } | 获取行 enumerator |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows) { get; } | 获取集合[`GridRow`](../gridrow)表示此工作表中各个行的对象。 |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight) { get; set; } | 获取或设置此工作表的默认行高，以点为单位。 |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels) { get; set; } | 获取或设置此工作表中的默认行高，以像素为单位。 |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth) { get; set; } | 获取或设置工作表的默认列宽，以字符为单位。 |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell)(int, int) | 获取Cell指定单元格行索引和列索引处的元素或空值。 |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear)() | 清除集合中的所有单元格。 |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents)(GridCellArea) | 清除范围的内容。 |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | 清除范围的内容。 |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats)(GridCellArea) | 清除范围的格式。 |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | 清除范围的格式。 |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange)(GridCellArea) | 清除范围的内容和格式。 |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | 清除范围的内容和格式。 |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn)(GridCells, int, int) | 复制整列的数据和格式。 |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns)(GridCells, int, int, int) | 复制整列的数据和格式。 |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow)(GridCells, int, int) | 复制整行的数据和格式。 |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows)(GridCells, int, int, int) | 复制某些整行的数据和格式。 |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns)() | 删除所有不包含任何数据的空白列。 |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows)() | 删除所有不包含任何数据的空白行。 |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn)(int) | 删除一列。 |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | 删除一列。 |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns)(int, int, bool) | 删除几列。 |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow)(int) | 删除一行。 |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows)(int, int) | 删除几行。 |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows#deleterows_1)(int, int, bool) | 删除工作表中的多行。 |
| [GetCell](../../aspose.cells.griddesktop.data/gridcells/getcell)(int, int) | 获取Cell指定单元格行索引和列索引处的元素或空值。 |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle)(int, int) | 获取给定单元格的样式。 |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn)(int) | 获取[`GridColumn`](../gridcolumn)元素或指定单元格列索引处。 |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth)(int) | 获取指定列的宽度 |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch)(int) | 获取指定列的宽度，以英寸为单位。 |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel)(int) | 获取指定列的宽度，以像素为单位。 |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator)() | 获取行 enumerator |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow)(int) | 获取[`GridRow`](../gridrow)元素或在指定的单元格行索引处。 |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight)(int) | 获取指定行的高度。 |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch)(int) | 以英寸为单位获取指定行的高度。 |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel)(int) | 以像素为单位获取指定行的高度。 |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel)(int) | 获取不同视图类型的宽度。 |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns)(int, int) | 对列进行分组。 |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | 对列进行分组。 |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows)(int, int) | 对行进行分组。 |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn)(int) | 隐藏一列。 |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow)(int) | 隐藏一行。 |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn)(int) | 在工作表中插入一个新列。 |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | 在工作表中插入一个新列。 |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns)(int, int) | 在工作表中插入一些列。 |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | 在工作表中插入一些列。 |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow)(int) | 在工作表中插入一个新行。 |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows)(int, int) | 在工作表中插入多行。 |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows#insertrows_1)(int, int, bool) | 在工作表中插入多行。 |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn)(int) | 检查给定列是否为空白（不包含任何数据）。 |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden)(int) | 检查给定索引处的列是否隐藏。 |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden)(int) | 检查给定索引处的行是否隐藏。 |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge)(int, int, int, int) | 将指定范围的单元格合并为一个单元格。 |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas)() | 删除所有公式并替换为公式的值。 |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth)(int, double) | 设置指定列的宽度。 |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch)(int, double) | 以英寸为单位设置列宽。 |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel)(int, int) | 以像素为单位设置列宽。 |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight)(int, double) | 设置指定行的高度。 |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch)(int, double) | 以英寸为单位设置行高。 |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel)(int, int) | 以像素为单位设置行高。 |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle)(CellRange, Style) | 将样式设置为指定范围的单元格。 |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_2)(string, Style) | 将样式设置为指定范围的单元格。 |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle#setstyle_1)(int, int, int, int, Style) | 将样式设置为指定范围的单元格。 |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | 按指定列索引对工作表范围内的数据从上到下进行升序/降序排序。 按指定行索引对工作表范围内的数据从左到右升序/降序排序。 |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns)(int, int) | 取消组合列。 |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows)(int, int) | 取消组合行。 |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn)(int, double) | 取消隐藏列 |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow)(int) | 取消隐藏一行。 |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge)(int, int, int, int) | 取消合并指定范围的合并单元格。 |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname)(int, int) | 根据行列索引获取单元格名称。 |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex)(string, out int, out int) | 根据名称获取单元格行列索引 |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname)(int) | 根据列索引获取列名。 |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex)(string) | 根据列名获取列索引。 |

### 也可以看看

* 命名空间 [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data)
* 部件 [Aspose.Cells.GridDesktop](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridDesktop.dll -->
