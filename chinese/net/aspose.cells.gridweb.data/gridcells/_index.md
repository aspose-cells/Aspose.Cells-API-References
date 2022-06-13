---
title: GridCells
second_title: Aspose.Cells for .NET API 参考
description: 封装Cell对象的集合
type: docs
weight: 190
url: /zh/net/aspose.cells.gridweb.data/gridcells/
---
## GridCells class

封装Cell对象的集合。

```csharp
public class GridCells : IEnumerable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Columns](../../aspose.cells.gridweb.data/gridcells/columns) { get; } |  |
| [Count](../../aspose.cells.gridweb.data/gridcells/count) { get; } | 获取单元格数。 |
| [FirstCell](../../aspose.cells.gridweb.data/gridcells/firstcell) { get; } |  |
| [Item](../../aspose.cells.gridweb.data/gridcells/item) { get; } | 获取Cell工作表中的项目 (3 indexers) |
| [LastCell](../../aspose.cells.gridweb.data/gridcells/lastcell) { get; } |  |
| [MaxColumn](../../aspose.cells.gridweb.data/gridcells/maxcolumn) { get; } | 包含数据或样式的单元格的最大列索引。 |
| [MaxDataColumn](../../aspose.cells.gridweb.data/gridcells/maxdatacolumn) { get; } |  |
| [MaxDataRow](../../aspose.cells.gridweb.data/gridcells/maxdatarow) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/gridcells/maxrow) { get; } | 包含数据或样式的单元格的最大行索引。 |
| [MergedCells](../../aspose.cells.gridweb.data/gridcells/mergedcells) { get; } | 获取合并单元格的集合。 |
| [MinColumn](../../aspose.cells.gridweb.data/gridcells/mincolumn) { get; } |  |
| [MinDataColumn](../../aspose.cells.gridweb.data/gridcells/mindatacolumn) { get; } |  |
| [MinDataRow](../../aspose.cells.gridweb.data/gridcells/mindatarow) { get; } |  |
| [MinRow](../../aspose.cells.gridweb.data/gridcells/minrow) { get; } |  |
| [RowEnumerator](../../aspose.cells.gridweb.data/gridcells/rowenumerator) { get; } | 获取行枚举器 |
| [Rows](../../aspose.cells.gridweb.data/gridcells/rows) { get; } |  |
| [StandardHeight](../../aspose.cells.gridweb.data/gridcells/standardheight) { get; set; } | 获取或设置此工作表中的默认行高，以磅为单位。 |
| [StandardHeightPixels](../../aspose.cells.gridweb.data/gridcells/standardheightpixels) { get; set; } | 获取或设置此工作表中的默认行高，以像素为单位。 |
| [StandardWidth](../../aspose.cells.gridweb.data/gridcells/standardwidth) { get; set; } | 获取或设置工作表的默认列宽，以字符为单位。 |
| [StandardWidthInch](../../aspose.cells.gridweb.data/gridcells/standardwidthinch) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.gridweb.data/gridcells/standardwidthpixels) { get; set; } |  |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/gridcells/clear)() | 清除集合中的所有单元格。 |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents)(GridCellArea) | 清除范围的内容。 |
| [ClearContents](../../aspose.cells.gridweb.data/gridcells/clearcontents#clearcontents_1)(int, int, int, int) | 清除范围的内容。 |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats)(GridCellArea) | 清除范围的格式。 |
| [ClearFormats](../../aspose.cells.gridweb.data/gridcells/clearformats#clearformats_1)(int, int, int, int) | 清除范围的格式。 |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange)(GridCellArea) | 清除范围的内容和格式。 |
| [ClearRange](../../aspose.cells.gridweb.data/gridcells/clearrange#clearrange_1)(int, int, int, int) | 清除范围的内容和格式。 |
| [CopyColumn](../../aspose.cells.gridweb.data/gridcells/copycolumn)(GridCells, int, int) | 复制整列的数据和格式。 |
| [CopyColumns](../../aspose.cells.gridweb.data/gridcells/copycolumns)(GridCells, int, int, int) | 复制整列的数据和格式。 |
| [CopyRow](../../aspose.cells.gridweb.data/gridcells/copyrow)(GridCells, int, int) | 复制整行的数据和格式。 |
| [CopyRows](../../aspose.cells.gridweb.data/gridcells/copyrows)(GridCells, int, int, int) | 复制一些整行的数据和格式。 |
| [DeleteBlankColumns](../../aspose.cells.gridweb.data/gridcells/deleteblankcolumns)() | 删除所有不包含任何数据的空白列。 |
| [DeleteBlankRows](../../aspose.cells.gridweb.data/gridcells/deleteblankrows)() | 删除所有不包含任何数据的空白行。 |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn)(int) | 删除一列。 |
| [DeleteColumn](../../aspose.cells.gridweb.data/gridcells/deletecolumn#deletecolumn_1)(int, bool) | 删除一列。 |
| [DeleteColumns](../../aspose.cells.gridweb.data/gridcells/deletecolumns)(int, int, bool) | 删除几列。 |
| [DeleteRange](../../aspose.cells.gridweb.data/gridcells/deleterange)(int, int, int, int, GridShiftType) | 删除一系列单元格并根据 shift 选项移动单元格。 |
| [DeleteRow](../../aspose.cells.gridweb.data/gridcells/deleterow)(int) | 删除一行。 |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows)(int, int) | 删除几行。 |
| [DeleteRows](../../aspose.cells.gridweb.data/gridcells/deleterows#deleterows_1)(int, int, bool) | 删除工作表中的多行。 |
| [Export](../../aspose.cells.gridweb.data/gridcells/export)(int, int, int, int, bool, bool) | 将 WebWorksheet 的 Cells 集合中的数据导出到新的 DataTable 对象 |
| [ExportArray](../../aspose.cells.gridweb.data/gridcells/exportarray)(int, int, int, int) | 将Cells集合中的数据导出到二维数组对象。 |
| [GetCell](../../aspose.cells.gridweb.data/gridcells/getcell)(int, int) | 获取指定单元格行索引和列索引处的Cell元素或 null。 |
| [GetColumnWidth](../../aspose.cells.gridweb.data/gridcells/getcolumnwidth)(int) | 获取指定列的宽度 |
| [GetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthinch)(int) | 获取指定列的宽度，单位为英寸。 |
| [GetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getcolumnwidthpixel)(int) | 获取指定列的宽度，以像素为单位。 |
| [GetEnumerator](../../aspose.cells.gridweb.data/gridcells/getenumerator)() | 获取行枚举器 |
| [GetRow](../../aspose.cells.gridweb.data/gridcells/getrow)(int) | 获取Row元素或指定单元格行索引处。 |
| [GetRowHeight](../../aspose.cells.gridweb.data/gridcells/getrowheight)(int) | 获取指定行的高度。 |
| [GetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/getrowheightinch)(int) | 获取指定行的高度，以英寸为单位。 |
| [GetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/getrowheightpixel)(int) | 获取指定行的高度，以像素为单位。 |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/getrowoutlinelevel)(int) | 获取行的大纲级别。 |
| [GetViewColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/getviewcolumnwidthpixel)(int) | 获取不同视图类型的宽度。 |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns)(int, int) | 分组列。 |
| [GroupColumns](../../aspose.cells.gridweb.data/gridcells/groupcolumns#groupcolumns_1)(int, int, bool) | 分组列。 |
| [GroupRows](../../aspose.cells.gridweb.data/gridcells/grouprows)(int, int) | 分组行。 |
| [HideColumn](../../aspose.cells.gridweb.data/gridcells/hidecolumn)(int) | 隐藏列。 |
| [HideRow](../../aspose.cells.gridweb.data/gridcells/hiderow)(int) | 隐藏一行。 |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn)(int) | 在工作表中插入一个新列。 |
| [InsertColumn](../../aspose.cells.gridweb.data/gridcells/insertcolumn#insertcolumn_1)(int, bool) | 在工作表中插入一个新列。 |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns)(int, int) | 在工作表中插入一些列。 |
| [InsertColumns](../../aspose.cells.gridweb.data/gridcells/insertcolumns#insertcolumns_1)(int, int, bool) | 在工作表中插入一些列。 |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange)(GridCellArea, GridShiftType) | 插入一系列单元格并根据 shift 选项移动单元格。 |
| [InsertRange](../../aspose.cells.gridweb.data/gridcells/insertrange#insertrange_1)(GridCellArea, int, GridShiftType, bool) | 插入一系列单元格并根据 shift 选项移动单元格。 |
| [InsertRow](../../aspose.cells.gridweb.data/gridcells/insertrow)(int) | 在工作表中插入一个新行。 |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows)(int, int) | 在工作表中插入多行。 |
| [InsertRows](../../aspose.cells.gridweb.data/gridcells/insertrows#insertrows_1)(int, int, bool) | 在工作表中插入多行。 |
| [IsBlankColumn](../../aspose.cells.gridweb.data/gridcells/isblankcolumn)(int) | 检查给定列是否为空白（不包含任何数据）。 |
| [IsColumnHidden](../../aspose.cells.gridweb.data/gridcells/iscolumnhidden)(int) | 检查给定索引处的列是否隐藏。 |
| [IsRowHidden](../../aspose.cells.gridweb.data/gridcells/isrowhidden)(int) | 检查给定索引处的行是否隐藏。 |
| [Merge](../../aspose.cells.gridweb.data/gridcells/merge)(int, int, int, int) | 将指定范围的单元格合并为一个单元格。 |
| [MoveRange](../../aspose.cells.gridweb.data/gridcells/moverange)(GridCellArea, int, int) | 移动范围。 |
| [RemoveFormulas](../../aspose.cells.gridweb.data/gridcells/removeformulas)() | 删除所有公式并替换为公式的值。 |
| [SetBorders](../../aspose.cells.gridweb.data/gridcells/setborders)(int, int, int, int, SetBorderPosition, WebBorderStyle) | 设置单元格范围的边框。 |
| [SetColumnWidth](../../aspose.cells.gridweb.data/gridcells/setcolumnwidth)(int, double) | 设置指定列的宽度。 |
| [SetColumnWidthInch](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthinch)(int, double) | 以英寸为单位设置列宽。 |
| [SetColumnWidthPixel](../../aspose.cells.gridweb.data/gridcells/setcolumnwidthpixel)(int, int) | 以像素为单位设置列宽。 |
| [SetRowHeight](../../aspose.cells.gridweb.data/gridcells/setrowheight)(int, double) | 设置指定行的高度。 |
| [SetRowHeightInch](../../aspose.cells.gridweb.data/gridcells/setrowheightinch)(int, double) | 以英寸为单位设置行高。 |
| [SetRowHeightPixel](../../aspose.cells.gridweb.data/gridcells/setrowheightpixel)(int, int) | 以像素为单位设置行高。 |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/gridcells/setrowoutlinelevel)(int, int) | 设置行的大纲级别。 |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle_1)(string, GridTableItemStyle) | 将样式设置为指定的单元格范围。 |
| [SetStyle](../../aspose.cells.gridweb.data/gridcells/setstyle#setstyle)(int, int, int, int, GridTableItemStyle) | 将样式设置为指定的单元格范围。 |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort)(int, int, int, int, int, bool, bool, bool) | 按指定的列索引对工作表范围内的数据从上到下进行升序/降序排序。 按指定的行索引对工作表范围内的数据从左到右进行升序/降序排序。 |
| [Sort](../../aspose.cells.gridweb.data/gridcells/sort#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) |  |
| [UngroupColumns](../../aspose.cells.gridweb.data/gridcells/ungroupcolumns)(int, int) | 取消分组列。 |
| [UngroupRows](../../aspose.cells.gridweb.data/gridcells/ungrouprows)(int, int) | 取消组合行。 |
| [UnhideColumn](../../aspose.cells.gridweb.data/gridcells/unhidecolumn)(int, double) | 取消隐藏列 |
| [UnhideRow](../../aspose.cells.gridweb.data/gridcells/unhiderow)(int) | 取消隐藏一行。 |
| [UnMerge](../../aspose.cells.gridweb.data/gridcells/unmerge)(int, int, int, int) | 取消合并指定范围的合并单元格。 |
| static [CellIndexToName](../../aspose.cells.gridweb.data/gridcells/cellindextoname)(int, int) | 根据行和列索引获取单元格名称。 |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/gridcells/cellnametoindex)(string, out int, out int) | 根据名称获取单元格行和列索引 |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/gridcells/columnindextoname)(int) | 根据列索引获取列名。 |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/gridcells/columnnametoindex)(string) | 根据列名获取列索引。 |

### 也可以看看

* 命名空间 [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data)
* 部件 [Aspose.Cells.GridWeb](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridWeb.dll -->
