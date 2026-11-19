---
title: "ImageOrPrintOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "允许在将工作表渲染为图像、打印工作表或将图表渲染为图像时指定选项。"
type: docs
url: /zh/java/com.aspose.cells/imageorprintoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImageOrPrintOptions
```

允许在将工作表渲染为图像、打印工作表或将图表渲染为图像时指定选项。

**Example**

```
         //Set Image Or Print Options
         ImageOrPrintOptions options = new ImageOrPrintOptions();
 
         //Set output image format
         options.setImageType(ImageType.PNG);
 
         //Set Horizontal resolution
         options.setHorizontalResolution(300);
 
         //Set Vertical Resolution
         options.setVerticalResolution(300);
 
         //Instantiate Workbook
         Workbook book = new Workbook("test.xls");
 
         //Save chart as Image using ImageOrPrint Options
         book.getWorksheets().get(0).getCharts().get(0).toImage("chart.png", options);
```
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [ImageOrPrintOptions()](#ImageOrPrintOptions--) | 构造函数。 |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将仅输出到结果中的一页。 |
| [getChartImageType()](#getChartImageType--) | 指示转换时的图表图像类型。 |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。 |
| [getClass()](#getClass--) |  |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | 获取渲染期间的自定义设置。 |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | 获取默认编辑语言。 |
| [getDefaultFont()](#getDefaultFont--) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。 |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | 指示嵌入在 svg 中的图像文件名。 |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | 用于在源文件中渲染 Emf 元文件的设置。 |
| [getGridlineColor()](#getGridlineColor--) | 获取网格线颜色。 |
| [getGridlineType()](#getGridlineType--) | 获取网格线类型。 |
| [getHorizontalResolution()](#getHorizontalResolution--) | 获取生成图像的水平分辨率，单位为每英寸点数。 |
| [getImageType()](#getImageType--) | 获取生成图像的格式。 |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | 如果 OnePagePerSheet 为 true，则一个工作表的所有内容将仅输出到结果中的一页。 |
| [getOnlyArea()](#getOnlyArea--) | 如果此属性为 true，则只输出一个区域，且不应用缩放。 |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | 指示在没有可打印内容时是否输出空白页。 |
| [getPageCount()](#getPageCount--) | 获取要保存的页数。 |
| [getPageIndex()](#getPageIndex--) | 获取要保存的第一页的基于 0 的索引。 |
| [getPageSavingCallback()](#getPageSavingCallback--) | 控制/指示页面保存过程的进度。 |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | 如果 PrintWithStatusDialog = true，则会出现显示当前打印状态的对话框。 |
| [getPrintingPage()](#getPrintingPage--) | 指示哪些页面将不会被打印。 |
| [getQuality()](#getQuality--) | 获取用于确定生成图像质量的值，仅在将页面保存为 `Jpeg` 格式时应用。 |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | 如果此属性为 true，生成的 svg 将适应视口。 |
| [getSaveFormat()](#getSaveFormat--) | 获取输出文件格式类型，支持 Tiff/XPS。 |
| [getSheetSet()](#getSheetSet--) | 获取要渲染的工作表。 |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | 获取 svg 中 css 名称的前缀，默认值为空字符串。 |
| [getTextCrossType()](#getTextCrossType--) | 获取当文本宽度大于单元格宽度时的显示文本类型。 |
| [getTiffColorDepth()](#getTiffColorDepth--) | 获取位深度，仅在将页面保存为 `Tiff` 格式时应用。 |
| [getTiffCompression()](#getTiffCompression--) | 获取压缩类型，仅在将页面保存为 `Tiff` 格式时应用。 |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | 获取光度解释类型，仅在将页面保存为 `Tiff` 格式时应用。 |
| [getTransparent()](#getTransparent--) | 指示生成图像的背景是否应为透明。 |
| [getVerticalResolution()](#getVerticalResolution--) | 获取生成图像的垂直分辨率，单位为每英寸点数。 |
| [getWarningCallback()](#getWarningCallback--) | 获取警告回调。 |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | 指示单元格的宽度和高度是否根据单元格值自动适配。 |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | 指示当单元格字体与字符不兼容时是否仅替换该字符的字体。 |
| [isOptimized()](#isOptimized--) | 指示是否优化输出元素。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | 如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将仅输出到结果中的一页。 |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | 指示单元格的宽度和高度是否根据单元格值自动适配。 |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | 指示转换时的图表图像类型。 |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。 |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | 设置渲染期间的自定义设置。 |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | 设置默认编辑语言。 |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | 当 Excel 中的字符是 Unicode 且单元格样式未设置正确的字体时，它们可能在 pdf、image 中显示为方块。 |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | 设置图像的期望宽度和高度。 |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | 设置图像的期望宽度和高度。 |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | 实现此接口以在渲染时获取 DrawObject 和 Bound。 |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | 指示嵌入在 svg 中的图像文件名。 |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | 用于在源文件中渲染 Emf 元文件的设置。 |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | 指示当单元格字体与字符不兼容时是否仅替换该字符的字体。 |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | 设置网格线颜色。 |
| [setGridlineType(int value)](#setGridlineType-int-) | 设置网格线类型。 |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | 设置生成图像的水平分辨率，单位为每英寸点数。 |
| [setImageType(int value)](#setImageType-int-) | 设置生成图像的格式。 |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | 如果 OnePagePerSheet 为 true，则一个工作表的所有内容将仅输出到结果中的一页。 |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | 如果此属性为 true，则只输出一个区域，且不应用缩放。 |
| [setOptimized(boolean value)](#setOptimized-boolean-) | 指示是否优化输出元素。 |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | 指示在没有可打印内容时是否输出空白页。 |
| [setPageCount(int value)](#setPageCount-int-) | 设置要保存的页数。 |
| [setPageIndex(int value)](#setPageIndex-int-) | 设置要保存的第一页的基于 0 的索引。 |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | 控制/指示页面保存过程的进度。 |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | 如果 PrintWithStatusDialog = true，则会出现显示当前打印状态的对话框。 |
| [setPrintingPage(int value)](#setPrintingPage-int-) | 指示哪些页面将不会被打印。 |
| [setQuality(int value)](#setQuality-int-) | 设置用于确定生成图像质量的值，仅在将页面保存为 `Jpeg` 格式时应用。 |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | 设置渲染算法的单个首选项值。 |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | 如果此属性为 true，生成的 svg 将适应视口。 |
| [setSaveFormat(int value)](#setSaveFormat-int-) | 设置输出文件格式类型，支持 Tiff/XPS。 |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | 设置要渲染的工作表。 |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | 设置 svg 中 css 名称的前缀，默认值为空字符串。 |
| [setTextCrossType(int value)](#setTextCrossType-int-) | 当文本宽度大于单元格宽度时，设置显示文本的类型。 |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | 设置位深度，仅在将页面保存为 `Tiff` 格式时应用。 |
| [setTiffCompression(int value)](#setTiffCompression-int-) | 设置压缩类型，仅在将页面保存为 `Tiff` 格式时应用。 |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | 设置光度解释类型，仅在将页面保存为 `Tiff` 格式时应用。 |
| [setTransparent(boolean value)](#setTransparent-boolean-) | 指示生成图像的背景是否应为透明。 |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | 设置生成图像的垂直分辨率，单位为每英寸点数（dpi）。 |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | 设置警告回调。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ImageOrPrintOptions() {#ImageOrPrintOptions--}
```
public ImageOrPrintOptions()
```


构造函数。

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```


如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将仅输出到结果的一个页面。pagesetup 的纸张尺寸宽度将失效，pagesetup 的其他设置仍然生效。

**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```


指示转换时的图表图像类型。默认值：PNG。

**Remarks**

NOTE: 此成员现已过时。取而代之的是，为了渲染质量，Chart 和 Shape 将始终以向量元素（例如点、线）渲染。此属性将在自 2022 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


当 Excel 中的字符为 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将此设置为 true 可尝试使用工作簿的默认字体首先显示这些字符。

**Remarks**

默认值为 true。

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```


获取渲染期间的自定义设置。

**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


获取默认编辑语言。

参见 [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage)。

**Remarks**

当设置不同的编辑语言时，可能会显示/渲染文本段落的不同布局。默认值为 [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO)。

**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```


当 Excel 中的字符为 Unicode 且单元格样式未设置正确的字体时，它们可能显示为方块。将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。

**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


实现此接口以在渲染时获取 DrawObject 和 Bound。

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


指示嵌入到 svg 中的图像文件名。应使用类似 "c:\\\\xpsEmbedded" 的完整目录路径。

**Remarks**

NOTE: 此成员现已过时。请删除此属性，因为图像现在始终以 base64 格式嵌入到 Svg 中。此属性将在自 2025 年 4 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```


用于在源文件中渲染 Emf 元文件的设置。

参见 [EmfRenderSetting](../../com.aspose.cells/emfrendersetting)。

**Remarks**

EMF 元文件标识为 “EMF+ Dual” 可以同时包含 EMF+ 记录和 EMF 记录。可以使用任一类型的记录来渲染图像、仅使用 EMF+ 记录或仅使用 EMF 记录。当设置了 [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) 时，渲染图像时将解析 EMF+ 记录，否则仅解析 EMF 记录。默认值是 [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY)。对于依赖 .NET System.Drawing.Common 的框架，此设置将被忽略。

**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```


获取网格线颜色。

**Remarks**

它将忽略源文件中的网格线颜色设置。

**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


获取网格线类型。

参见 [GridlineType](../../com.aspose.cells/gridlinetype)。

**Remarks**

默认值为 Dotted 类型。

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


获取生成图像的水平分辨率，单位为每英寸点数。

**Remarks**

默认值为 96。设置  和  会影响输出图像的宽度和高度（单位：像素）。

**Example**

以下代码将分辨率设置为 192，生成图像的宽度和高度是保持默认分辨率 96 时的两倍。

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render worksheet page to image.
         SheetRender sr = new SheetRender(wb.getWorksheets().get(0), opts);
         sr.toImage(0, "Sheet_Page1.png");
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


获取生成图像的格式。默认值：PNG。

参见 [ImageType](../../com.aspose.cells/imagetype)。

**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```


如果 OnePagePerSheet 为 true，则单个工作表的所有内容将仅输出到结果的一个页面。页面设置的纸张大小将失效，页面设置的其他设置仍然生效。

**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```


如果此属性为 true，则只输出一个区域，且不应用缩放。

**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


指示在没有可打印内容时是否输出空白页。

**Remarks**

默认值为 false。

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


获取要保存的页数。

**Remarks**

默认值为 System.Int32.MaxValue，表示将渲染所有页面。

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


获取要保存的第一页的基于 0 的索引。

**Remarks**

默认值为 0。

**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```


控制/指示页面保存过程的进度。

**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```


如果 PrintWithStatusDialog = true，则会出现显示当前打印状态的对话框；否则不会显示此类对话框。

**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```


指示哪些页面将不会被打印。

参见 [PrintingPageType](../../com.aspose.cells/printingpagetype)。

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


获取一个值，用于确定生成图像的质量，仅在将页面保存为 `Jpeg` 格式时应用。默认值为 100。

**Remarks**

仅在保存为 JPEG 时生效。取值必须在 0 到 100 之间。默认值为 100。

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


如果此属性为 true，生成的 svg 将适应视口。

**Remarks**

NOTE: 此成员现已过时。请改用 [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--)。此属性将在自 2025 年 4 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


获取输出文件格式类型，支持 Tiff/XPS。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

**Remarks**

NOTE: 此成员现已过时。对于 Tiff/Svg，请使用 [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--)；对于 Xps，请使用带有 [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions) 的 [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-)。此属性将在自 2022 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


获取要渲染的工作表。默认是工作簿中所有可见工作表：[SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--)。

**Remarks**

当在 [SheetRender](../../com.aspose.cells/sheetrender) 中使用时，此设置将被忽略。

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```


获取 svg 中 css 名称的前缀，默认值为空字符串。

**Remarks**

NOTE: 此成员现已过时。请改用 [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--)。此属性将在自 2025 年 4 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


获取当文本宽度大于单元格宽度时的显示文本类型。

请参阅 [TextCrossType](../../com.aspose.cells/textcrosstype)。

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


获取位深度，仅在将页面保存为 `Tiff` 格式时应用。

参见 [ColorDepth](../../com.aspose.cells/colordepth)。

**Remarks**

仅在保存为 TIFF 时生效。如果 TiffCompression 设置为 CCITT3、CCITT4，则此设置不生效，生成的 tiff 图像的位深度始终为 1。

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


获取压缩类型，仅在将页面保存为 `Tiff` 格式时应用。

参见 [TiffCompression](../../com.aspose.cells/tiffcompression)。

**Remarks**

仅在保存为 TIFF 时生效。默认值为 Lzw。

**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```


获取光度解释类型，仅在将页面保存为 `Tiff` 格式时应用。

**Remarks**

仅在保存为 TIFF 时生效。默认值为 -1，表示未应用 PhotometricInterpretation。

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


指示生成图像的背景是否应为透明。

**Remarks**

默认值为 false。这意味着生成的图像背景为白色。

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


获取生成图像的垂直分辨率，单位为每英寸点数。

**Remarks**

默认值为 96。设置  和  会影响输出图像的宽度和高度（单位：像素）。

**Example**

以下代码将分辨率设置为 192，生成图像的宽度和高度是保持默认分辨率 96 时的两倍。

```
         Workbook wb = new Workbook("Book1.xlsx");
 
         ImageOrPrintOptions opts = new ImageOrPrintOptions();
 
         //Set output image type: png.
         opts.setImageType(ImageType.PNG);
 
         //Set resolution to 192.
         opts.setHorizontalResolution(192);
         opts.setVerticalResolution(192);
 
         //Render Chart to image.
         wb.getWorksheets().get(0).getCharts().get(0).toImage("Chart.png", opts);
```

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


获取警告回调。

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isCellAutoFit() {#isCellAutoFit--}
```
public boolean isCellAutoFit()
```


指示单元格的宽度和高度是否根据单元格值自动适配。默认值为 false。

**Remarks**

注意：此成员已过时。相反，此属性不再使用，请删除此属性。此属性将在自 2022 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


指示当单元格字体与字符不兼容时是否仅替换该字符的字体。

**Remarks**

默认值为 false。我们将首先尝试 Workbook 的默认字体以及 PdfSaveOption/system 用于单元格字体。

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


指示是否优化输出元素。

**Remarks**

默认值为 false。目前当此属性设置为 true 时，将进行以下优化：1. 优化边框线。2. 在渲染为 Svg 图像时优化文件大小。

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setAllColumnsInOnePagePerSheet(boolean value) {#setAllColumnsInOnePagePerSheet-boolean-}
```
public void setAllColumnsInOnePagePerSheet(boolean value)
```


如果 AllColumnsInOnePagePerSheet 为 true，则一个工作表的所有列内容将仅输出到结果的一个页面。pagesetup 的纸张尺寸宽度将失效，pagesetup 的其他设置仍然生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```


指示单元格的宽度和高度是否根据单元格值自动适配。默认值为 false。

**Remarks**

注意：此成员已过时。相反，此属性不再使用，请删除此属性。此属性将在自 2022 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```


指示转换时的图表图像类型。默认值：PNG。

**Remarks**

NOTE: 此成员现已过时。取而代之的是，为了渲染质量，Chart 和 Shape 将始终以向量元素（例如点、线）渲染。此属性将在自 2022 年 6 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


当 Excel 中的字符为 Unicode 且单元格样式未设置正确的字体时，它们可能在 PDF、图像中显示为方块。将此设置为 true 可尝试使用工作簿的默认字体首先显示这些字符。

**Remarks**

默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```


设置渲染期间的自定义设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


设置默认编辑语言。

参见 [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage)。

**Remarks**

当设置不同的编辑语言时，可能会显示/渲染文本段落的不同布局。默认值为 [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


当 Excel 中的字符为 Unicode 且单元格样式未设置正确的字体时，它们可能显示为方块。将 DefaultFont 设置为如 MingLiu 或 MS Gothic 等字体以显示这些字符。如果未设置此属性，Aspose.Cells 将使用系统默认字体来显示这些 Unicode 字符。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


设置图像的期望宽度和高度。

**Remarks**

注意：此成员已过时。请改为使用 [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) 并将参数 keepAspectRatio 设置为 false。此属性将在自 2023 年 5 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| desiredWidth | int | 以像素为单位的期望宽度 |
| desiredHeight | int | 以像素为单位的期望高度 |

### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```


设置图像的期望宽度和高度。

**Remarks**

输出图像的宽度和高度（以像素为单位）仅基于设置的期望宽度和高度。在这种情况下， 和  不会影响输出图像的宽度和高度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| desiredWidth | int | 以像素为单位的期望宽度 |
| desiredHeight | int | 以像素为单位的期望高度 |
| keepAspectRatio | boolean | 是否保持原始图像的宽高比 |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


实现此接口以在渲染时获取 DrawObject 和 Bound。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```


指示嵌入到 svg 中的图像文件名。应使用类似 "c:\\\\xpsEmbedded" 的完整目录路径。

**Remarks**

NOTE: 此成员现已过时。请删除此属性，因为图像现在始终以 base64 格式嵌入到 Svg 中。此属性将在自 2025 年 4 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


用于在源文件中渲染 Emf 元文件的设置。

参见 [EmfRenderSetting](../../com.aspose.cells/emfrendersetting)。

**Remarks**

EMF 元文件标识为 “EMF+ Dual” 可以同时包含 EMF+ 记录和 EMF 记录。可以使用任一类型的记录来渲染图像、仅使用 EMF+ 记录或仅使用 EMF 记录。当设置了 [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) 时，渲染图像时将解析 EMF+ 记录，否则仅解析 EMF 记录。默认值是 [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY)。对于依赖 .NET System.Drawing.Common 的框架，此设置将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```


指示当单元格字体与字符不兼容时是否仅替换该字符的字体。

**Remarks**

默认值为 false。我们将首先尝试 Workbook 的默认字体以及 PdfSaveOption/system 用于单元格字体。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```


设置网格线颜色。

**Remarks**

它将忽略源文件中的网格线颜色设置。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```


设置网格线类型。

参见 [GridlineType](../../com.aspose.cells/gridlinetype)。

**Remarks**

默认值为 Dotted 类型。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```


设置生成图像的水平分辨率，单位为每英寸点数。

**Remarks**

默认值为 96。设置  和  会影响输出图像的宽度和高度（单位：像素）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```


设置生成图像的格式。默认值：PNG。

参见 [ImageType](../../com.aspose.cells/imagetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


如果 OnePagePerSheet 为 true，则单个工作表的所有内容将仅输出到结果的一个页面。页面设置的纸张大小将失效，页面设置的其他设置仍然生效。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```


如果此属性为 true，则只输出一个区域，且不应用缩放。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```


指示是否优化输出元素。

**Remarks**

默认值为 false。目前当此属性设置为 true 时，将进行以下优化：1. 优化边框线。2. 在渲染为 Svg 图像时优化文件大小。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


指示在没有可打印内容时是否输出空白页。

**Remarks**

默认值为 false。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```


设置要保存的页数。

**Remarks**

默认值为 System.Int32.MaxValue，表示将渲染所有页面。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```


设置要保存的第一页的基于 0 的索引。

**Remarks**

默认值为 0。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```


控制/指示页面保存过程的进度。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```


如果 PrintWithStatusDialog = true，则会出现显示当前打印状态的对话框；否则不会显示此类对话框。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```


指示哪些页面将不会被打印。

参见 [PrintingPageType](../../com.aspose.cells/printingpagetype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```


设置一个值以确定生成图像的质量，仅在将页面保存为 `Jpeg` 格式时应用。默认值为 100。

**Remarks**

仅在保存为 JPEG 时生效。取值必须在 0 到 100 之间。默认值为 100。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```


为渲染算法设置单个偏好的值。提示类别包括对渲染质量以及渲染过程中的整体时间/质量权衡的控制。请参阅 RenderingHints 类以获取一些常用键和值的定义。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 键 | java.awt.RenderingHints.Key | 要设置的提示键。 |
| 值 | java.lang.Object | 指示指定提示类别偏好的值。 |

### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```


如果此属性为 true，生成的 svg 将适应视口。

**Remarks**

NOTE: 此成员现已过时。请改用 [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--)。此属性将在自 2025 年 4 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```


设置输出文件格式类型，支持 Tiff/XPS。

参见 [SaveFormat](../../com.aspose.cells/saveformat)。

**Remarks**

NOTE: 此成员现已过时。对于 Tiff/Svg，请使用 [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--)；对于 Xps，请使用带有 [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions) 的 [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-)。此属性将在自 2022 年 8 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


设置要渲染的工作表。默认是工作簿中所有可见工作表：[SheetSet.getVisible()](../../com.aspose.cells/sheetset\\#getVisible--)。

**Remarks**

当在 [SheetRender](../../com.aspose.cells/sheetrender) 中使用时，此设置将被忽略。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```


设置 svg 中 css 名称的前缀，默认值为空字符串。

**Remarks**

NOTE: 此成员现已过时。请改用 [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--)。此属性将在自 2025 年 4 月起的 12 个月后移除。Aspose 对您可能遇到的不便表示歉意。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


当文本宽度大于单元格宽度时，设置显示文本的类型。

请参阅 [TextCrossType](../../com.aspose.cells/textcrosstype)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```


设置位深度，仅在将页面保存为 `Tiff` 格式时应用。

参见 [ColorDepth](../../com.aspose.cells/colordepth)。

**Remarks**

仅在保存为 TIFF 时生效。如果 TiffCompression 设置为 CCITT3、CCITT4，则此设置不生效，生成的 tiff 图像的位深度始终为 1。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```


设置压缩类型，仅在将页面保存为 `Tiff` 格式时应用。

参见 [TiffCompression](../../com.aspose.cells/tiffcompression)。

**Remarks**

仅在保存为 TIFF 时生效。默认值为 Lzw。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```


设置光度解释类型，仅在将页面保存为 `Tiff` 格式时应用。

**Remarks**

仅在保存为 TIFF 时生效。默认值为 -1，表示未应用 PhotometricInterpretation。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```


指示生成图像的背景是否应为透明。

**Remarks**

默认值为 false。这意味着生成的图像背景为白色。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```


设置生成图像的垂直分辨率，单位为每英寸点数（dpi）。

**Remarks**

默认值为 96。设置  和  会影响输出图像的宽度和高度（单位：像素）。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```


设置警告回调。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

