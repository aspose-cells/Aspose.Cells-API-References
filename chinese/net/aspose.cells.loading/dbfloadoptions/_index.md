---
title: "类 DbfLoadOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Loading.DbfLoadOptions 类。表示加载 .dbf 文件的选项"
type: docs
url: /zh/net/aspose.cells.loading/dbfloadoptions/
---
## DbfLoadOptions class

表示加载 .dbf 文件的选项。

```csharp
public class DbfLoadOptions : LoadOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [DbfLoadOptions](dbfloadoptions/)() | 这些选项。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | 指示在加载文件时是否自动过滤数据。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | 获取和设置自动适配选项（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | 检查模板文件中的数据是否有效。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改与单元格相关的对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您通过 Cell.PutValue(string) 输入超过 32K 的值时，如果此属性为 true，您将收到异常；如果此属性为 false，我们将接受您的输入字符串作为单元格的值，以便随后您可以将完整的字符串值输出为其他文件格式，如 CSV。然而，如果您设置了对 Excel 文件格式无效的此类值，之后不应将工作簿另存为 Excel 文件格式。否则生成的 Excel 文件可能会出现意外错误。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | 获取或设置将用于加载的工作簿的区域设置。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | 获取用于初始化工作簿样式的默认样式设置（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | 获取和设置单独的字体配置。仅适用于使用此 [`LoadOptions`](../../aspose.cells/loadoptions/) 加载的 [`Workbook`](../../aspose.cells/workbook/)。 （继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | 在直接打印文件时忽略未打印的数据（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | 指示是否忽略无用的形状。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | 获取和设置中断监视器。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | 是否在从模板文件加载工作簿时将未解析的数据保存在内存中。默认值为 true。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | 获取或设置基于保存文件的 CountryCode 的工作簿版本的用户界面语言。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | 读取模板文件时用于处理单元格数据的数据处理程序。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | 用于指示如何加载数据的过滤器。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | 获取加载格式。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | 获取或设置已加载工作簿的内存模式。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | 指示在读取文件时是否解析公式。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | 指示在加载文件时是否解析数据透视表缓存记录。默认值为 false。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | 获取和设置工作簿的密码。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | 指示在获取和设置公式时是否保留公式标记之间填充的空格和换行符。默认值为 false。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | 获取或设置将用于加载的工作簿的区域设置。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) 设置默认标准字体名称（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) 设置默认标准字体大小。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | 获取或设置警告回调。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |

## 方法

| 名称 | 描述 |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | 从默认打印机的设置中设置默认打印纸张大小。（继承自 [`LoadOptions`](../../aspose.cells/loadoptions/)。） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Loading;

    public class LoadingClassDbfLoadOptionsDemo
    {
        public static void Run()
        {
            // 创建 DbfLoadOptions 实例
            DbfLoadOptions loadOptions = new DbfLoadOptions();

            // 使用 DBF 加载选项创建工作簿
            Workbook workbook = new Workbook("sample.dbf", loadOptions);

            // 访问第一个工作表
            Worksheet worksheet = workbook.Worksheets[0];

            // 修改某些单元格（演示与其他组件的集成）
            worksheet.Cells["A1"].PutValue("Modified DBF Data");
            
            // 以 Excel 格式保存工作簿
            workbook.Save("DbfLoadOptionsDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### 另请参见

* class [LoadOptions](../../aspose.cells/loadoptions/)
* namespace [Aspose.Cells.Loading](../../aspose.cells.loading/)
* assembly [Aspose.Cells](../../)


