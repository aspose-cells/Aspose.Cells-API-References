---
title: "SvgImageOptions 类"
linktitle: "SvgImageOptions"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "SvgImageOptions 类。封装在 Go 中表示 svgimageoptions 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/svgimageoptions/
---

## SvgImageOptions class

生成 SVG 图像的选项。

```go

type SvgImageOptions struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |
| [NewSvgImageOptions](./newsvgimageoptions/) | 构造函数。 |
| [NewSvgImageOptions_ImageOrPrintOptions](./newsvgimageoptions_imageorprintoptions/) | 从父对象构造。 |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetImageType](./getimagetype/) | 获取或设置生成图像的格式。默认值：PNG。 |
| [SetImageType](./setimagetype/) | 获取或设置生成图像的格式。默认值：PNG。 |
| [GetFitToViewPort](./getfittoviewport/) | 如果此属性为 true，生成的 svg 将适配视口。 |
| [SetFitToViewPort](./setfittoviewport/) | 如果此属性为 true，生成的 svg 将适配视口。 |
| [GetCssPrefix](./getcssprefix/) | 获取并设置 svg 中 css 名称的前缀，默认值为空字符串。 |
| [SetCssPrefix](./setcssprefix/) | 获取并设置 svg 中 css 名称的前缀，默认值为空字符串。 |
| [GetEmbeddedFontType](./getembeddedfonttype/) | 获取并设置嵌入 Svg 的字体类型。 |
| [SetEmbeddedFontType](./setembeddedfonttype/) | 获取并设置嵌入 Svg 的字体类型。 |
| [SetPrintWithStatusDialog](./setprintwithstatusdialog/) | 如果 PrintWithStatusDialog = true，将出现显示当前打印状态的对话框。否则不会显示此类对话框。 |
| [GetPrintWithStatusDialog](./getprintwithstatusdialog/) | 如果 PrintWithStatusDialog = true，将出现显示当前打印状态的对话框。否则不会显示此类对话框。 |
| [GetHorizontalResolution](./gethorizontalresolution/) | 获取或设置生成图像的水平分辨率（每英寸点数）。 |
| [SetHorizontalResolution](./sethorizontalresolution/) | 获取或设置生成图像的水平分辨率（每英寸点数）。 |
| [GetVerticalResolution](./getverticalresolution/) | 获取或设置生成图像的垂直分辨率（每英寸点数）。 |
| [SetVerticalResolution](./setverticalresolution/) | 获取或设置生成图像的垂直分辨率（每英寸点数）。 |
| [GetTiffCompression](./gettiffcompression/) | 获取或设置仅在将页面保存为 <c>Tiff</c> 格式时使用的压缩类型。 |
| [SetTiffCompression](./settiffcompression/) | 获取或设置仅在将页面保存为 <c>Tiff</c> 格式时使用的压缩类型。 |
| [GetTiffColorDepth](./gettiffcolordepth/) | 获取或设置仅在将页面保存为 <c>Tiff</c> 格式时使用的位深度。 |
| [SetTiffColorDepth](./settiffcolordepth/) | 获取或设置仅在将页面保存为 <c>Tiff</c> 格式时使用的位深度。 |
| [GetTiffBinarizationMethod](./gettiffbinarizationmethod/) | 获取或设置在 ImageType 为 Tiff 且 TiffCompression 等于 Ccitt3 或 Ccitt4 时，将图像转换为 1 bpp 格式所使用的方法。 |
| [SetTiffBinarizationMethod](./settiffbinarizationmethod/) | 获取或设置在 ImageType 为 Tiff 且 TiffCompression 等于 Ccitt3 或 Ccitt4 时，将图像转换为 1 bpp 格式所使用的方法。 |
| [GetPrintingPage](./getprintingpage/) | 指示哪些页面将不被打印。 |
| [SetPrintingPage](./setprintingpage/) | 指示哪些页面将不被打印。 |
| [GetQuality](./getquality/) | 获取或设置仅在将页面保存为 <c>Jpeg</c> 格式时用于确定生成图像质量的值。默认值为 100。 |
| [SetQuality](./setquality/) | 获取或设置仅在将页面保存为 <c>Jpeg</c> 格式时用于确定生成图像质量的值。默认值为 100。 |
| [GetOnePagePerSheet](./getonepagepersheet/) | 如果 OnePagePerSheet 为 true，则一个工作表的所有内容将输出到结果中的唯一一页。pagesetup 的纸张大小将失效，但 pagesetup 的其他设置仍会生效。 |
| [SetOnePagePerSheet](./setonepagepersheet/) | 如果 OnePagePerSheet 为 true，则一个工作表的所有内容将输出到结果中的唯一一页。pagesetup 的纸张大小将失效，但 pagesetup 的其他设置仍会生效。 |
| [GetAllColumnsInOnePagePerSheet](./getallcolumnsinonepagepersheet/) | 如果 AllColumnsInOnePagePerSheet 为 true，单个工作表的所有列内容将输出到结果中的唯一一页。pagesetup 的纸张宽度将失效，但 pagesetup 的其他设置仍然生效。 |
| [SetAllColumnsInOnePagePerSheet](./setallcolumnsinonepagepersheet/) | 如果 AllColumnsInOnePagePerSheet 为 true，单个工作表的所有列内容将输出到结果中的唯一一页。pagesetup 的纸张宽度将失效，但 pagesetup 的其他设置仍然生效。 |
| [GetDrawObjectEventHandler](./getdrawobjecteventhandler/) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [SetDrawObjectEventHandler](./setdrawobjecteventhandler/) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [GetOnlyArea](./getonlyarea/) | 如果此属性为 true，则会输出一个 Area，且不会生效任何比例。 |
| [SetOnlyArea](./setonlyarea/) | 如果此属性为 true，则会输出一个 Area，且不会生效任何比例。 |
| [GetTransparent](./gettransparent/) | 指示生成的图像背景是否应透明。 |
| [SetTransparent](./settransparent/) | 指示生成的图像背景是否应透明。 |
| [SetIsFontSubstitutionCharGranularity](./setisfontsubstitutionchargranularity/) | 指示是否仅在单元格字体与字符不兼容时替换该字符的字体。 |
| [IsFontSubstitutionCharGranularity](./isfontsubstitutionchargranularity/) | 指示是否仅在单元格字体与字符不兼容时替换该字符的字体。 |
| [SetPageIndex](./setpageindex/) | 获取或设置要保存的第一页的基于 0 的索引。 |
| [GetPageIndex](./getpageindex/) | 获取或设置要保存的第一页的基于 0 的索引。 |
| [SetPageCount](./setpagecount/) | 获取或设置要保存的页数。 |
| [GetPageCount](./getpagecount/) | 获取或设置要保存的页数。 |
| [SetDesiredSize](./setdesiredsize/) | 设置图像的期望宽度和高度。 |
| [IsOptimized](./isoptimized/) | 指示是否优化输出元素。 |
| [SetIsOptimized](./setisoptimized/) | 指示是否优化输出元素。 |
| [GetDefaultFont](./getdefaultfont/) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。请将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。 |
| [SetDefaultFont](./setdefaultfont/) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。请将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。 |
| [GetCheckWorkbookDefaultFont](./getcheckworkbookdefaultfont/) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。将此设置为 true，以尝试首先使用工作簿的默认字体来显示这些字符。 |
| [SetCheckWorkbookDefaultFont](./setcheckworkbookdefaultfont/) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确字体时，它们可能在 pdf、图像中显示为方块。将此设置为 true，以尝试首先使用工作簿的默认字体来显示这些字符。 |
| [GetOutputBlankPageWhenNothingToPrint](./getoutputblankpagewhennothingtoprint/) | 指示在没有内容可打印时是否输出空白页。 |
| [SetOutputBlankPageWhenNothingToPrint](./setoutputblankpagewhennothingtoprint/) | 指示在没有内容可打印时是否输出空白页。 |
| [GetGridlineType](./getgridlinetype/) | 获取或设置网格线类型。 |
| [SetGridlineType](./setgridlinetype/) | 获取或设置网格线类型。 |
| [GetGridlineColor](./getgridlinecolor/) | 获取或设置网格线颜色。 |
| [SetGridlineColor](./setgridlinecolor/) | 获取或设置网格线颜色。 |
| [GetTextCrossType](./gettextcrosstype/) | 获取或设置当文本宽度大于单元格宽度时的显示文本类型。 |
| [SetTextCrossType](./settextcrosstype/) | 获取或设置当文本宽度大于单元格宽度时的显示文本类型。 |
| [GetDefaultEditLanguage](./getdefaulteditlanguage/) | 获取或设置默认编辑语言。 |
| [SetDefaultEditLanguage](./setdefaulteditlanguage/) | 获取或设置默认编辑语言。 |
| [GetSheetSet](./getsheetset/) | 获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表：Aspose.Cells.Rendering.SheetSet.Visible。 |
| [SetSheetSet](./setsheetset/) | 获取或设置要渲染的工作表。默认是工作簿中所有可见的工作表：Aspose.Cells.Rendering.SheetSet.Visible。 |
| [GetEmfRenderSetting](./getemfrendersetting/) | 用于在源文件中渲染 Emf 元文件的设置。 |
| [SetEmfRenderSetting](./setemfrendersetting/) | 用于在源文件中渲染 Emf 元文件的设置。 |
| [GetCustomRenderSettings](./getcustomrendersettings/) | 获取或设置渲染期间的自定义设置。 |
| [SetCustomRenderSettings](./setcustomrendersettings/) | 获取或设置渲染期间的自定义设置。 |
