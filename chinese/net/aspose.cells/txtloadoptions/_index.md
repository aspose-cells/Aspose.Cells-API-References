---
title: TxtLoadOptions
second_title: Aspose.Cells for .NET API 参考
description: 表示加载文本文件的选项
type: docs
weight: 6110
url: /zh/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

表示加载文本文件的选项。

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [TxtLoadOptions](txtloadoptions#constructor)() | 创建加载文本文件的选项。 |
| [TxtLoadOptions](txtloadoptions#constructor_1)(LoadFormat) | 创建加载文本文件的选项。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | 表示加载文件时是否自动过滤数据。 |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | 获取和设置自动拟合选项 |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | 检查模板文件中的数据是否有效 |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | 当用户修改单元格相关对象时是否检查excel文件的限制。 例如，excel不允许输入超过32K的字符串值。 当你输入一个超过32K的值时，例如通过Cell.PutValue(string)，如果这样属性为真，您将得到一个异常。 如果此属性为假，我们将接受您输入的字符串值作为单元格的值，以便稍后 您可以为其他文件格式输出完整的字符串值，例如 CSV. 但是，如果您设置的此类值对 excel 文件格式无效， 您以后不应将工作簿另存为 excel 文件格式。否则生成的excel文件可能会出现意外错误。 |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | 获取或设置一个值，该值指示文本文件中的字符串是否转换为日期数据。 |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | 获取或设置一个值，该值指示文本文件中的字符串是否转换为数值数据。 |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | 获取或设置文件加载时的系统文化信息。 |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | 获取用于初始化工作簿样式的默认样式设置 |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | 获取和设置默认编码。仅适用于 csv 文件。 |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet) { get; set; } | 当数据的行或列超过限制时，是否将数据扩展到下一张。 如果该属性为true，额外的数据将被扩展到当前一张之后的下一张（如果当前一张是最后一张， 将追加新的表格到当前工作簿）。 如果此属性为false，超出限制的数据将被忽略。 默认为false； |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | 获取和设置单独的字体配置。 仅适用于[`Workbook`](../workbook)它使用这个[`LoadOptions`](../loadoptions)加载。&gt; |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula) { get; set; } | 如果文本以“=”开头，则表示文本是否为公式。 |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier) { get; set; } | 单元格值是否有文本限定符。默认为真。 |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | 直接打印文件忽略不打印的数据 |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | 获取和设置中断监视器。 |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded) { get; set; } | 真表示文件包含几种编码。 |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | 表示如果长度为15，是否不解析字符串值。 |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | 从模板文件加载工作簿时，是否将未解析的数据保留在内存中。默认为真。 |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | 根据保存文件的 CountryCode 获取或设置 Workbook 版本的用户界面语言。 |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | 读取模板文件时处理单元格数据的数据处理程序。 |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | 表示如何加载数据的过滤器。 |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | 获取加载格式。 |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | 表示将字符串值转换为数字或日期时间时为解析值应用样式的策略。 |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | 获取或设置内存使用选项。 |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | 读取文件时是否解析公式 |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | 表示加载文件时是否解析pivot缓存记录。 默认值为false。 |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | 获取和设置工作簿的密码。 |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers) { get; set; } | 获取和设置用于加载文本文件的首选值解析器。 |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | 根据加载文件时的 CountryCode 获取或设置系统区域设置。 |
| [Separator](../../aspose.cells/txtloadoptions/separator) { get; set; } | 获取和设置文本文件的字符分隔符。 |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring) { get; set; } | 获取并设置一个字符串值作为分隔符。 |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier) { get; set; } | 指定单元格值的文本限定符。默认限定符是 '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone) { get; set; } | 是否应将连续分隔符视为一个。 |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue) { get; set; } | 指示是否应将前导单引号作为一个单元格值的一部分。 默认为真。如果为 false，则将从相应单元格的 value 中删除前导单引号和[`QuotePrefix`](../style/quoteprefix)将为单元格设置为 true。 |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | 获取或设置警告回调。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | 从默认打印机设置中设置默认打印纸尺寸。 |

### 也可以看看

* class [AbstractTextLoadOptions](../abstracttextloadoptions)
* 命名空间 [Aspose.Cells](../../aspose.cells)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
