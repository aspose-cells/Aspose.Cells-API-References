---
title: "类 GridLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.GridLoadOptions 类。表示加载文件的选项。已过时：此类将在独立 DLL 使用 Cells 公共 API 后被废弃，您可以使用 Aspose.Cells.LodOptions。"
type: docs
url: /zh/net/aspose.cells.gridweb.data/gridloadoptions/
---
## GridLoadOptions class

表示加载文件的选项。 [Obsolete(\"此类将在独立 DLL 使用 Cells 公共 API 后被废弃，您可以使用 Aspose.Cells.LodOptions \")]

```csharp
public class GridLoadOptions : ISerializable
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GridLoadOptions](gridloadoptions/)() | 创建一个加载文件的选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | 指示在加载文件时是否自动过滤数据。 |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | 检查模板文件中的数据是否有效。 |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改与单元格相关的对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到一个 Exception。如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，例如 CSV。然而，如果您设置的值对 Excel 文件格式无效，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。 |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | 如果直接打印文件，忽略未打印的数据。 |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | 在从模板文件加载 Workbook 时，是否在内存中保留未解析的数据。默认值为 true。 |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | 指示是否仅适配高度未自定义的行。 |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | 指示在读取文件时是否解析公式。 |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | 指示在加载文件时是否解析数据透视表缓存记录。默认值为 false。 |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | 获取和设置工作簿的密码。 |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。 |

### 另请参见

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


