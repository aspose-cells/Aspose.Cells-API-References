---
title: ImageOrPrintOptions
second_title: Aspose.Cells for .NET API 参考
description: 允许在将工作表渲染为图像打印工作表或将图表渲染为图像时指定选项
type: docs
weight: 5140
url: /zh/net/aspose.cells.rendering/imageorprintoptions/
---
## ImageOrPrintOptions class

允许在将工作表渲染为图像、打印工作表或将图表渲染为图像时指定选项。

```csharp
public class ImageOrPrintOptions
```

## 构造函数

| 姓名 | 描述 |
| --- | --- |
| [ImageOrPrintOptions](imageorprintoptions)() | 默认构造函数。 |

## 特性

| 姓名 | 描述 |
| --- | --- |
| [AllColumnsInOnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/allcolumnsinonepagepersheet) { get; set; } | 如果 AllColumnsInOnePagePerSheet 为 true ，则一张表的所有列内容将只输出到结果中的一页。 pagesetup 的纸张尺寸宽度无效，pagesetup 的其他设置仍然有效。 |
| [CheckWorkbookDefaultFont](../../aspose.cells.rendering/imageorprintoptions/checkworkbookdefaultfont) { get; set; } | 当 Excel 中的字符为 Unicode 且未在单元格样式中设置正确的字体时， 它们可能在 pdf、图像中显示为块。 将此设置为 true 以尝试使用工作簿的默认字体首先显示这些字符。 |
| [CustomPrintPageEventHandler](../../aspose.cells.rendering/imageorprintoptions/customprintpageeventhandler) { get; set; } | 客户端可以在使用此 EventHandler 打印每一页时特殊输出到打印机 |
| [CustomQueryPageSettingsEventHandler](../../aspose.cells.rendering/imageorprintoptions/customquerypagesettingseventhandler) { get; set; } | 客户端可以在使用此事件处理程序打印每一页时控制打印机的页面设置 |
| [DefaultEditLanguage](../../aspose.cells.rendering/imageorprintoptions/defaulteditlanguage) { get; set; } | 获取或设置默认编辑语言。 |
| [DefaultFont](../../aspose.cells.rendering/imageorprintoptions/defaultfont) { get; set; } | 当 Excel 中的字符为 Unicode 且未在单元格样式中设置正确的字体时， 它们可能在 pdf、图像中显示为块。 设置默认字体如 MingLiu 或 MS Gothic 以显示这些字符。 如果未设置此属性，Aspose.Cells 将使用系统默认字体显示这些 unicode 字符。 |
| [DrawObjectEventHandler](../../aspose.cells.rendering/imageorprintoptions/drawobjecteventhandler) { get; set; } | 实现该接口，在渲染时获取DrawObject和Bound。 |
| [EmbededImageNameInSvg](../../aspose.cells.rendering/imageorprintoptions/embededimagenameinsvg) { get; set; } | 表示嵌入图像在 svg 中的文件名。 这应该是完整路径，其目录如“c:\\xpsEmbedded” |
| [EmfType](../../aspose.cells.rendering/imageorprintoptions/emftype) { get; set; } | 获取或设置指定元文件格式的 EmfType..  默认值为 EmfPlusDual。 |
| [GridlineType](../../aspose.cells.rendering/imageorprintoptions/gridlinetype) { get; set; } | 获取或设置网格线类型。 |
| [HorizontalResolution](../../aspose.cells.rendering/imageorprintoptions/horizontalresolution) { get; set; } | 获取或设置生成图像的水平分辨率，以每英寸点数为单位。 除 Emf 格式图像外，应用生成图像方法。 |
| [ImageType](../../aspose.cells.rendering/imageorprintoptions/imagetype) { get; set; } | 获取或设置生成图像的格式。 默认值:PNG。 |
| [IsCellAutoFit](../../aspose.cells.rendering/imageorprintoptions/iscellautofit) { get; set; } | 表示单元格的宽度和高度是否由单元格值自动拟合。 默认值为假。 |
| [IsFontSubstitutionCharGranularity](../../aspose.cells.rendering/imageorprintoptions/isfontsubstitutionchargranularity) { get; set; } | 表示当单元格字体不兼容时是否只替换字符的字体。 |
| [IsOptimized](../../aspose.cells.rendering/imageorprintoptions/isoptimized) { get; set; } | 表示是否优化输出元素。 |
| [OnePagePerSheet](../../aspose.cells.rendering/imageorprintoptions/onepagepersheet) { get; set; } | 如果 OnePagePerSheet 为 true ，则结果中一张表的所有内容将仅输出到一页。 pagesetup 的纸张大小会失效，pagesetup 的其他设置仍然有效。 |
| [OnlyArea](../../aspose.cells.rendering/imageorprintoptions/onlyarea) { get; set; } | 如果该属性为 true ，则输出一个Area，不进行缩放。 |
| [OutputBlankPageWhenNothingToPrint](../../aspose.cells.rendering/imageorprintoptions/outputblankpagewhennothingtoprint) { get; set; } | 表示在没有可打印的内容时是否输出空白页。 |
| [PageCount](../../aspose.cells.rendering/imageorprintoptions/pagecount) { get; set; } | 获取或设置要保存的页数。 |
| [PageIndex](../../aspose.cells.rendering/imageorprintoptions/pageindex) { get; set; } | 获取或设置要保存的第一页的从 0 开始的索引。 |
| [PageSavingCallback](../../aspose.cells.rendering/imageorprintoptions/pagesavingcallback) { get; set; } | 控制/指示页面保存过程的进度。 |
| [PixelFormat](../../aspose.cells.rendering/imageorprintoptions/pixelformat) { get; set; } | 获取或设置生成图像的像素格式。 |
| [PrintingPage](../../aspose.cells.rendering/imageorprintoptions/printingpage) { get; set; } | 指示不打印哪些页面。 |
| [PrintWithStatusDialog](../../aspose.cells.rendering/imageorprintoptions/printwithstatusdialog) { get; set; } | 如果 PrintWithStatusDialog = true ，将出现一个显示当前打印状态的对话框。 否则不会显示这样的对话框。 |
| [Quality](../../aspose.cells.rendering/imageorprintoptions/quality) { get; set; } | 获取或设置确定生成图像质量的值 仅在将页面保存到` 时应用Jpeg` 格式。默认值为 100 |
| [SaveFormat](../../aspose.cells.rendering/imageorprintoptions/saveformat) { get; set; } | 获取或设置输出文件格式类型 支持 Tiff/XPS |
| [SmoothingMode](../../aspose.cells.rendering/imageorprintoptions/smoothingmode) { get; set; } | 指定是否对线条和曲线以及填充区域的边缘应用平滑（抗锯齿）。 默认值为 SmoothingMode.None |
| [SVGFitToViewPort](../../aspose.cells.rendering/imageorprintoptions/svgfittoviewport) { get; set; } | 如果此属性为真，则生成的 svg 将适合查看端口。 |
| [TextCrossType](../../aspose.cells.rendering/imageorprintoptions/textcrosstype) { get; set; } | 获取或设置文本宽度大于单元格宽度时显示的文本类型。 |
| [TextRenderingHint](../../aspose.cells.rendering/imageorprintoptions/textrenderinghint) { get; set; } | 指定文本渲染的质量。 默认值为 TextRenderingHint.SystemDefault |
| [TiffColorDepth](../../aspose.cells.rendering/imageorprintoptions/tiffcolordepth) { get; set; } | 获取或设置仅在将页面保存为` Tiff` 格式时应用的位深度。 |
| [TiffCompression](../../aspose.cells.rendering/imageorprintoptions/tiffcompression) { get; set; } | 获取或设置仅在将页面保存为` Tiff` 格式时应用的压缩类型。 |
| [Transparent](../../aspose.cells.rendering/imageorprintoptions/transparent) { get; set; } | 指示生成图像的背景是否应该是透明的。 |
| [VerticalResolution](../../aspose.cells.rendering/imageorprintoptions/verticalresolution) { get; set; } | 获取或设置生成图像的垂直分辨率，以每英寸点数为单位。 除 Emf 格式图像外，应用生成图像方法。 |
| [WarningCallback](../../aspose.cells.rendering/imageorprintoptions/warningcallback) { get; set; } | 获取或设置警告回调。 |

## 方法

| 姓名 | 描述 |
| --- | --- |
| [SetDesiredSize](../../aspose.cells.rendering/imageorprintoptions/setdesiredsize)(int, int) | 设置图像的所需宽度和高度。 |

### 例子

```csharp

[C#]

 //设置图像或打印选项
ImageOrPrintOptions options = new ImageOrPrintOptions();

 //设置输出图像格式
options.ImageType = ImageType.Png;

 //设置水平分辨率
options.HorizontalResolution = 300;

 //设置垂直分辨率
options.VerticalResolution = 300;

 //实例化 Workbook
Workbook book = new Workbook("test.xls");

 //使用ImageOrPrint Options

book.Worksheets[0].Charts[0].ToImage("chart.png", options);

[VB.NET]

'设置图像或打印选项
Dim options As New ImageOrPrintOptions()

'设置输出图像格式
options.ImageType = ImageType.Png

'设置水平分辨率
options.HorizontalResolution = 300

'设置垂直分辨率
options.VerticalResolution = 300

'实例化 Workbook
Dim book As New Workbook("test.xls")

'使用 ImageOrPrint 选项将图表另存为图像
book.Worksheets(0).Charts(0).ToImage("chart.png", options)
```

### 也可以看看

* 命名空间 [Aspose.Cells.Rendering](../../aspose.cells.rendering)
* 部件 [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
