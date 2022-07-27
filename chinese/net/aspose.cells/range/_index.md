---
title: Range
second_title: Aspose.Cells for .NET API 参考
description: 封装表示电子表格中一系列单元格的对象
type: docs
weight: 5030
url: /zh/net/aspose.cells/range/
---
## Range class

封装表示电子表格中一系列单元格的对象。

```csharp
public class Range
```

## 特性

| 姓名 | 描述 |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | 获取范围的地址。 |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | 获取范围内的列数。 |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | 设置或获取此范围的列宽 |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | 返回代表当前区域的 Range 对象。 当前区域是由空白行和空白列的任意组合限定的范围。 |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | 获取一个 Range 对象，该对象表示包含指定范围的整列（或多列）。 |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | 获取一个 Range 对象，该对象表示包含指定范围的整行（或多行）。 |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | 获取范围第一列的索引。 |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | 获取范围第一行的索引。 |
| [Height](../../aspose.cells/range/height) { get; } | 获取范围的宽度（以磅为单位）。 |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | 获取范围内的所有超链接。 |
| [Item](../../aspose.cells/range/item) { get; } | 获取[`Cell`](../cell)此范围内的对象。 |
| [Left](../../aspose.cells/range/left) { get; } | 获取从 A 列左边缘到范围左边缘的距离（以磅为单位）。 |
| [Name](../../aspose.cells/range/name) { get; set; } | 获取或设置范围的名称。 |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | 获取范围的引用。 |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | 获取范围内的行数。 |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | 设置或获取此范围内的行高 |
| [Top](../../aspose.cells/range/top) { get; } | 获取从第 1 行的上边缘到范围的上边缘的距离（以磅为单位）。 |
| [Value](../../aspose.cells/range/value) { get; set; } | 获取和设置范围的值。 |
| [Width](../../aspose.cells/range/width) { get; } | 获取范围的宽度（以磅为单位）。 |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | 获取[`Worksheet`](./worksheet)包含此范围的对象。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | 对整个范围应用格式。 |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | 自动填充目标范围。 |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | 自动填充目标范围。 |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | 从源范围复制数据（包括公式）、格式、绘图对象等。 |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | 使用粘贴特殊选项复制范围。 |
| [CopyData](../../aspose.cells/range/copydata)(Range) | 从源区域复制单元格数据（包括公式）。 |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | 从源范围复制样式设置。 |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | 从源范围复制单元格值。 |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | 将此范围内的数据导出到DataTable对象. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | 将此范围内的数据导出到DataTable对象. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | 将此范围内的数据导出到DataTable对象. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | 获取[`Cell`](../cell)此范围内的对象或空值。 |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | 获取此 Range 中单元格的枚举器。 |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | 获取[`Range`](../range)范围偏移量. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | 返回一个[`Range`](../range)表示两个范围的矩形交集的对象。 |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | 表示范围是否相交。 |
| [Merge](../../aspose.cells/range/merge)() | 将一系列单元格组合成一个单元格。 |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | 将当前范围移动到目标范围。 |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | 将一个值放入范围内，如果合适，该值将转换为其他数据类型并重置单元格的数字格式。 |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | 设置范围内的边界。 |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | 围绕一系列单元格设置轮廓边框。 |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | 围绕具有相同边框样式和颜色的一系列单元格设置轮廓边框。 |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | 在一系列单元格周围设置线条边框。 |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | 设置范围的样式。 |
| override [ToString](../../aspose.cells/range/tostring)() | 返回一个代表当前 Range 对象的字符串。 |
| [Union](../../aspose.cells/range/union)(Range) | 返回两个范围的并集。 |
| [UnMerge](../../aspose.cells/range/unmerge)() | 取消合并此范围内的合并单元格。 |

### 例子

```csharp

[C#]

//实例化一个工作簿对象
Workbook workbook = new Workbook();
// 获取第一个工作表单元格。
Cells cells = workbook.Worksheets[0].Cells;
// 创建一个范围 (A1:D3)。
Range range = cells.CreateRange("A1", "D3");
// 将值设置为范围。
range.Value = "Hello";
//保存Excel文件
workbook.Save("book1.xlsm");

 [Visual Basic]

'实例化工作簿对象
Dim workbook As Workbook = New Workbook()
'获取第一个工作表单元格。
Dim cells as Cells = workbook.Worksheets[0].Cells
'创建一个范围 (A1:D3)。
Dim range as Range = cells.CreateRange("A1", "D3")
'将值设置为范围。
range.Value = "Hello"
'保存 Excel 文件
workbook.Save("book1.xlsm")
```

### 也可以看看

* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
