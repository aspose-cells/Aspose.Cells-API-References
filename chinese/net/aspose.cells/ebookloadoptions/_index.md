---
title: "类 EbookLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.EbookLoadOptions 类。表示导入电子书文件时的选项"
type: docs
url: /zh/net/aspose.cells/ebookloadoptions/
---
## EbookLoadOptions class

表示导入电子书文件时的选项。

```csharp
public class EbookLoadOptions : HtmlLoadOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [EbookLoadOptions](ebookloadoptions/#constructor)() | 创建用于加载电子书文件的选项。 |
| [EbookLoadOptions](ebookloadoptions/#constructor_1)(LoadFormat) | 创建加载电子书文件的选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**已废弃。**) 将保存附件文件的目录。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | 指示在加载文件时是否自动过滤数据。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | 指示是否自动调整列和行的宽高。默认值为 false。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | 获取和设置自动适配选项（继承自 [`LoadOptions`](../loadoptions/)。） |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | 检查模板文件中的数据是否有效。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常。如果此属性为 false，我们将接受您输入的字符串值作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿保存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | 获取或设置一个值，指示文本文件中的字符串是否转换为日期数据。默认值为 true。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**已废弃。**) 如果为 true，当字符串值以字符 '=' 开头时将字符串转换为公式，默认值为 false。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | 获取或设置一个值，指示文本文件中的字符串是否转换为数值数据。默认值为 true。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | 获取或设置用于将要加载的工作簿的区域设置。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | 获取工作簿初始化样式的默认样式设置（继承自 [`LoadOptions`](../loadoptions/)。） |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | 指示在使用 `<br>` 标签换行时是否删除冗余空格。默认值为 false。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | 指示是否在 HTML 文件中检测 LaTeX 公式。默认值为 false。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | 获取或设置默认编码。仅适用于 csv 文件。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | 获取或设置各个字体配置。仅适用于使用此 [`LoadOptions`](../loadoptions/) 加载的 [`Workbook`](../workbook/)。 （继承自 [`LoadOptions`](../loadoptions/)。） |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | 指示如果文本以 "=" 开头，则该文本是否为公式。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | 指定在加载 HTML 时超链接的加载方式。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | 如果直接打印文件，则忽略未打印的数据。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | 指示是否忽略无用的形状。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | 获取或设置中断监视器。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | 指示如果字符串长度为 15，则不解析该字符串值。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | 指示从模板文件加载工作簿时是否在内存中保留未解析的数据。默认值为 true。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | 获取或设置基于保存文件的 CountryCode 的工作簿版本的用户界面语言。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | 读取模板文件时用于处理单元格数据的数据处理程序。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | 用于指示如何加载数据的过滤器。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | 获取加载格式。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | 指示如果原始 html 文件包含公式，是否导入公式。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | 指示在将字符串值转换为数字或日期时间时，对解析值应用样式的策略。（继承自 [`AbstractTextLoadOptions`](../abstracttextloadoptions/)。） |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | 获取或设置已加载工作簿的内存模式。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) 指定在加载 HTML 时 HTML &lt;p&gt; 元素的渲染方式。默认值为 Normal。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | 指定在加载 HTML 时 HTML &lt;p&gt; 元素的渲染方式。默认值为 Normal。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | 指示读取文件时是否解析公式。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | 指示加载文件时是否解析数据透视表缓存记录。默认值为 false。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | 获取或设置工作簿的密码。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行。默认值为 false。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | 获取创建文件的程序 ID。仅适用于 MHT 文件。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | 获取或设置用于将要加载的工作簿的区域设置。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) 设置默认的标准字体名称（继承自 [`LoadOptions`](../loadoptions/)。） |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) 设置默认的标准字体大小。（继承自 [`LoadOptions`](../loadoptions/)。） |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | 获取或设置用于导入对象的 StreamProviderImportHtmlFile。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | 指示在 html 文件包含 `<div>` 标记时是否支持其布局。默认值为 false。（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | 获取 HtmlTableLoadOptionCollection 实例（继承自 [`HtmlLoadOptions`](../htmlloadoptions/)。） |
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
    using System.IO;
    using System.Text;

    public class EbookLoadOptionsDemo
    {
        public static void EbookLoadOptionsExample()
        {
            // 创建 EbookLoadOptions 的实例
            EbookLoadOptions options = new EbookLoadOptions();

            // 设置属性
            options.AttachedFilesDirectory = "C:\\AttachedFiles";
            options.LoadFormulas = true;
            options.SupportDivTag = true;
            options.DeleteRedundantSpaces = true;
            options.AutoFitColsAndRows = true;
            options.ConvertFormulasData = true;
            options.HasFormula = true;
            options.Encoding = Encoding.UTF8;
            options.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            options.ConvertNumericData = true;
            options.ConvertDateTimeData = true;
            options.KeepPrecision = true;
            options.Password = "password";
            options.ParsingFormulaOnOpen = true;
            options.ParsingPivotCachedRecords = true;
            options.LanguageCode = CountryCode.USA;
            options.Region = CountryCode.USA;
            options.CultureInfo = new System.Globalization.CultureInfo("en-US");
            options.StandardFont = "Arial";
            options.StandardFontSize = 12.0;
            options.InterruptMonitor = null; // Assuming no interrupt monitor is set
            options.IgnoreNotPrinted = true;
            options.CheckDataValid = true;
            options.CheckExcelRestriction = true;
            options.KeepUnparsedData = true;
            options.LoadFilter = new LoadFilter();
            options.LightCellsDataHandler = null; // Assuming no light cells data handler is set
            options.MemorySetting = MemorySetting.Normal;
            options.WarningCallback = null; // Assuming no warning callback is set
            options.AutoFitterOptions = new AutoFitterOptions();
            options.AutoFilter = true;
            options.FontConfigs = new IndividualFontConfigs();
            options.IgnoreUselessShapes = true;
            options.PreservePaddingSpacesInFormula = true;

            // 使用指定的选项将电子书文件加载到 Workbook 中
            Workbook workbook = new Workbook("EbookLoadOptionsExample_original.ebook", options);

            // 将工作簿保存为 Excel 文件
            workbook.Save("EbookLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### 另请参见

* class [HtmlLoadOptions](../htmlloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


