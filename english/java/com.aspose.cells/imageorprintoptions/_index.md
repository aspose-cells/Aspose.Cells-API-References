---
title: ImageOrPrintOptions
second_title: Aspose.Cells for Java API Reference
description: Allows to specify options when rendering worksheet to images printing worksheet or rendering chart to image.
type: docs
weight: 273
url: /java/com.aspose.cells/imageorprintoptions/
---

**Inheritance:**
java.lang.Object
```
public class ImageOrPrintOptions
```

Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.

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
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. |
| [getChartImageType()](#getChartImageType--) | Indicate the chart imagetype when converting. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Gets or sets default edit language. |
| [getDefaultFont()](#getDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--) | Indicate the filename of embedded image in svg. |
| [getGridlineType()](#getGridlineType--) | Gets or sets gridline type. |
| [getHorizontalResolution()](#getHorizontalResolution--) | Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [getImageType()](#getImageType--) | Gets or sets the format of the generated images. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. |
| [getOnlyArea()](#getOnlyArea--) | If this property is true , one Area will be output, and no scale will take effect. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indicates whether to output a blank page when there is nothing to print. |
| [getPageCount()](#getPageCount--) | Gets or sets the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | Gets or sets the 0-based index of the first page to save. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Control/Indicate progress of page saving process. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. |
| [getPrintingPage()](#getPrintingPage--) | Indicates which pages will not be printed. |
| [getQuality()](#getQuality--) | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--) | if this property is true, the generated svg will fit to view port. |
| [getSaveFormat()](#getSaveFormat--) | Gets or sets the output file format type Support Tiff/XPS NOTE: This member is now obsolete. |
| [getSheetSet()](#getSheetSet--) | Gets or sets the sheets to render. |
| [getTextCrossType()](#getTextCrossType--) | Gets or sets displaying text type when the text width is larger than cell width. |
| [getTiffColorDepth()](#getTiffColorDepth--) | Gets or sets bit depth to apply only when saving pages to the Tiff format. |
| [getTiffCompression()](#getTiffCompression--) | Gets or sets the type of compression to apply only when saving pages to the Tiff format. |
| [getTransparent()](#getTransparent--) | Indicates if the background of generated image should be transparent. |
| [getVerticalResolution()](#getVerticalResolution--) | Gets or sets the vertical resolution for generated images, in dots per inch. |
| [getWarningCallback()](#getWarningCallback--) | Gets or sets warning callback. |
| [hashCode()](#hashCode--) |  |
| [isCellAutoFit()](#isCellAutoFit--) | Indicates whether the width and height of the cells is automatically fitted by cell value. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [isOptimized()](#isOptimized--) | Indicates whether to optimize the output elements. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) |  |
| [setCellAutoFit(boolean value)](#setCellAutoFit-boolean-) |  |
| [setChartImageType(ImageFormat value)](#setChartImageType-com.aspose.cells.ImageFormat-) |  |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) |  |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) |  |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) |  |
| [setDesiredSize(int desiredWidth, int desiredHeight)](#setDesiredSize-int-int-) | Sets desired width and height of image. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) |  |
| [setEmbededImageNameInSvg(String value)](#setEmbededImageNameInSvg-java.lang.String-) |  |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) |  |
| [setGridlineType(int value)](#setGridlineType-int-) |  |
| [setHorizontalResolution(int value)](#setHorizontalResolution-int-) |  |
| [setImageType(int value)](#setImageType-int-) |  |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) |  |
| [setOnlyArea(boolean value)](#setOnlyArea-boolean-) |  |
| [setOptimized(boolean value)](#setOptimized-boolean-) |  |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) |  |
| [setPageCount(int value)](#setPageCount-int-) |  |
| [setPageIndex(int value)](#setPageIndex-int-) |  |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) |  |
| [setPrintWithStatusDialog(boolean value)](#setPrintWithStatusDialog-boolean-) |  |
| [setPrintingPage(int value)](#setPrintingPage-int-) |  |
| [setQuality(int value)](#setQuality-int-) |  |
| [setRenderingHint(RenderingHints.Key key, Object value)](#setRenderingHint-java.awt.RenderingHints.Key-java.lang.Object-) | Sets the value of a single preference for the rendering algorithms. |
| [setSVGFitToViewPort(boolean value)](#setSVGFitToViewPort-boolean-) |  |
| [setSaveFormat(int value)](#setSaveFormat-int-) |  |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) |  |
| [setTextCrossType(int value)](#setTextCrossType-int-) |  |
| [setTiffColorDepth(int value)](#setTiffColorDepth-int-) |  |
| [setTiffCompression(int value)](#setTiffCompression-int-) |  |
| [setTransparent(boolean value)](#setTransparent-boolean-) |  |
| [setVerticalResolution(int value)](#setVerticalResolution-int-) |  |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


Indicate the chart imagetype when converting. default value: PNG. NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```
public boolean getCheckWorkbookDefaultFont()
```


When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. Default is true.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


Gets or sets default edit language. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO.

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
### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}
```
public String getEmbededImageNameInSvg()
```


Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\\\xpsEmbedded"

**Returns:**
java.lang.String
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


Gets or sets gridline type. Default is Dotted type.

**Returns:**
int
### getHorizontalResolution() {#getHorizontalResolution--}
```
public int getHorizontalResolution()
```


Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images. The default value is 96.

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Gets or sets the format of the generated images. default value: PNG.

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


Indicates whether to output a blank page when there is nothing to print. Default is false.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.

**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```


Gets or sets the 0-based index of the first page to save. Default is 0.

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

**Returns:**
int
### getQuality() {#getQuality--}
```
public int getQuality()
```


Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. The default value is 100 Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

**Returns:**
int
### getSVGFitToViewPort() {#getSVGFitToViewPort--}
```
public boolean getSVGFitToViewPort()
```


if this property is true, the generated svg will fit to view port.

**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```


Gets or sets the output file format type Support Tiff/XPS NOTE: This member is now obsolete. Instead, For Tiff/Svg, use [getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--); For Xps, use [Workbook.save(String,SaveOptions)](../../com.aspose.cells/workbook\#save-String-SaveOptions-) with [XpsSaveOptions](../../com.aspose.cells/xpssaveoptions). This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```


Gets or sets the sheets to render. Default is all visible sheets in the workbook: \{@link com.aspose.cells.SheetSet.getVisible()\}. The set is ignored when it is used in [SheetRender](../../com.aspose.cells/sheetrender)

**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```


Gets or sets displaying text type when the text width is larger than cell width.

**Returns:**
int
### getTiffColorDepth() {#getTiffColorDepth--}
```
public int getTiffColorDepth()
```


Gets or sets bit depth to apply only when saving pages to the Tiff format. Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

**Returns:**
int
### getTiffCompression() {#getTiffCompression--}
```
public int getTiffCompression()
```


Gets or sets the type of compression to apply only when saving pages to the Tiff format. Has effect only when saving to TIFF. The default value is Lzw.

**Returns:**
int
### getTransparent() {#getTransparent--}
```
public boolean getTransparent()
```


Indicates if the background of generated image should be transparent. The default value is false. That means the background of the generated images is white.

**Returns:**
boolean
### getVerticalResolution() {#getVerticalResolution--}
```
public int getVerticalResolution()
```


Gets or sets the vertical resolution for generated images, in dots per inch. Applies generating image method except Emf format image. The default value is 96.

**Returns:**
int
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


Gets or sets warning callback.

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


Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. NOTE: This member is now obsolete. Instead, please use [Worksheet.autoFitColumns(AutoFitterOptions)](../../com.aspose.cells/worksheet\#autoFitColumns-AutoFitterOptions-) and [Worksheet.autoFitRows(AutoFitterOptions)](../../com.aspose.cells/worksheet\#autoFitRows-AutoFitterOptions-). This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```


Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

**Returns:**
boolean
### isOptimized() {#isOptimized--}
```
public boolean isOptimized()
```


Indicates whether to optimize the output elements. Default value is false. Currently only the border lines are\\u807doptimized when this property is set to true.

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




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCellAutoFit(boolean value) {#setCellAutoFit-boolean-}
```
public void setCellAutoFit(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setChartImageType(ImageFormat value) {#setChartImageType-com.aspose.cells.ImageFormat-}
```
public void setChartImageType(ImageFormat value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDesiredSize(int desiredWidth, int desiredHeight) {#setDesiredSize-int-int-}
```
public void setDesiredSize(int desiredWidth, int desiredHeight)
```


Sets desired width and height of image.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | int | desired width in pixels |
| desiredHeight | int | desired height in pixels |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbededImageNameInSvg(String value) {#setEmbededImageNameInSvg-java.lang.String-}
```
public void setEmbededImageNameInSvg(String value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFontSubstitutionCharGranularity(boolean value) {#setFontSubstitutionCharGranularity-boolean-}
```
public void setFontSubstitutionCharGranularity(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setGridlineType(int value) {#setGridlineType-int-}
```
public void setGridlineType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHorizontalResolution(int value) {#setHorizontalResolution-int-}
```
public void setHorizontalResolution(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setImageType(int value) {#setImageType-int-}
```
public void setImageType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOnlyArea(boolean value) {#setOnlyArea-boolean-}
```
public void setOnlyArea(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOptimized(boolean value) {#setOptimized-boolean-}
```
public void setOptimized(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPageCount(int value) {#setPageCount-int-}
```
public void setPageCount(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPageIndex(int value) {#setPageIndex-int-}
```
public void setPageIndex(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-}
```
public void setPageSavingCallback(IPageSavingCallback value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPrintWithStatusDialog(boolean value) {#setPrintWithStatusDialog-boolean-}
```
public void setPrintWithStatusDialog(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPrintingPage(int value) {#setPrintingPage-int-}
```
public void setPrintingPage(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setQuality(int value) {#setQuality-int-}
```
public void setQuality(int value)
```




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




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSaveFormat(int value) {#setSaveFormat-int-}
```
public void setSaveFormat(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTiffColorDepth(int value) {#setTiffColorDepth-int-}
```
public void setTiffColorDepth(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTiffCompression(int value) {#setTiffCompression-int-}
```
public void setTiffCompression(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTransparent(boolean value) {#setTransparent-boolean-}
```
public void setTransparent(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setVerticalResolution(int value) {#setVerticalResolution-int-}
```
public void setVerticalResolution(int value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```




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
