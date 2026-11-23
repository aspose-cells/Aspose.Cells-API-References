---
title: "类 MarkdownLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.MarkdownLoadOptions 类。表示加载 markdown 文档的选项"
type: docs
url: /zh/net/aspose.cells/markdownloadoptions/
---
## MarkdownLoadOptions class

表示加载 markdown 文档的选项。

```csharp
public class MarkdownLoadOptions : AbstractTextLoadOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [MarkdownLoadOptions](markdownloadoptions/)() | 默认构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | 指示在加载文件时是否自动过滤数据。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | 获取和设置自动适配选项（继承自 [`LoadOptions`](../loadoptions/)。） |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | 检查模板文件中的数据是否有效。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常。如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | 获取或设置一个值，指示文本文件中的字符串是否转换为日期数据。默认值为 true。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | 获取或设置一个值，指示文本文件中的字符串是否转换为数值数据。默认值为 true。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | 获取或设置用于将要加载的工作簿的区域设置。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | 获取工作簿初始化样式的默认样式设置（继承自 [`LoadOptions`](../loadoptions/)。） |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | 获取或设置默认编码。仅适用于 csv 文件。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | 获取或设置各个字体配置。仅适用于使用此 [`LoadOptions`](../loadoptions/) 加载的 [`Workbook`](../workbook/)。 （继承自 [`LoadOptions`](../loadoptions/)。） |
| [HasFormula](../../aspose.cells/markdownloadoptions/hasformula/) { get; set; } | 指示文本是否为公式（如果以 "=" 开头）。 |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | 如果直接打印文件，则忽略未打印的数据。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | 指示是否忽略无用的形状。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | 获取或设置中断监视器。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | 指示如果字符串长度为 15，则不解析该字符串值。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | 指示从模板文件加载工作簿时是否在内存中保留未解析的数据。默认值为 true。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | 获取或设置基于保存文件的 CountryCode 的工作簿版本的用户界面语言。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | 读取模板文件时用于处理单元格数据的数据处理程序。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | 用于指示如何加载数据的过滤器。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | 获取加载格式。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | 指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | 获取或设置已加载工作簿的内存模式。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | 指示读取文件时是否解析公式。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | 指示加载文件时是否解析数据透视表缓存记录。默认值为 false。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | 获取或设置工作簿的密码。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | 获取或设置用于将要加载的工作簿的区域设置。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) 设置默认的标准字体名称（继承自 [`LoadOptions`](../loadoptions/)。） |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) 设置默认的标准字体大小。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | 获取或设置警告回调。（继承自 [`LoadOptions`](../loadoptions/)。） |

## 方法

| 名称 | 描述 |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | 根据默认打印机的设置设置默认打印纸张大小。（继承自 [`LoadOptions`](../loadoptions/)。） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsClassMarkdownLoadOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // 创建 MarkdownLoadOptions 的实例
                MarkdownLoadOptions options = new MarkdownLoadOptions();

                // 设置 HasFormula 属性
                options.HasFormula = true;

                // 显示属性值
                Console.WriteLine($"HasFormula property is set to: {options.HasFormula}");

                // 创建工作簿并使用选项加载 markdown 文件
                Workbook workbook = new Workbook("sample.md", options);

                // 将工作簿保存为 Excel 格式
                workbook.Save("output.xlsx");

                Console.WriteLine("Markdown file loaded and converted to Excel successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### 另请参见

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


