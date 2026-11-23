---
title: "类 PaginatedSaveOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.PaginatedSaveOptions 类。表示分页的选项"
type: docs
url: /zh/net/aspose.cells/paginatedsaveoptions/
---
## PaginatedSaveOptions class

表示分页的选项。

```csharp
public abstract class PaginatedSaveOptions : SaveOptions
```

## 属性

| 名称 | 描述 |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells/paginatedsaveoptions/allcolumnsinonepagepersheet/) { get; set; } | 如果 AllColumnsInOnePagePerSheet 为 true，则单个工作表的所有列内容将在结果中仅输出到一页。页面设置的纸张宽度将被忽略，而页面设置的其他设置仍然生效。 |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | 用于临时文件的文件夹，可用作数据缓存。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | 是否在用户修改单元格相关对象时检查 Excel 文件的限制。例如，Excel 不允许输入超过 32K 的字符串值。当您输入超过 32K 的值时，它将被截断。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [CheckFontCompatibility](../../aspose.cells/paginatedsaveoptions/checkfontcompatibility/) { get; set; } | 指示是否检查文本中每个字符的字体兼容性。 |
| [CheckWorkbookDefaultFont](../../aspose.cells/paginatedsaveoptions/checkworkbookdefaultfont/) { get; set; } | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将此设置为 true 可尝试首先使用工作簿的默认字体来显示这些字符。 |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | 在保存文件后使工作簿为空。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | 如果为 true 且目录不存在，目录将在保存文件之前自动创建。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [CustomRenderSettings](../../aspose.cells/paginatedsaveoptions/customrendersettings/) { get; set; } | 获取或设置渲染期间的自定义设置。 |
| [DefaultEditLanguage](../../aspose.cells/paginatedsaveoptions/defaulteditlanguage/) { get; set; } | 获取或设置默认编辑语言。 |
| [DefaultFont](../../aspose.cells/paginatedsaveoptions/defaultfont/) { get; set; } | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。 |
| [DrawObjectEventHandler](../../aspose.cells/paginatedsaveoptions/drawobjecteventhandler/) { get; set; } | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [EmfRenderSetting](../../aspose.cells/paginatedsaveoptions/emfrendersetting/) { get; set; } | 用于渲染 Emf 元文件的设置。 |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | 指示在保存为 .xls 文件时是否加密文档属性。默认值为 true。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [GridlineColor](../../aspose.cells/paginatedsaveoptions/gridlinecolor/) { get; set; } | 获取或设置网格线颜色。 |
| [GridlineType](../../aspose.cells/paginatedsaveoptions/gridlinetype/) { get; set; } | 获取或设置网格线类型。 |
| [IgnoreError](../../aspose.cells/paginatedsaveoptions/ignoreerror/) { get; set; } | 指示在渲染时是否需要隐藏错误。错误可能出现在形状、图像、图表渲染等方面。 |
| [IsFontSubstitutionCharGranularity](../../aspose.cells/paginatedsaveoptions/isfontsubstitutionchargranularity/) { get; set; } | 指示当单元格字体不兼容时是否仅替换字符的字体。 |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | 指示是否在保存文件前合并条件格式和验证的区域。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [OnePagePerSheet](../../aspose.cells/paginatedsaveoptions/onepagepersheet/) { get; set; } | 如果 OnePagePerSheet 为 true，单个工作表的所有内容将仅输出为结果中的一页。pagesetup 的纸张尺寸将失效，其他 pagesetup 设置仍然生效。 |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells/paginatedsaveoptions/outputblankpagewhennothingtoprint/) { get; set; } | 指示在没有内容可打印时是否输出空白页。 |
| [PageCount](../../aspose.cells/paginatedsaveoptions/pagecount/) { get; set; } | 获取或设置要保存的页数。 |
| [PageIndex](../../aspose.cells/paginatedsaveoptions/pageindex/) { get; set; } | 获取或设置要保存的第一页的零基索引。 |
| [PageSavingCallback](../../aspose.cells/paginatedsaveoptions/pagesavingcallback/) { get; set; } | 控制/指示页面保存过程的进度。 |
| [PrintingPageType](../../aspose.cells/paginatedsaveoptions/printingpagetype/) { get; set; } | 指示哪些页面不会被打印。 |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | 指示是否缓存图表的最新数据。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [RenderingBehavior](../../aspose.cells/paginatedsaveoptions/renderingbehavior/) { get; set; } | 获取或设置要应用的 Excel 特定渲染行为。 |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | 获取保存的文件格式。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [SheetSet](../../aspose.cells/paginatedsaveoptions/sheetset/) { get; set; } | 获取或设置要渲染的工作表。默认是工作簿中所有可见工作表：[`Visible`](../../aspose.cells.rendering/sheetset/visible/)。 |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | 指示是否在保存文件前对外部定义的名称进行排序。（Inherited from [`SaveOptions`](../saveoptions/).） |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | 指示是否在保存文件之前对已定义的名称进行排序。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [TextCrossType](../../aspose.cells/paginatedsaveoptions/textcrosstype/) { get; set; } | 获取或设置当文本宽度大于单元格宽度时的显示文本类型。 |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | 指示是否更新 Smart Art 设置。默认值为 false。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | 指示是否在保存文件之前验证合并单元格。（继承自 [`SaveOptions`](../saveoptions/)。） |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | 获取或设置警告回调。（继承自 [`SaveOptions`](../saveoptions/)。） |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PaginatedSaveOptionsDemo
    {
        public static void PaginatedSaveOptionsExample()
        {
            // 打开 Excel 文件
            Workbook workbook = new Workbook("PaginatedSaveOptionsExample_original.xlsx");

            // 创建 PaginatedSaveOptions 的实例
            PdfSaveOptions options = new PdfSaveOptions();

            // 设置属性
            options.DefaultFont = "Arial";
            options.CheckWorkbookDefaultFont = true;
            options.CheckFontCompatibility = true;
            options.IsFontSubstitutionCharGranularity = true;
            options.OnePagePerSheet = false;
            options.AllColumnsInOnePagePerSheet = false;
            options.IgnoreError = true;
            options.OutputBlankPageWhenNothingToPrint = false;
            options.PageIndex = 3; // Starting page index (0-based index)
            options.PageCount = 2; // Number of pages to be printed
            options.PrintingPageType = PrintingPageType.IgnoreBlank;
            options.GridlineType = GridlineType.Dotted;
            options.TextCrossType = TextCrossType.CrossKeep;
            options.DefaultEditLanguage = DefaultEditLanguage.English;
            options.SheetSet = new SheetSet(new int[] { workbook.Worksheets.ActiveSheetIndex });
            options.ClearData = false;
            options.CachedFileFolder = "C:\\Temp";
            options.ValidateMergedAreas = true;
            options.MergeAreas = true;
            options.SortNames = true;
            options.SortExternalNames = true;
            options.RefreshChartCache = true;
            options.UpdateSmartArt = false;

            // 保存 PDF 文件
            workbook.Save("PaginatedSaveOptionsExample.pdf", options);

            return;
        }
    }
}
```

### 另请参见

* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


