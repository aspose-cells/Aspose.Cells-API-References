---
title: "类 GridImageOrPrintOptions"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "Aspose.Cells.GridDesktop.Data.GridImageOrPrintOptions 类。允许在将工作表渲染为图像、打印工作表或将图表渲染为图像时指定选项"
type: docs
url: /zh/net/aspose.cells.griddesktop.data/gridimageorprintoptions/
---
## GridImageOrPrintOptions class

允许在将工作表渲染为图像、打印工作表或将图表渲染为图像时指定选项。

```csharp
public class GridImageOrPrintOptions
```

## 构造函数

| 名称 | 描述 |
| --- | --- |
| [GridImageOrPrintOptions](gridimageorprintoptions/)() | GridImageOrPrintOptions 的构造函数 |

## 属性

| 名称 | 描述 |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/allcolumnsinonepagepersheet/) { get; set; } | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将输出到结果的唯一一页。pagesetup 的纸张宽度将失效，而 pagesetup 的其他设置仍然生效。 |
| [CheckWorkbookDefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/checkworkbookdefaultfont/) { get; set; } | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将此设置为 true 可尝试首先使用工作簿的默认字体来显示这些字符。 |
| [DefaultFont](../../aspose.cells.griddesktop.data/gridimageorprintoptions/defaultfont/) { get; set; } | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。 |
| [EmbededImageNameInSvg](../../aspose.cells.griddesktop.data/gridimageorprintoptions/embededimagenameinsvg/) { get; set; } | 指示 SVG 中嵌入图像的文件名。应使用类似 "c:\\xpsEmbedded" 的完整目录路径。 |
| [EmfType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/emftype/) { get; set; } | 获取或设置一个 EmfType，指定元文件的格式。默认值为 EmfPlusDual。 |
| [GridlineType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/gridlinetype/) { get; set; } | 获取或设置网格线类型。 |
| [HorizontalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/horizontalresolution/) { get; set; } | 获取或设置生成图像的水平分辨率（每英寸点数）。适用于除 Emf 格式图像之外的图像生成方法。 |
| [ImageType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/imagetype/) { get; set; } | 获取或设置生成图像的格式。默认值：PNG。 |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isfontsubstitutionchargranularity/) { get; set; } | 指示当单元格字体不兼容时是否仅替换字符的字体。 |
| [IsOptimized](../../aspose.cells.griddesktop.data/gridimageorprintoptions/isoptimized/) { get; set; } | 指示是否优化输出元素。 |
| [OnePagePerSheet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onepagepersheet/) { get; set; } | 如果 OnePagePerSheet 为 true，单个工作表的所有内容将仅输出为结果中的一页。pagesetup 的纸张尺寸将失效，其他 pagesetup 设置仍然生效。 |
| [OnlyArea](../../aspose.cells.griddesktop.data/gridimageorprintoptions/onlyarea/) { get; set; } | 如果此属性为 true，则只输出一个区域，且不进行缩放。 |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/outputblankpagewhennothingtoprint/) { get; set; } | 指示在没有内容可打印时是否输出空白页。 |
| [PageCount](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pagecount/) { get; set; } | 获取或设置要保存的页数。 |
| [PageIndex](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pageindex/) { get; set; } | 获取或设置要保存的第一页的零基索引。 |
| [PixelFormat](../../aspose.cells.griddesktop.data/gridimageorprintoptions/pixelformat/) { get; set; } | 获取或设置生成图像的像素格式。 |
| [PrintingPage](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printingpage/) { get; set; } | 指示哪些页面不会被打印。 |
| [PrintWithStatusDialog](../../aspose.cells.griddesktop.data/gridimageorprintoptions/printwithstatusdialog/) { get; set; } | 如果 PrintWithStatusDialog = true，则会出现显示当前打印状态的对话框；否则不会显示此类对话框。 |
| [Quality](../../aspose.cells.griddesktop.data/gridimageorprintoptions/quality/) { get; set; } | 获取或设置一个值，用于确定生成图像的质量，仅在将页面保存为 `Jpeg` 格式时使用。默认值为 100。 |
| [SmoothingMode](../../aspose.cells.griddesktop.data/gridimageorprintoptions/smoothingmode/) { get; set; } | 指定是否对线条、曲线以及填充区域的边缘应用平滑（抗锯齿）。默认值为 SmoothingMode.None。 |
| [SVGFitToViewPort](../../aspose.cells.griddesktop.data/gridimageorprintoptions/svgfittoviewport/) { get; set; } | 如果此属性为 true，生成的 svg 将适配视口。 |
| [TextCrossType](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textcrosstype/) { get; set; } | 获取或设置当文本宽度大于单元格宽度时的显示文本类型。 |
| [TextRenderingHint](../../aspose.cells.griddesktop.data/gridimageorprintoptions/textrenderinghint/) { get; set; } | 指定文本渲染的质量。默认值为 TextRenderingHint.SystemDefault |
| [Transparent](../../aspose.cells.griddesktop.data/gridimageorprintoptions/transparent/) { get; set; } | 指示生成的图像背景是否应透明。 |
| [VerticalResolution](../../aspose.cells.griddesktop.data/gridimageorprintoptions/verticalresolution/) { get; set; } | 获取或设置生成图像的垂直分辨率，单位为每英寸点数。适用于除 Emf 格式图像之外的生成图像方法。 |

## 方法

| 名称 | 描述 |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setdesiredsize/)(int, int) | 设置图像的期望宽度和高度。 |
| [setRenderSheetSet](../../aspose.cells.griddesktop.data/gridimageorprintoptions/setrendersheetset/)(int[]) | 设置要渲染的工作表。默认是工作簿中所有可见的工作表。基于零的工作表索引。 |

### 另请参见

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


