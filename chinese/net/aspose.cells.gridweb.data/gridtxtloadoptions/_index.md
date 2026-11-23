---
title: "类 GridTxtLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridWeb.Data.GridTxtLoadOptions 类。表示加载文本文件的选项"
type: docs
url: /zh/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

表示加载文本文件的选项。

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | 创建加载文本文件的选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | 指示在加载文件时是否自动过滤数据。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | 检查模板文件中的数据是否有效。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常。如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | 获取或设置一个值，指示文本文件中的字符串是否转换为日期数据。 |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | 获取或设置一个值，指示文本文件中的字符串是否转换为数值数据。 |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | 获取并设置默认编码。仅适用于 csv 文件。 |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | 当数据的行或列超出限制时，是否将数据扩展到下一个工作表。如果此属性为 true，超出部分的数据将扩展到当前工作表之后的下一个工作表（如果当前工作表是最后一个，则在当前工作簿中追加新工作表）。如果此属性为 false，超出限制的数据将被忽略。默认值为 false； |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | 指示文本是否为公式（如果以 "=" 开头）。 |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | 是否为单元格值设置文本限定符。默认值为 true。 |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | 在直接打印文件时忽略未打印的数据（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | True 表示文件包含多种编码。 |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | 指示是否在字符串长度为 15 时不进行解析。 |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | 在从模板文件加载工作簿时，是否在内存中保留未解析的数据。默认值为 true。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | 指示是否仅适用于高度未自定义的行。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | 指示在读取文件时是否解析公式。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | 指示在加载文件时是否解析透视表缓存记录。默认值为 false。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | 获取和设置工作簿的密码。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。（继承自 [`GridLoadOptions`](../gridloadoptions/)。） |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | 获取和设置文本文件的字符分隔符。 |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | 获取和设置字符串值作为分隔符。 |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | 指定单元格值的文本限定符。默认限定符为 '\\"'。 |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | 是否应将连续的分隔符视为一个。 |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | 指示是否应将前导单引号视为单元格值的一部分。默认值为 true。如果为 false，前导单引号将从相应单元格的值中移除，并且 [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) 将被设置为 true。 |

### 另请参见

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


