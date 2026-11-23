---
title: "类 WebCells"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.WebCells 类。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | 获取单元格的数量。 |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | 获取指定单元格行索引和列索引处的 Cell 元素。（两个索引器） |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | 获取合并单元格的集合。 |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | 包含数据或样式的单元格的最小列号。 |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | 包含数据或样式的单元格的最小行号。 |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | 获取或设置此工作表中默认的行高，单位为点。 |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | 获取或设置工作表中默认的列宽，单位为字符。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | 清除范围的内容。 |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | 删除列。 |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | 删除行。 |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | 删除多行。当进行批量删除行时，此方法比 DeleteRow 快得多。 |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | 将 WebWorksheet 中 Cells 集合的数据导出到新的 DataTable 对象。 |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | 将 Cells 集合中的数据导出为二维数组对象。 |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | 获取列标题。如果标题未设置，则返回空字符串。 |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | 获取列是否为只读。这是 GridWeb 的扩展方法，实际 Excel 文件中不会保留或生效。 |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | 获取指定列的宽度。 |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | 获取单元格枚举器。 |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | 获取行标题。如果标题未设置，则返回空字符串。 |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | 获取指定行的高度。 |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | 获取指定行的隐藏状态。 |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | 获取行的轮廓级别。 |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | 获取行是否为只读。这是 GridWeb 的扩展方法，实际 Excel 文件中不会保留或生效。 |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | 在工作表中插入新列。 |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | 在工作表中插入新行。 |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | 在工作表中插入多行。 |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | 为单元格范围设置边框。 |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | 设置列的标题。请注意，这是扩展属性，不能保存在 Excel 文件中。 |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | 将列设为只读，使用户无法在客户端删除它。这是 GridWeb 的扩展方法，实际 Excel 文件中不会保留或生效。 |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | 设置指定列的宽度。接受的宽度类型为 Point、Pixel 或 Inch。 |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | 设置行的标题。 |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | 设置指定行的高度。接受的宽度类型为 Point、Pixel 或 Inch。 |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | 设置指定行的隐藏状态。 |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | 设置行的轮廓级别。 |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | 设置行的轮廓级别。 |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | 将行设为只读，使用户无法在客户端删除它。这是 GridWeb 的扩展方法，实际 Excel 文件中不会保留或生效。 |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | 为指定的单元格范围设置样式。 |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | 为指定的单元格范围设置样式。 |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | 在 WebWorksheet 的范围内按指定列索引将数据从上到下升序排序。 |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | 在 WebWorksheet 的范围内按列索引数组指定的字段将数据从上到下升序排序。 |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | 在 WebWorksheet 的范围内按指定列索引将数据从上到下升序排序。 |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | 按由索引数组指定的某些字段，对 WebWorksheet 中的一个范围内的数据进行升序排序。 |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | 取消合并指定范围的合并单元格。 |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | 根据其行列索引获取单元格名称。 |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | 根据名称获取单元格的行列索引。 |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | 根据列索引获取列名称。 |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | 根据列名称获取列索引。 |

### 备注

注意：此类已过时。请改用 GridCells。该类将在自 2014 年 8 月起的 6 个月后移除。Aspose 对您可能遇到的任何不便表示歉意。

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


