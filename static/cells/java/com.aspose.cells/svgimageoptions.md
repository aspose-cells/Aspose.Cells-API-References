##SvgImageOptions
Options for generating Svg image.
**Inheritance:**
java.lang.Object, [com.aspose.cells.ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions)
```
public class SvgImageOptions extends ImageOrPrintOptions
```
Options for generating Svg image.
## Constructors
| Constructor | Description |
| --- | --- |
| [SvgImageOptions()](#SvgImageOptions--) | Ctor. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. |
| [getChartImageType()](#getChartImageType--) | Indicate the chart imagetype when converting. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getClass()](#getClass--) |  |
| [getCssPrefix()](#getCssPrefix--) | Gets the prefix of the css name in svg,the default value is empty string. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Gets custom settings during rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Gets default edit language. |
| [getDefaultFont()](#getDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbeddedFontType()](#getEmbeddedFontType--) | Gets the type of font that embedded in Svg. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Indicate the filename of embedded image in svg. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Setting for rendering Emf metafiles in source file. |
| [getFitToViewPort()](#getFitToViewPort--) | if this property is true, the generated svg will fit to view port. |
| [getGridlineColor()](#getGridlineColor--) | Gets gridline colr. |
| [getGridlineType()](#getGridlineType--) | Gets gridline type. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Gets the horizontal resolution for generated images, in dots per inch. |
| [getImageType()](#getImageType--) | Gets the format of the generated images. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. |
| [getOnlyArea()](#getOnlyArea--) | If this property is true , one Area will be output, and no scale will take effect. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indicates whether to output a blank page when there is nothing to print. |
| [getPageCount()](#getPageCount--) | Gets the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | Gets the 0-based index of the first page to save. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Control/Indicate progress of page saving process. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. |
| [getPrintingPage()](#getPrintingPage--) | Indicates which pages will not be printed. |
| [getQuality()](#getQuality--) | Gets a value determining the quality of the generated images to apply only when saving pages to the `Jpeg` format. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | if this property is true, the generated svg will fit to view port. |
| [getSaveFormat()](#getSaveFormat--) | Gets the output file format type Support Tiff/XPS |
| [getSheetSet()](#getSheetSet--) | Gets the sheets to render. |
| [getSvgCssPrefix()](#getSvgCssPrefix--) | Gets the prefix of the css name in svg,the default value is empty string. |
| [getTextCrossType()](#getTextCrossType--) | Gets displaying text type when the text width is larger than cell width. |
| [getTiffColorDepth()](#getTiffColorDepth--) | Gets bit depth to apply only when saving pages to the `Tiff` format. |
| [getTiffCompression()](#getTiffCompression--) | Gets the type of compression to apply only when saving pages to the `Tiff` format. |
| [getTiffPhotometricInterpretation()](#getTiffPhotometricInterpretation--) | Gets the type of PhotometricInterpretation to apply only when saving pages to the `Tiff` format. |
| [getTransparent()](#getTransparent--) | Indicates if the background of generated image should be transparent. |
| [getVerticalResolution()](#getVerticalResolution--) | Gets the vertical resolution for generated images, in dots per inch. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Indicates whether the width and height of the cells is automatically fitted by cell value. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [isOptimized()](#isOptimized--) | Indicates whether to optimize the output elements. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) | Indicates whether the width and height of the cells is automatically fitted by cell value. |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) | Indicate the chart imagetype when converting. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [setCssPrefix(String value)](#setCssPrefix-java.lang.String-) | Sets the prefix of the css name in svg,the default value is empty string. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Sets custom settings during rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Sets default edit language. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Sets desired width and height of image. |
| [setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)](#setDesiredSize-int-int-boolean-) | Sets desired width and height of image. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implements this interface to get DrawObject and Bound when rendering. |
| [setEmbeddedFontType(int value)](#setEmbeddedFontType-int-) | Sets the type of font that embedded in Svg. |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) | Indicate the filename of embedded image in svg. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Setting for rendering Emf metafiles in source file. |
| [setFitToViewPort(boolean value)](#setFitToViewPort-boolean-) | if this property is true, the generated svg will fit to view port. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Sets gridline colr. |
| [setGridlineType(int value)](#setGridlineType-int-) | Sets gridline type. |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) | Sets the horizontal resolution for generated images, in dots per inch. |
| [setImageType(int value)](#setImageType-int-) | Sets the format of the generated images. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) | If this property is true , one Area will be output, and no scale will take effect. |
| [setOptimized(boolean value)](#setOptimized-boolean-) | Indicates whether to optimize the output elements. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indicates whether to output a blank page when there is nothing to print. |
| [setPageCount(int value)](#setPageCount-int-) | Sets the number of pages to save. |
| [setPageIndex(int value)](#setPageIndex-int-) | Sets the 0-based index of the first page to save. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Control/Indicate progress of page saving process. |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. |
| [setPrintingPage(int value)](#setPrintingPage-int-) | Indicates which pages will not be printed. |
| [setQuality(int value)](#setQuality-int-) | Sets a value determining the quality of the generated images to apply only when saving pages to the `Jpeg` format. |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Sets the value of a single preference for the rendering algorithms. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) | if this property is true, the generated svg will fit to view port. |
| [setSaveFormat(int value)](#setSaveFormat-int-) | Sets the output file format type Support Tiff/XPS |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Sets the sheets to render. |
| [setSvgCssPrefix(String value)](#setSvgCssPrefix-java.lang.String-) | Sets the prefix of the css name in svg,the default value is empty string. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Sets displaying text type when the text width is larger than cell width. |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) | Sets bit depth to apply only when saving pages to the `Tiff` format. |
| [setTiffCompression(int value)](#setTiffCompression-int-) | Sets the type of compression to apply only when saving pages to the `Tiff` format. |
| [setTiffPhotometricInterpretation(int value)](#setTiffPhotometricInterpretation-int-) | Sets the type of PhotometricInterpretation to apply only when saving pages to the `Tiff` format. |
| [setTransparent(boolean value)](#setTransparent-boolean-) | Indicates if the background of generated image should be transparent. |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) | Sets the vertical resolution for generated images, in dots per inch. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### SvgImageOptions() {#SvgImageOptions--}
```
public SvgImageOptions()
```
Ctor.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |
**Returns:**
boolean
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```
public boolean getAllColumnsInOnePagePerSheet()
```
If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
**Returns:**
boolean
### getChartImageType() {#getChartImageType--}
```
public ImageFormat getChartImageType()
```
Indicate the chart imagetype when converting. default value: PNG.
**Remarks**
NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.
**Remarks**
Default is true.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCssPrefix() {#getCssPrefix--}
```
public String getCssPrefix()
```
Gets the prefix of the css name in svg,the default value is empty string.
**Returns:**
java.lang.String
### getCustomRenderSettings() {#getCustomRenderSettings--}
```
public CustomRenderSettings getCustomRenderSettings()
```
Gets custom settings during rendering.
**Returns:**
[CustomRenderSettings](../../com.aspose.cells/customrendersettings)
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```
Gets default edit language.
See [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).
**Returns:**
int
### getDefaultFont() {#getDefaultFont--}
```
public String getDefaultFont()
```
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.
**Returns:**
java.lang.String
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```
Implements this interface to get DrawObject and Bound when rendering.
**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbeddedFontType() {#getEmbeddedFontType--}
```
public int getEmbeddedFontType()
```
Gets the type of font that embedded in Svg.
See [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).
**Remarks**
Default value is [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE) which indicates that it will not embed font in Svg.
**Returns:**
int
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```
Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\\\xpsEmbedded"
**Remarks**
NOTE: This member is now obsolete. Instead, please remove this property because images are now always embedded in Svg with base64 format. This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
java.lang.String
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```
Setting for rendering Emf metafiles in source file.
See [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).
**Remarks**
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.
**Returns:**
int
### getFitToViewPort() {#getFitToViewPort--}
```
public boolean getFitToViewPort()
```
if this property is true, the generated svg will fit to view port.
**Returns:**
boolean
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```
Gets gridline colr.
**Remarks**
It will ignore the gridline color settings in the source file.
**Returns:**
[Color](../../com.aspose.cells/color)
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```
Gets gridline type.
See [GridlineType](../../com.aspose.cells/gridlinetype).
**Remarks**
Default is Dotted type.
**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```
Gets the horizontal resolution for generated images, in dots per inch.
**Remarks**
The default value is 96. Setting  and  effects the width and height of the output image in pixels.
**Example**
The following code sets resolution to 192, the width and height of the generated image is twice of the one with resolution left as the default value 96.
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
Gets the format of the generated images. default value: PNG.
See [ImageType](../../com.aspose.cells/imagetype).
**Returns:**
int
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```
If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
**Returns:**
boolean
### getOnlyArea() {#getOnlyArea--}
```
public boolean getOnlyArea()
```
If this property is true , one Area will be output, and no scale will take effect.
**Returns:**
boolean
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```
Indicates whether to output a blank page when there is nothing to print.
**Remarks**
Default is false.
**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```
Gets the number of pages to save.
**Remarks**
Default is System.Int32.MaxValue which means all pages will be rendered.
**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```
Gets the 0-based index of the first page to save.
**Remarks**
Default is 0.
**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```
Control/Indicate progress of page saving process.
**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}
```
public boolean getPrintWithStatusDialog()
```
If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.
**Returns:**
boolean
### getPrintingPage() {#getPrintingPage--}
```
public int getPrintingPage()
```
Indicates which pages will not be printed.
See [PrintingPageType](../../com.aspose.cells/printingpagetype).
**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```
Gets a value determining the quality of the generated images to apply only when saving pages to the `Jpeg` format. The default value is 100
**Remarks**
Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.
**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```
if this property is true, the generated svg will fit to view port.
**Remarks**
NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```
Gets the output file format type Support Tiff/XPS
See [SaveFormat](../../com.aspose.cells/saveformat).
**Remarks**
NOTE: This member is now obsolete. Instead, For Tiff/Svg, use [ImageType](../../com.aspose.cells/imagetype); For Xps, use [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) with [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```
Gets the sheets to render. Default is all visible sheets in the workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).
**Remarks**
The set is ignored when it is used in [SheetRender](../../com.aspose.cells/sheetrender)
**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSvgCssPrefix() {#getSvgCssPrefix--}
```
public String getSvgCssPrefix()
```
Gets the prefix of the css name in svg,the default value is empty string.
**Remarks**
NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
java.lang.String
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```
Gets displaying text type when the text width is larger than cell width.
See [TextCrossType](../../com.aspose.cells/textcrosstype).
**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```
Gets bit depth to apply only when saving pages to the `Tiff` format.
See [ColorDepth](../../com.aspose.cells/colordepth).
**Remarks**
Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.
**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```
Gets the type of compression to apply only when saving pages to the `Tiff` format.
See [TiffCompression](../../com.aspose.cells/tiffcompression).
**Remarks**
Has effect only when saving to TIFF. The default value is Lzw.
**Returns:**
int
### getTiffPhotometricInterpretation() {#getTiffPhotometricInterpretation--}
```
public int getTiffPhotometricInterpretation()
```
Gets the type of PhotometricInterpretation to apply only when saving pages to the `Tiff` format.
**Remarks**
Has effect only when saving to TIFF. The default value is -1, represent no PhotometricInterpretation is applied.
**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```
Indicates if the background of generated image should be transparent.
**Remarks**
The default value is false. That means the background of the generated images is white.
**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```
Gets the vertical resolution for generated images, in dots per inch.
**Remarks**
The default value is 96. Setting  and  effects the width and height of the output image in pixels.
**Example**
The following code sets resolution to 192, the width and height of the generated image is twice of the one with resolution left as the default value 96.
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
Gets warning callback.
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
Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false.
**Remarks**
NOTE: This member is now obsolete. Instead, this property is not used, please remove this property.. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```
Indicates whether to only substitute the font of character when the cell font is not compatibility for it.
**Remarks**
Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.
**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```
Indicates whether to optimize the output elements.
**Remarks**
Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.
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
If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```
Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false.
**Remarks**
NOTE: This member is now obsolete. Instead, this property is not used, please remove this property.. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```
Indicate the chart imagetype when converting. default value: PNG.
**Remarks**
NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |
### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.
**Remarks**
Default is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCssPrefix(String value) {#setCssPrefix-java.lang.String-}
```
public void setCssPrefix(String value)
```
Sets the prefix of the css name in svg,the default value is empty string.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCustomRenderSettings(CustomRenderSettings value) {#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-}
```
public void setCustomRenderSettings(CustomRenderSettings value)
```
Sets custom settings during rendering.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomRenderSettings](../../com.aspose.cells/customrendersettings) |  |
### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```
Sets default edit language.
See [DefaultEditLanguage](../../com.aspose.cells/defaulteditlanguage).
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [DefaultEditLanguage.AUTO](../../com.aspose.cells/defaulteditlanguage\#AUTO).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```
When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```
Sets desired width and height of image.
**Remarks**
NOTE: This member is now obsolete. Instead, please use [setDesiredSize(int,int,boolean)](../../com.aspose.cells/imageorprintoptions\#setDesiredSize-int-int-boolean-) by setting param keepAspectRatio to false. This property will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | int | desired width in pixels |
| desiredHeight | int | desired height in pixels |
### setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio) {#setDesiredSize-int-int-boolean-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight, boolean keepAspectRatio)
```
Sets desired width and height of image.
**Remarks**
The width and height of the output image in pixels will be only based on the set desired width and height. The  and  will not effect the width and height of the output image in this case.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | int | desired width in pixels |
| desiredHeight | int | desired height in pixels |
| keepAspectRatio | boolean | whether to keep aspect ratio of origin image |
### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```
Implements this interface to get DrawObject and Bound when rendering.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |
### setEmbeddedFontType(int value) {#setEmbeddedFontType-int-}
```
public void setEmbeddedFontType(int value)
```
Sets the type of font that embedded in Svg.
See [SvgEmbeddedFontType](../../com.aspose.cells/svgembeddedfonttype).
**Remarks**
Default value is [SvgEmbeddedFontType.NONE](../../com.aspose.cells/svgembeddedfonttype\#NONE) which indicates that it will not embed font in Svg.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```
Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\\\xpsEmbedded"
**Remarks**
NOTE: This member is now obsolete. Instead, please remove this property because images are now always embedded in Svg with base64 format. This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```
Setting for rendering Emf metafiles in source file.
See [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).
**Remarks**
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setFitToViewPort(boolean value) {#setFitToViewPort-boolean-}
```
public void setFitToViewPort(boolean value)
```
if this property is true, the generated svg will fit to view port.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```
Indicates whether to only substitute the font of character when the cell font is not compatibility for it.
**Remarks**
Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setGridlineColor(Color value) {#setGridlineColor-com.aspose.cells.Color-}
```
public void setGridlineColor(Color value)
```
Sets gridline colr.
**Remarks**
It will ignore the gridline color settings in the source file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```
Sets gridline type.
See [GridlineType](../../com.aspose.cells/gridlinetype).
**Remarks**
Default is Dotted type.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```
Sets the horizontal resolution for generated images, in dots per inch.
**Remarks**
The default value is 96. Setting  and  effects the width and height of the output image in pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```
Sets the format of the generated images. default value: PNG.
See [ImageType](../../com.aspose.cells/imagetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```
If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```
If this property is true , one Area will be output, and no scale will take effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```
Indicates whether to optimize the output elements.
**Remarks**
Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```
Indicates whether to output a blank page when there is nothing to print.
**Remarks**
Default is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```
Sets the number of pages to save.
**Remarks**
Default is System.Int32.MaxValue which means all pages will be rendered.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```
Sets the 0-based index of the first page to save.
**Remarks**
Default is 0.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```
Control/Indicate progress of page saving process.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |
### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```
If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```
Indicates which pages will not be printed.
See [PrintingPageType](../../com.aspose.cells/printingpagetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```
Sets a value determining the quality of the generated images to apply only when saving pages to the `Jpeg` format. The default value is 100
**Remarks**
Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRenderingHint(RenderingHints.Key key, Object value) {#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-}
```
public void setRenderingHint(RenderingHints.Key key, Object value)
```
Sets the value of a single preference for the rendering algorithms. Hint categories include controls for rendering quality and overall time/quality trade-off in the rendering process. Refer to the RenderingHints class for definitions of some common keys and values.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | java.awt.RenderingHints.Key | the key of the hint to be set. |
| value | java.lang.Object | the value indicating preferences for the specified hint category. |
### setSVGFitToViewPort(boolean value) {#setSVGFitToViewPort-boolean-}
```
public void setSVGFitToViewPort(boolean value)
```
if this property is true, the generated svg will fit to view port.
**Remarks**
NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.getFitToViewPort()](../../com.aspose.cells/svgimageoptions\#getFitToViewPort--). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```
Sets the output file format type Support Tiff/XPS
See [SaveFormat](../../com.aspose.cells/saveformat).
**Remarks**
NOTE: This member is now obsolete. Instead, For Tiff/Svg, use [ImageType](../../com.aspose.cells/imagetype); For Xps, use [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) with [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```
Sets the sheets to render. Default is all visible sheets in the workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).
**Remarks**
The set is ignored when it is used in [SheetRender](../../com.aspose.cells/sheetrender)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |
### setSvgCssPrefix(String value) {#setSvgCssPrefix-java.lang.String-}
```
public void setSvgCssPrefix(String value)
```
Sets the prefix of the css name in svg,the default value is empty string.
**Remarks**
NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.getCssPrefix()](../../com.aspose.cells/svgimageoptions\#getCssPrefix--). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```
Sets displaying text type when the text width is larger than cell width.
See [TextCrossType](../../com.aspose.cells/textcrosstype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```
Sets bit depth to apply only when saving pages to the `Tiff` format.
See [ColorDepth](../../com.aspose.cells/colordepth).
**Remarks**
Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```
Sets the type of compression to apply only when saving pages to the `Tiff` format.
See [TiffCompression](../../com.aspose.cells/tiffcompression).
**Remarks**
Has effect only when saving to TIFF. The default value is Lzw.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTiffPhotometricInterpretation(int value) {#setTiffPhotometricInterpretation-int-}
```
public void setTiffPhotometricInterpretation(int value)
```
Sets the type of PhotometricInterpretation to apply only when saving pages to the `Tiff` format.
**Remarks**
Has effect only when saving to TIFF. The default value is -1, represent no PhotometricInterpretation is applied.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```
Indicates if the background of generated image should be transparent.
**Remarks**
The default value is false. That means the background of the generated images is white.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```
Sets the vertical resolution for generated images, in dots per inch.
**Remarks**
The default value is 96. Setting  and  effects the width and height of the output image in pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```
Sets warning callback.
**Parameters:**
| Parameter | Type | Description |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |
