---
title: "类 SvgImageOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.Rendering.SvgImageOptions 类。生成 Svg 图像的选项"
type: docs
url: /zh/net/aspose.cells.rendering/svgimageoptions/
---
## SvgImageOptions class

生成 Svg 图像的选项。

```csharp
public class SvgImageOptions : ImageOrPrintOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [SvgImageOptions](svgimageoptions/)() | 构造函数。 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将仅输出到结果的一个页面。pagesetup 的纸张尺寸宽度将失效，pagesetup 的其他设置仍然生效。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [ChartImageType](../../aspose.cells.rendering/imageorprintoptions/chartimagetype/) { get; set; } | (**Obsolete.**) 指示转换时的图表图像类型。默认值：PNG。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont/) { get; set; } | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。将此设置为 true，以尝试首先使用工作簿的默认字体显示这些字符。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CssPrefix](../../aspose.cells.rendering/svgimageoptions/cssprefix/) { get; set; } | 获取和设置 svg 中 css 名称的前缀，默认值为空字符串。 |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler/) { get; set; } | 客户端可以在使用此 EventHandler 打印每页时将输出定向到打印机。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler/) { get; set; } | 客户端可以在使用此 EventHandler 打印每页时控制打印机的页面设置。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [CustomRenderSettings](../../aspose.cells.rendering/imageorprintoptions/customrendersettings/) { get; set; } | 获取或设置渲染期间的自定义设置。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage/) { get; set; } | 获取或设置默认编辑语言。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont/) { get; set; } | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler/) { get; set; } | 实现此接口以在渲染时获取 DrawObject 和 Bound。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmbeddedFontType](../../aspose.cells.rendering/svgimageoptions/embeddedfonttype/) { get; set; } | 获取或设置嵌入到 Svg 中的字体类型。 |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg/) { get; set; } | (**Obsolete.**) 指示嵌入到 svg 中的图像文件名。它应是类似 "c:\\xpsEmbedded" 的完整目录路径。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfRenderSetting](../../aspose.cells.rendering/imageorprintoptions/emfrendersetting/) { get; set; } | 用于在源文件中渲染 Emf 元文件的设置。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype/) { get; set; } | 获取或设置指定元文件格式的 EmfType。默认值为 EmfPlusDual。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [FitToViewPort](../../aspose.cells.rendering/svgimageoptions/fittoviewport/) { get; set; } | 如果此属性为 true，生成的 svg 将适配视口。 |
| [GridlineColor](../../aspose.cells.rendering/imageorprintoptions/gridlinecolor/) { get; set; } | 获取或设置网格线颜色。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype/) { get; set; } | 获取或设置网格线类型。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution/) { get; set; } | 获取或设置生成图像的水平分辨率（单位为每英寸点数）。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| override [ImageType](../../aspose.cells.rendering/svgimageoptions/imagetype/) { get; set; } | 获取或设置生成图像的格式。默认值：PNG。 |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit/) { get; set; } | (**Obsolete.**) 指示单元格的宽度和高度是否自动根据单元格值进行适配。默认值为 false。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | 指示当单元格字体与字符不兼容时是否仅替换字符的字体。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized/) { get; set; } | 指示是否优化输出元素。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet/) { get; set; } | 如果 OnePagePerSheet 为 true，单个工作表的所有内容将仅输出到结果中的一页。pagesetup 的纸张大小将失效，pagesetup 的其他设置仍然有效。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea/) { get; set; } | 如果此属性为 true，则只输出一个区域，且不应用缩放。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | 指示当没有内容可打印时是否输出空白页。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount/) { get; set; } | 获取或设置要保存的页数。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex/) { get; set; } | 获取或设置要保存的第一页的基于 0 的索引。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback/) { get; set; } | 控制/指示页面保存过程的进度。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat/) { get; set; } | 获取或设置生成图像的像素格式。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage/) { get; set; } | 指示哪些页面不会被打印。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog/) { get; set; } | 如果 PrintWithStatusDialog = true，将出现显示当前打印状态的对话框。否则不会显示此类对话框。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality/) { get; set; } | 获取或设置一个值，用于确定生成图像的质量，仅在将页面保存为 `Jpeg` 格式时适用。默认值为 100(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat/) { get; set; } | (**Obsolete.**) 获取或设置输出文件格式类型，支持 Tiff/XPS(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SheetSet](../../aspose.cells.rendering/imageorprintoptions/sheetset/) { get; set; } | 获取或设置要渲染的工作表。默认是工作簿中所有可见工作表：[`Visible`](../sheetset/visible/).(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode/) { get; set; } | 指定是否对线条、曲线以及填充区域的边缘应用平滑（抗锯齿）。默认值为 SmoothingMode.None(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SvgCssPrefix](../../aspose.cells.rendering/imageorprintoptions/svgcssprefix/) { get; set; } | (**Obsolete.**) 获取和设置 svg 中 css 名称的前缀，默认值为空字符串.(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport/) { get; set; } | (**Obsolete.**) 如果此属性为 true，生成的 svg 将适配视口。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype/) { get; set; } | 获取或设置当文本宽度大于单元格宽度时的显示文本类型。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint/) { get; set; } | 指定文本渲染的质量。默认值为 TextRenderingHint.SystemDefault(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffBinarizationMethod](../../aspose.cells.rendering/imageorprintoptions/tiffbinarizationmethod/) { get; set; } | 获取或设置在将图像转换为 1 bpp 格式时使用的方法，当 [`ImageType`](../imageorprintoptions/imagetype/) 为 Tiff 且 [`TiffCompression`](../imageorprintoptions/tiffcompression/) 等于 Ccitt3 或 Ccitt4 时。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth/) { get; set; } | 获取或设置仅在将页面保存为 `Tiff` 格式时使用的位深度。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression/) { get; set; } | 获取或设置仅在将页面保存为 `Tiff` 格式时使用的压缩类型。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent/) { get; set; } | 指示生成图像的背景是否应透明。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution/) { get; set; } | 获取或设置生成图像的垂直分辨率（每英寸点数）。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback/) { get; set; } | 获取或设置警告回调。(Inherited from [`ImageOrPrintOptions`](../imageorprintoptions/).) |

## 方法

| 名称 | 描述 |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int) | (**Obsolete.**) 设置图像的期望宽度和高度。(继承自 [`ImageOrPrintOptions`](../imageorprintoptions/).) |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize/)(int, int, bool) | 设置图像的期望宽度和高度。(继承自 [`ImageOrPrintOptions`](../imageorprintoptions/).) |

### 示例

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Rendering;
    using System;

    public class RenderingClassSvgImageOptionsDemo
    {
        public static void Run()
        {
            // 创建一个新的工作簿并访问第一个工作表
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // 为图表填充示例数据
            worksheet.Cells["A1"].PutValue("Q1");
            worksheet.Cells["A2"].PutValue(12000);
            worksheet.Cells["A3"].PutValue(16500);
            worksheet.Cells["B1"].PutValue("Q2");
            worksheet.Cells["B2"].PutValue(25500);
            worksheet.Cells["B3"].PutValue(10800);

            // 创建柱状图
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A2:B3", true);
            chart.NSeries.CategoryData = "A1:B1";

            // 初始化 SVG 图像选项
            SvgImageOptions svgOptions = new SvgImageOptions();
            
            // 配置 SVG 渲染选项
            svgOptions.FitToViewPort = true;
            svgOptions.CssPrefix = "chart-";
            svgOptions.EmbeddedFontType = SvgEmbeddedFontType.Woff;
            svgOptions.ImageType = ImageType.Svg;

            // 设置打印质量和分辨率
            svgOptions.PrintWithStatusDialog = true;
            svgOptions.HorizontalResolution = 300;
            svgOptions.VerticalResolution = 300;

            // 使用配置的选项将图表渲染为 SVG
            chart.ToImage("chart_output.svg", svgOptions);

            // 演示工作簿保存集成
            workbook.Save("SvgRenderingDemo.xlsx");
        }
    }
}
```

### 另请参见

* class [ImageOrPrintOptions](../imageorprintoptions/)
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


