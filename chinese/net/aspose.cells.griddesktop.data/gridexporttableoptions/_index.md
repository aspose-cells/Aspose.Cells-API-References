---
title: "类 GridExportTableOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridDesktop.Data.GridExportTableOptions 类。表示所有导出表格选项"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridexporttableoptions/
---
## GridExportTableOptions class

表示所有导出表格选项。

```csharp
public class GridExportTableOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GridExportTableOptions](gridexporttableoptions/)() | GridExportTableOptions 的构造函数 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [CheckMixedValueType](../../aspose.cells.griddesktop.data/gridexporttableoptions/checkmixedvaluetype/) { get; set; } | False，Aspose.Cells 将基于第一行的值类型设置 DataColumn 的类型以提升性能。True，Aspose.Cells 将在设置 DataColumn 类型之前检查列中的值类型是否混合。如果值类型混合，DataColumn 的类型将为 string。 |
| [DataTable](../../aspose.cells.griddesktop.data/gridexporttableoptions/datatable/) { get; set; } | 获取并设置已分配列数据类型的 DataTable。 |
| [ExportAsHtmlString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportashtmlstring/) { get; set; } | 将单元格的 html 字符串值导出到 DataTable。 |
| [ExportAsString](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportasstring/) { get; set; } | 将单元格的字符串值导出到 DataTable。 |
| [ExportColumnName](../../aspose.cells.griddesktop.data/gridexporttableoptions/exportcolumnname/) { get; set; } | 指示是否将第一行的数据导出为 DataTable 的列名。默认值为 false。 |
| [FormatStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/formatstrategy/) { get; set; } | 获取并设置导出值为字符串时的格式策略。 |
| [Indexes](../../aspose.cells.griddesktop.data/gridexporttableoptions/indexes/) { get; set; } | 应导出的列/行的索引。 |
| [IsVertical](../../aspose.cells.griddesktop.data/gridexporttableoptions/isvertical/) { get; set; } | 如果 Workbook 文件中的行对应 DataTable 中的行，则为 True；如果 Workbook 文件中的列对应 DataTable 中的行，则为 False。 |
| [PlotVisibleCells](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecells/) { get; set; } | 仅导出可见单元格。 |
| [PlotVisibleColumns](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblecolumns/) { get; set; } | 仅导出可见列。 |
| [PlotVisibleRows](../../aspose.cells.griddesktop.data/gridexporttableoptions/plotvisiblerows/) { get; set; } | 仅导出可见行。 |
| [RenameStrategy](../../aspose.cells.griddesktop.data/gridexporttableoptions/renamestrategy/) { get; set; } | 列重复名称的策略。 |
| [SkipErrorValue](../../aspose.cells.griddesktop.data/gridexporttableoptions/skiperrorvalue/) { get; set; } | 指示是否跳过列的无效值。例如，如果列类型是 decimal，值大于 decimal.MaxValue 并且此属性为 true，则我们将不再抛出异常。默认值为 false。 |

### 另请参见

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


