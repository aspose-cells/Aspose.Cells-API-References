---
title: Cells
second_title: Aspose.Cells for .NET API 参考
description: 封装单元格相关对象的集合例如Cell./cellRow...等
type: docs
weight: 300
url: /zh/net/aspose.cells/cells/
---
## Cells class

封装单元格相关对象的集合，例如[`Cell`](../cell),Row，...等。

```csharp
public class Cells : IDisposable, IEnumerable
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | 获取代表此工作表中各个列的[`Column`](../column)对象的集合。 |
| [Count](../../aspose.cells/cells/count) { get; } | 获取实例化的 Cell 对象的总数。 |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | 获取实例化的 Cell 对象的总数。 |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | 获取此工作表中的第一个单元格。 |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | 表示行高和默认字体高度匹配 |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | 指示该行是否默认隐藏。 |
| [Item](../../aspose.cells/cells/item) { get; } | 获取指定单元格行索引和列索引处的[`Cell`](../cell)元素。 (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | 获取此工作表中的最后一个单元格。 |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | 已在集合中实例化的那些单元格的最小列索引（不包括列 其中样式是为整个列定义的，但没有在其中实例化单元格）。 |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | 包含数据的单元格的最大列索引。 |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | 包含数据的单元格的最大行索引。 |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | 获取包括数据、合并单元格和形状的最大范围。 |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | 包含数据或样式的单元格的最大行索引。 |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | 获取或设置此单元格的内存使用选项。 |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | 获取合并单元格的集合。 |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | 已在集合中实例化的那些单元格的最小列索引（不包括列 其中样式是为整个列定义的，但没有在其中实例化单元格）。 |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | 包含数据的单元格的最小列索引。 |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | 包含数据的单元格的最小行索引。 |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | 包含数据或样式的单元格的最小行索引。 |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | 获取或设置单元格数据模型是否应支持多线程读取。 此属性的默认值为 false。 |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | 获取ods的字段列表。 |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | 获取或设置一个值，该值指示是否所有工作表值都保留为字符串。 默认为假。 |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | 获取运行时创建的[`Range`](../range)对象的集合。 |
| [Rows](../../aspose.cells/cells/rows) { get; } | 获取[`Row`](../row)对象的集合，这些对象表示此工作表中的各个行。 |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | 获取或设置此工作表中的默认行高，以磅为单位。 |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | 获取或设置此工作表中的默认行高，以英寸为单位。 |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | 获取或设置此工作表中的默认行高，以像素为单位。 |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | 获取或设置工作表中的默认列宽，以字符为单位。 |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | 获取或设置工作表中的默认列宽，单位为英寸。 |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | 获取或设置工作表中的默认列宽，以像素为单位。 |
| [Style](../../aspose.cells/cells/style) { get; set; } | 获取和设置默认样式。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | 向单元格添加范围对象引用 |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | 对整列应用格式。 |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | 对整行应用格式。 |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | 为整个工作表应用格式。 |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | 在指定的单元格行索引和列索引处获取[`Cell`](../cell)元素或 null。 |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | 在指定列索引处获取[`Column`](../column)元素或 null。 |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | 获取[`Row`](../row)元素或指定单元格行索引处。 |
| [Clear](../../aspose.cells/cells/clear)() | 清除所有单元格和行对象。 |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | 清除范围的内容。 |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | 清除范围的内容。 |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | 清除范围的格式。 |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | 清除范围的格式。 |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | 清除所有合并范围。 |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | 清除范围的内容和格式。 |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | 清除范围的内容和格式。 |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | 如果可能，将单元格中的字符串数据转换为数值。 |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | 复制整列的数据和格式。 |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | 复制整列的数据和格式。 |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | 复制整列的数据和格式。 |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | 复制整列的数据和格式。 |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | 复制整行的数据和格式。 |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | 复制某些整行的数据和格式。 |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | 复制某些整行的数据和格式。 |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | 复制某些整行的数据和格式。 |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | 从范围的地址创建[`Range`](../range)对象。 |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | 从一系列单元格中创建[`Range`](../range)对象。 |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | 从单元格行或单元格列创建[`Range`](../range)对象。 |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | 从一系列单元格中创建[`Range`](../range)对象。 |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | 删除所有不包含任何数据的空白列。 |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | 删除所有不包含任何数据的空白列。 |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | 删除所有不包含任何数据的空白行。 |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | 删除所有不包含任何数据的空白行。 |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | 删除一列。 |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | 删除一列。 |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | 删除几列。 |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | 删除一系列单元格并根据 shift 选项移动单元格。 |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | 删除一行。 |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | 删除几行。 |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | 删除工作表中的多行。 |
| [Dispose](../../aspose.cells/cells/dispose)() | 执行与释放、释放或 重置非托管资源相关的应用程序定义任务。 |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | 获取此列中的最后一个单元格。 |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | 获取此范围内具有最大列索引的最后一个单元格。 |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | 获取该行的最后一个单元格。 |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | 获取此范围内具有最大行索引的最后一个单元格。 |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | 将[`Cells`](../cells)集合中的数据导出到二维数组对象。 |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | 将[`Cells`](../cells)集合中的数据导出到DataTable目的。 |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | 将[`Cells`](../cells)集合中的数据导出到DataTable目的。 |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | 将[`Cells`](../cells)集合中的数据导出到DataTable目的。 |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | 将[`Cells`](../cells)集合中的数据导出到DataTable目的。 |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | 将[`Cells`](../cells)集合中的数据导出到DataTable目的。 |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | 将[`Cells`](../cells)集合中的单元格值类型导出到二维数组对象。 |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | 查找包含输入对象的单元格。 |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | 查找包含输入对象的单元格。 |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | 在指定的单元格行索引和列索引处获取[`Cell`](../cell)元素或 null。 |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | 获取给定单元格的样式。 |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | 获取普通视图中指定列的宽度 |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | 获取普通视图中指定列的宽度，单位为英寸。 |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | 获取普通视图中指定列的宽度，以像素为单位。 |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | 获取引用特定单元格的所有单元格。 |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | 获取单元格枚举器。 |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | 获取列的大纲级别（从零开始）。 |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | 获取行的大纲级别（从零开始）。 |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | 获取包含指定列数据的单元格的最后一行索引。 |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | 获取最大分组列大纲级别（从零开始）。 |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | 获取最大分组行大纲级别（从零开始）。 |
| [GetRow](../../aspose.cells/cells/getrow)(int) | 获取指定单元格行索引处的[`Row`](../row)元素。 |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | 获取行枚举器。 |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | 获取指定行的高度。 |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | 获取指定行的高度，以英寸为单位。 |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | 获取指定行的高度，以像素为单位。 |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | 如果行隐藏，则以点为单位获取原始行的高度 |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | 获取不同视图类型的宽度。 |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | 获取指定行的高度。 |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | 获取指定行的高度，以英寸为单位。 |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | 分组列。 |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | 分组列。 |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | 分组行。 |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | 分组行。 |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | 隐藏列。 |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | 隐藏多列。 |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | 折叠分组的行/列。 |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | 隐藏一行。 |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | 隐藏多行。 |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | 将双精度数组导入工作表。 |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | 将整数数组导入工作表。 |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | 将字符串数组导入工作表。 |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | 将数据数组列表导入工作表。 |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | 将 CSV 文件导入单元格。 |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | 将 CSV 文件导入单元格。 |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | 将 CSV 文件导入单元格。 |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | 将 CSV 文件导入单元格。 |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | 导入自定义对象。 |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | 导入自定义对象。 |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | 从IDataReader对象导入数据。 |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | 从自定义数据表中导入数据。 |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | 从数据视图导入数据。 |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | 从自定义数据表中导入数据。 |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | 从IDataReader对象导入数据。 |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | 将DataGrid导入工作表。 |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | 将DataGrid导入工作表。 |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | 将DataGrid导入工作表。 |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | 将DataGrid导入工作表。此方法不会尝试将文本转换为数值。 |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | 将 DataRow 导入 Excel 文件。 |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | 将DataView导入工作表。 |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | 将公式数组导入工作表。 |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | 将网格视图导入此单元格。 |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | 将数据数组导入工作表。 |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | 将数据数组导入工作表。 |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | 在工作表中插入一个新列。 |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | 在工作表中插入一个新列。 |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | 在工作表中插入一些列。 |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | 在工作表中插入一些列。 |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | 插入剪切范围。 |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | 插入一系列单元格并根据 shift 选项移动单元格。 |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | 插入一系列单元格并根据 shift 选项移动单元格。 |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | 插入一系列单元格并根据 shift 选项移动单元格。 |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | 在工作表中插入一个新行。 |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | 在工作表中插入多行。 |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | 在工作表中插入多行。 |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | 在工作表中插入多行。 |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | 检查给定列是否为空白（不包含任何数据）。 |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | 检查给定索引处的列是否隐藏。 |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | 检查范围是否可以删除。 |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | 检查给定索引处的行是否隐藏。 |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | 链接到 xml 地图。 |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | 将指定范围的单元格合并为一个单元格。 |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | 将指定范围的单元格合并为一个单元格。 |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | 将指定范围的单元格合并为一个单元格。 |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | 移动范围。 |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | 删除工作表中的重复行。 |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | 删除范围内的重复值。 |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | 删除范围内的重复数据。 |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | 删除所有公式并替换为公式的值。 |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | 检索范围的小计设置。 |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | 设置普通视图中指定列的宽度。 |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | 在普通视图中以英寸为单位设置列宽。 |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | 在普通视图中以像素为单位设置列宽。 |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | 设置指定行的高度。 |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | 以英寸为单位设置行高。 |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | 以像素为单位设置行高。 |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | 设置不同视图中列的宽度。 |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | 展开分组的行/列。 |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | 为范围创建小计。 |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | 为范围创建小计。 |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | 将列中的文本拆分为列。 |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | 取消分组列。 |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | 取消组合行。 |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | 取消组合行。 |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | 取消隐藏列 |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | 取消隐藏多列。 |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | 取消隐藏一行。 |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | 取消隐藏隐藏的行。 |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | 取消合并指定范围的合并单元格。 |

### 例子

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

//设置默认行高
cells.StandardHeight = 20;
 //设置行高
cells.SetRowHeight(2, 20.5);

 //设置默认列宽
cells.StandardWidth = 15;
 //设置列宽
cells.SetColumnWidth(3, 12.57);

 //合并单元格
cells.Merge(5, 4, 2, 2);

 //将值放入cells
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

 //导出数据
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

//设置默认行高
cells.StandardHeight = 20
//设置行高
cells.SetRowHeight(2, 20.5)

//设置默认列宽
cells.StandardWidth = 15
//设置列宽
cells.SetColumnWidth(3, 12.57)

//合并 cells
cells.Merge(5, 4, 2, 2)

//导出数据
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
