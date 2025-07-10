﻿---
title: ImageOrPrintOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Allows to specify options when rendering worksheet to images printing worksheet or rendering chart to image.
type: docs
url: /nodejs-cpp/imageorprintoptions/
---

## ImageOrPrintOptions class

Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.

```javascript
class ImageOrPrintOptions;
```


### Example
```javascript
const { Workbook, ImageOrPrintOptions } = require("aspose.cells.node");

//Set Image Or Print Options
var options = new ImageOrPrintOptions();
//set Horizontal resolution
options.horizontalResolution = 200;
//set Vertica; Resolution
options.verticalResolution = 300;

//Instantiate Workbook
var book = new Workbook("input/Chart.xls");
//Save chart as Image using ImageOrPrint Options
book.worksheets.get(0).charts.get(0).toImage("output/chart.png", options);
```
## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Ctor. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [printWithStatusDialog](#printWithStatusDialog--)| boolean | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [horizontalResolution](#horizontalResolution--)| number | Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [verticalResolution](#verticalResolution--)| number | Gets or sets the vertical resolution for generated images, in dots per inch. |
| [tiffCompression](#tiffCompression--)| TiffCompression | Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format. |
| [tiffColorDepth](#tiffColorDepth--)| ColorDepth | Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format. |
| [tiffBinarizationMethod](#tiffBinarizationMethod--)| ImageBinarizationMethod | Gets or sets method used while converting images to 1 bpp format when [ImageType](../imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [printingPage](#printingPage--)| PrintingPageType | Indicates which pages will not be printed. |
| [quality](#quality--)| number | Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100 |
| [onePagePerSheet](#onePagePerSheet--)| boolean | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [allColumnsInOnePagePerSheet](#allColumnsInOnePagePerSheet--)| boolean | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [drawObjectEventHandler](#drawObjectEventHandler--)| DrawObjectEventHandler | Implements this interface to get DrawObject and Bound when rendering. |
| [embededImageNameInSvg](#embededImageNameInSvg--)| string | Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [sVGFitToViewPort](#sVGFitToViewPort--)| boolean | if this property is true, the generated svg will fit to view port. |
| [svgCssPrefix](#svgCssPrefix--)| string | Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [onlyArea](#onlyArea--)| boolean | If this property is true , one Area will be output, and no scale will take effect. |
| [transparent](#transparent--)| boolean | Indicates if the background of generated image should be transparent. |
| [warningCallback](#warningCallback--)| IWarningCallback | Gets or sets warning callback. |
| [pageSavingCallback](#pageSavingCallback--)| IPageSavingCallback | Control/Indicate progress of page saving process. |
| [isFontSubstitutionCharGranularity](#isFontSubstitutionCharGranularity--)| boolean | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [pageIndex](#pageIndex--)| number | Gets or sets the 0-based index of the first page to save. |
| [pageCount](#pageCount--)| number | Gets or sets the number of pages to save. |
| [isOptimized](#isOptimized--)| boolean | Indicates whether to optimize the output elements. |
| [defaultFont](#defaultFont--)| string | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [checkWorkbookDefaultFont](#checkWorkbookDefaultFont--)| boolean | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [outputBlankPageWhenNothingToPrint](#outputBlankPageWhenNothingToPrint--)| boolean | Indicates whether to output a blank page when there is nothing to print. |
| [gridlineType](#gridlineType--)| GridlineType | Gets or sets gridline type. |
| [gridlineColor](#gridlineColor--)| Color | Gets or sets gridline colr. |
| [textCrossType](#textCrossType--)| TextCrossType | Gets or sets displaying text type when the text width is larger than cell width. |
| [defaultEditLanguage](#defaultEditLanguage--)| DefaultEditLanguage | Gets or sets default edit language. |
| [sheetSet](#sheetSet--)| SheetSet | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [emfRenderSetting](#emfRenderSetting--)| EmfRenderSetting | Setting for rendering Emf metafiles in source file. |
| [customRenderSettings](#customRenderSettings--)| CustomRenderSettings | Gets or sets custom settings during rendering. |

## Methods

| Method | Description |
| --- | --- |
| [setPrintWithStatusDialog(boolean)](#setPrintWithStatusDialog-boolean-)| <b>@deprecated.</b> Please use the 'printWithStatusDialog' property instead. If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [getPrintWithStatusDialog()](#getPrintWithStatusDialog--)| <b>@deprecated.</b> Please use the 'printWithStatusDialog' property instead. If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [getHorizontalResolution()](#getHorizontalResolution--)| <b>@deprecated.</b> Please use the 'horizontalResolution' property instead. Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [setHorizontalResolution(number)](#setHorizontalResolution-number-)| <b>@deprecated.</b> Please use the 'horizontalResolution' property instead. Gets or sets the horizontal resolution for generated images, in dots per inch. |
| [getVerticalResolution()](#getVerticalResolution--)| <b>@deprecated.</b> Please use the 'verticalResolution' property instead. Gets or sets the vertical resolution for generated images, in dots per inch. |
| [setVerticalResolution(number)](#setVerticalResolution-number-)| <b>@deprecated.</b> Please use the 'verticalResolution' property instead. Gets or sets the vertical resolution for generated images, in dots per inch. |
| [getTiffCompression()](#getTiffCompression--)| <b>@deprecated.</b> Please use the 'tiffCompression' property instead. Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format. |
| [setTiffCompression(TiffCompression)](#setTiffCompression-tiffcompression-)| <b>@deprecated.</b> Please use the 'tiffCompression' property instead. Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format. |
| [getTiffColorDepth()](#getTiffColorDepth--)| <b>@deprecated.</b> Please use the 'tiffColorDepth' property instead. Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format. |
| [setTiffColorDepth(ColorDepth)](#setTiffColorDepth-colordepth-)| <b>@deprecated.</b> Please use the 'tiffColorDepth' property instead. Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format. |
| [getTiffBinarizationMethod()](#getTiffBinarizationMethod--)| <b>@deprecated.</b> Please use the 'tiffBinarizationMethod' property instead. Gets or sets method used while converting images to 1 bpp format when [ImageType](../imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [setTiffBinarizationMethod(ImageBinarizationMethod)](#setTiffBinarizationMethod-imagebinarizationmethod-)| <b>@deprecated.</b> Please use the 'tiffBinarizationMethod' property instead. Gets or sets method used while converting images to 1 bpp format when [ImageType](../imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4. |
| [getPrintingPage()](#getPrintingPage--)| <b>@deprecated.</b> Please use the 'printingPage' property instead. Indicates which pages will not be printed. |
| [setPrintingPage(PrintingPageType)](#setPrintingPage-printingpagetype-)| <b>@deprecated.</b> Please use the 'printingPage' property instead. Indicates which pages will not be printed. |
| [getQuality()](#getQuality--)| <b>@deprecated.</b> Please use the 'quality' property instead. Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100 |
| [setQuality(number)](#setQuality-number-)| <b>@deprecated.</b> Please use the 'quality' property instead. Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100 |
| [getOnePagePerSheet()](#getOnePagePerSheet--)| <b>@deprecated.</b> Please use the 'onePagePerSheet' property instead. If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [setOnePagePerSheet(boolean)](#setOnePagePerSheet-boolean-)| <b>@deprecated.</b> Please use the 'onePagePerSheet' property instead. If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--)| <b>@deprecated.</b> Please use the 'allColumnsInOnePagePerSheet' property instead. If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [setAllColumnsInOnePagePerSheet(boolean)](#setAllColumnsInOnePagePerSheet-boolean-)| <b>@deprecated.</b> Please use the 'allColumnsInOnePagePerSheet' property instead. If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--)| <b>@deprecated.</b> Please use the 'drawObjectEventHandler' property instead. Implements this interface to get DrawObject and Bound when rendering. |
| [setDrawObjectEventHandler(DrawObjectEventHandler)](#setDrawObjectEventHandler-drawobjecteventhandler-)| <b>@deprecated.</b> Please use the 'drawObjectEventHandler' property instead. Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbededImageNameInSvg()](#getEmbededImageNameInSvg--)| <b>@deprecated.</b> Please use the 'embededImageNameInSvg' property instead. Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [setEmbededImageNameInSvg(string)](#setEmbededImageNameInSvg-string-)| <b>@deprecated.</b> Please use the 'embededImageNameInSvg' property instead. Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [getSVGFitToViewPort()](#getSVGFitToViewPort--)| <b>@deprecated.</b> Please use the 'sVGFitToViewPort' property instead. if this property is true, the generated svg will fit to view port. |
| [setSVGFitToViewPort(boolean)](#setSVGFitToViewPort-boolean-)| <b>@deprecated.</b> Please use the 'sVGFitToViewPort' property instead. if this property is true, the generated svg will fit to view port. |
| [getSvgCssPrefix()](#getSvgCssPrefix--)| <b>@deprecated.</b> Please use the 'svgCssPrefix' property instead. Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [setSvgCssPrefix(string)](#setSvgCssPrefix-string-)| <b>@deprecated.</b> Please use the 'svgCssPrefix' property instead. Gets and sets the prefix of the css name in svg,the default value is empty string. |
| [getOnlyArea()](#getOnlyArea--)| <b>@deprecated.</b> Please use the 'onlyArea' property instead. If this property is true , one Area will be output, and no scale will take effect. |
| [setOnlyArea(boolean)](#setOnlyArea-boolean-)| <b>@deprecated.</b> Please use the 'onlyArea' property instead. If this property is true , one Area will be output, and no scale will take effect. |
| [getTransparent()](#getTransparent--)| <b>@deprecated.</b> Please use the 'transparent' property instead. Indicates if the background of generated image should be transparent. |
| [setTransparent(boolean)](#setTransparent-boolean-)| <b>@deprecated.</b> Please use the 'transparent' property instead. Indicates if the background of generated image should be transparent. |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getPageSavingCallback()](#getPageSavingCallback--)| <b>@deprecated.</b> Please use the 'pageSavingCallback' property instead. Control/Indicate progress of page saving process. |
| [setPageSavingCallback(IPageSavingCallback)](#setPageSavingCallback-ipagesavingcallback-)| <b>@deprecated.</b> Please use the 'pageSavingCallback' property instead. Control/Indicate progress of page saving process. |
| [setIsFontSubstitutionCharGranularity(boolean)](#setIsFontSubstitutionCharGranularity-boolean-)| <b>@deprecated.</b> Please use the 'isFontSubstitutionCharGranularity' property instead. Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--)| <b>@deprecated.</b> Please use the 'isFontSubstitutionCharGranularity' property instead. Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [setPageIndex(number)](#setPageIndex-number-)| <b>@deprecated.</b> Please use the 'pageIndex' property instead. Gets or sets the 0-based index of the first page to save. |
| [getPageIndex()](#getPageIndex--)| <b>@deprecated.</b> Please use the 'pageIndex' property instead. Gets or sets the 0-based index of the first page to save. |
| [setPageCount(number)](#setPageCount-number-)| <b>@deprecated.</b> Please use the 'pageCount' property instead. Gets or sets the number of pages to save. |
| [getPageCount()](#getPageCount--)| <b>@deprecated.</b> Please use the 'pageCount' property instead. Gets or sets the number of pages to save. |
| [isOptimized()](#isOptimized--)| <b>@deprecated.</b> Please use the 'isOptimized' property instead. Indicates whether to optimize the output elements. |
| [setIsOptimized(boolean)](#setIsOptimized-boolean-)| <b>@deprecated.</b> Please use the 'isOptimized' property instead. Indicates whether to optimize the output elements. |
| [getDefaultFont()](#getDefaultFont--)| <b>@deprecated.</b> Please use the 'defaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [setDefaultFont(string)](#setDefaultFont-string-)| <b>@deprecated.</b> Please use the 'defaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--)| <b>@deprecated.</b> Please use the 'checkWorkbookDefaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [setCheckWorkbookDefaultFont(boolean)](#setCheckWorkbookDefaultFont-boolean-)| <b>@deprecated.</b> Please use the 'checkWorkbookDefaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--)| <b>@deprecated.</b> Please use the 'outputBlankPageWhenNothingToPrint' property instead. Indicates whether to output a blank page when there is nothing to print. |
| [setOutputBlankPageWhenNothingToPrint(boolean)](#setOutputBlankPageWhenNothingToPrint-boolean-)| <b>@deprecated.</b> Please use the 'outputBlankPageWhenNothingToPrint' property instead. Indicates whether to output a blank page when there is nothing to print. |
| [getGridlineType()](#getGridlineType--)| <b>@deprecated.</b> Please use the 'gridlineType' property instead. Gets or sets gridline type. |
| [setGridlineType(GridlineType)](#setGridlineType-gridlinetype-)| <b>@deprecated.</b> Please use the 'gridlineType' property instead. Gets or sets gridline type. |
| [getGridlineColor()](#getGridlineColor--)| <b>@deprecated.</b> Please use the 'gridlineColor' property instead. Gets or sets gridline colr. |
| [setGridlineColor(Color)](#setGridlineColor-color-)| <b>@deprecated.</b> Please use the 'gridlineColor' property instead. Gets or sets gridline colr. |
| [getTextCrossType()](#getTextCrossType--)| <b>@deprecated.</b> Please use the 'textCrossType' property instead. Gets or sets displaying text type when the text width is larger than cell width. |
| [setTextCrossType(TextCrossType)](#setTextCrossType-textcrosstype-)| <b>@deprecated.</b> Please use the 'textCrossType' property instead. Gets or sets displaying text type when the text width is larger than cell width. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--)| <b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language. |
| [setDefaultEditLanguage(DefaultEditLanguage)](#setDefaultEditLanguage-defaulteditlanguage-)| <b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language. |
| [getSheetSet()](#getSheetSet--)| <b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [setSheetSet(SheetSet)](#setSheetSet-sheetset-)| <b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [getEmfRenderSetting()](#getEmfRenderSetting--)| <b>@deprecated.</b> Please use the 'emfRenderSetting' property instead. Setting for rendering Emf metafiles in source file. |
| [setEmfRenderSetting(EmfRenderSetting)](#setEmfRenderSetting-emfrendersetting-)| <b>@deprecated.</b> Please use the 'emfRenderSetting' property instead. Setting for rendering Emf metafiles in source file. |
| [getCustomRenderSettings()](#getCustomRenderSettings--)| <b>@deprecated.</b> Please use the 'customRenderSettings' property instead. Gets or sets custom settings during rendering. |
| [setCustomRenderSettings(CustomRenderSettings)](#setCustomRenderSettings-customrendersettings-)| <b>@deprecated.</b> Please use the 'customRenderSettings' property instead. Gets or sets custom settings during rendering. |
| [setDesiredSize(number, number, boolean)](#setDesiredSize-number-number-boolean-)| Sets desired width and height of image. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getImageType()](#getImageType--)| Gets or sets the format of the generated images. default value: PNG. |
| [setImageType(ImageType)](#setImageType-imagetype-)| Gets or sets the format of the generated images. default value: PNG. |


### constructor() {#constructor--}

Ctor.

```javascript
constructor();
```


### printWithStatusDialog {#printWithStatusDialog--}

If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.

```javascript
printWithStatusDialog : boolean;
```


### horizontalResolution {#horizontalResolution--}

Gets or sets the horizontal resolution for generated images, in dots per inch.

```javascript
horizontalResolution : number;
```


**Remarks**

ara>The default value is 96.</para> <para>Setting [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) effects the width and height of the output image in pixels.</para

### verticalResolution {#verticalResolution--}

Gets or sets the vertical resolution for generated images, in dots per inch.

```javascript
verticalResolution : number;
```


**Remarks**

ara>The default value is 96.</para> <para>Setting [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) effects the width and height of the output image in pixels.</para

### tiffCompression {#tiffCompression--}

Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format.

```javascript
tiffCompression : TiffCompression;
```


**Remarks**

Has effect only when saving to TIFF. The default value is Lzw.

### tiffColorDepth {#tiffColorDepth--}

Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format.

```javascript
tiffColorDepth : ColorDepth;
```


**Remarks**

Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

### tiffBinarizationMethod {#tiffBinarizationMethod--}

Gets or sets method used while converting images to 1 bpp format when [ImageType](../imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4.

```javascript
tiffBinarizationMethod : ImageBinarizationMethod;
```


**Remarks**

The default value is FloydSteinbergDithering.

### printingPage {#printingPage--}

Indicates which pages will not be printed.

```javascript
printingPage : PrintingPageType;
```


### quality {#quality--}

Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100

```javascript
quality : number;
```


**Remarks**

Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

### onePagePerSheet {#onePagePerSheet--}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
onePagePerSheet : boolean;
```


### allColumnsInOnePagePerSheet {#allColumnsInOnePagePerSheet--}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
allColumnsInOnePagePerSheet : boolean;
```


### drawObjectEventHandler {#drawObjectEventHandler--}

Implements this interface to get DrawObject and Bound when rendering.

```javascript
drawObjectEventHandler : DrawObjectEventHandler;
```


### embededImageNameInSvg {#embededImageNameInSvg--}

Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded"

```javascript
embededImageNameInSvg : string;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please remove this property because images are now always embedded in Svg with base64 format. This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### sVGFitToViewPort {#sVGFitToViewPort--}

if this property is true, the generated svg will fit to view port.

```javascript
sVGFitToViewPort : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.FitToViewPort](../svgimageoptions.fittoviewport/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### svgCssPrefix {#svgCssPrefix--}

Gets and sets the prefix of the css name in svg,the default value is empty string.

```javascript
svgCssPrefix : string;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.CssPrefix](../svgimageoptions.cssprefix/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### onlyArea {#onlyArea--}

If this property is true , one Area will be output, and no scale will take effect.

```javascript
onlyArea : boolean;
```


### transparent {#transparent--}

Indicates if the background of generated image should be transparent.

```javascript
transparent : boolean;
```


**Remarks**

The default value is false. That means the background of the generated images is white.

### warningCallback {#warningCallback--}

Gets or sets warning callback.

```javascript
warningCallback : IWarningCallback;
```


### pageSavingCallback {#pageSavingCallback--}

Control/Indicate progress of page saving process.

```javascript
pageSavingCallback : IPageSavingCallback;
```


### isFontSubstitutionCharGranularity {#isFontSubstitutionCharGranularity--}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

```javascript
isFontSubstitutionCharGranularity : boolean;
```


**Remarks**

Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### pageIndex {#pageIndex--}

Gets or sets the 0-based index of the first page to save.

```javascript
pageIndex : number;
```


**Remarks**

Default is 0.

### pageCount {#pageCount--}

Gets or sets the number of pages to save.

```javascript
pageCount : number;
```


**Remarks**

Default is System.Int32.MaxValue which means all pages will be rendered.

### isOptimized {#isOptimized--}

Indicates whether to optimize the output elements.

```javascript
isOptimized : boolean;
```


**Remarks**

Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.

### defaultFont {#defaultFont--}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
defaultFont : string;
```


### checkWorkbookDefaultFont {#checkWorkbookDefaultFont--}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```javascript
checkWorkbookDefaultFont : boolean;
```


**Remarks**

Default is true.

### outputBlankPageWhenNothingToPrint {#outputBlankPageWhenNothingToPrint--}

Indicates whether to output a blank page when there is nothing to print.

```javascript
outputBlankPageWhenNothingToPrint : boolean;
```


**Remarks**

Default is false.

### gridlineType {#gridlineType--}

Gets or sets gridline type.

```javascript
gridlineType : GridlineType;
```


**Remarks**

Default is Dotted type.

### gridlineColor {#gridlineColor--}

Gets or sets gridline colr.

```javascript
gridlineColor : Color;
```


**Remarks**

It will ignore the gridline color settings in the source file.

### textCrossType {#textCrossType--}

Gets or sets displaying text type when the text width is larger than cell width.

```javascript
textCrossType : TextCrossType;
```


### defaultEditLanguage {#defaultEditLanguage--}

Gets or sets default edit language.

```javascript
defaultEditLanguage : DefaultEditLanguage;
```


**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).

### sheetSet {#sheetSet--}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
sheetSet : SheetSet;
```


**Remarks**

The set is ignored when it is used in [SheetRender](../sheetrender/)

### emfRenderSetting {#emfRenderSetting--}

Setting for rendering Emf metafiles in source file.

```javascript
emfRenderSetting : EmfRenderSetting;
```


**Remarks**

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

### customRenderSettings {#customRenderSettings--}

Gets or sets custom settings during rendering.

```javascript
customRenderSettings : CustomRenderSettings;
```


### setPrintWithStatusDialog(boolean) {#setPrintWithStatusDialog-boolean-}

<b>@deprecated.</b> Please use the 'printWithStatusDialog' property instead. If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.

```javascript
setPrintWithStatusDialog(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPrintWithStatusDialog() {#getPrintWithStatusDialog--}

<b>@deprecated.</b> Please use the 'printWithStatusDialog' property instead. If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.

```javascript
getPrintWithStatusDialog() : boolean;
```


### getHorizontalResolution() {#getHorizontalResolution--}

<b>@deprecated.</b> Please use the 'horizontalResolution' property instead. Gets or sets the horizontal resolution for generated images, in dots per inch.

```javascript
getHorizontalResolution() : number;
```


**Remarks**

ara>The default value is 96.</para> <para>Setting [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) effects the width and height of the output image in pixels.</para

### setHorizontalResolution(number) {#setHorizontalResolution-number-}

<b>@deprecated.</b> Please use the 'horizontalResolution' property instead. Gets or sets the horizontal resolution for generated images, in dots per inch.

```javascript
setHorizontalResolution(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

ara>The default value is 96.</para> <para>Setting [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) effects the width and height of the output image in pixels.</para

### getVerticalResolution() {#getVerticalResolution--}

<b>@deprecated.</b> Please use the 'verticalResolution' property instead. Gets or sets the vertical resolution for generated images, in dots per inch.

```javascript
getVerticalResolution() : number;
```


**Remarks**

ara>The default value is 96.</para> <para>Setting [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) effects the width and height of the output image in pixels.</para

### setVerticalResolution(number) {#setVerticalResolution-number-}

<b>@deprecated.</b> Please use the 'verticalResolution' property instead. Gets or sets the vertical resolution for generated images, in dots per inch.

```javascript
setVerticalResolution(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

ara>The default value is 96.</para> <para>Setting [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) effects the width and height of the output image in pixels.</para

### getTiffCompression() {#getTiffCompression--}

<b>@deprecated.</b> Please use the 'tiffCompression' property instead. Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format.

```javascript
getTiffCompression() : TiffCompression;
```


**Returns**

[TiffCompression](../tiffcompression/)

**Remarks**

Has effect only when saving to TIFF. The default value is Lzw.

### setTiffCompression(TiffCompression) {#setTiffCompression-tiffcompression-}

<b>@deprecated.</b> Please use the 'tiffCompression' property instead. Gets or sets the type of compression to apply only when saving pages to the <c>Tiff</c> format.

```javascript
setTiffCompression(value: TiffCompression) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TiffCompression](../tiffcompression/) | The value to set. |

**Remarks**

Has effect only when saving to TIFF. The default value is Lzw.

### getTiffColorDepth() {#getTiffColorDepth--}

<b>@deprecated.</b> Please use the 'tiffColorDepth' property instead. Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format.

```javascript
getTiffColorDepth() : ColorDepth;
```


**Returns**

[ColorDepth](../colordepth/)

**Remarks**

Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

### setTiffColorDepth(ColorDepth) {#setTiffColorDepth-colordepth-}

<b>@deprecated.</b> Please use the 'tiffColorDepth' property instead. Gets or sets bit depth to apply only when saving pages to the <c>Tiff</c> format.

```javascript
setTiffColorDepth(value: ColorDepth) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ColorDepth](../colordepth/) | The value to set. |

**Remarks**

Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

### getTiffBinarizationMethod() {#getTiffBinarizationMethod--}

<b>@deprecated.</b> Please use the 'tiffBinarizationMethod' property instead. Gets or sets method used while converting images to 1 bpp format when [ImageType](../imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4.

```javascript
getTiffBinarizationMethod() : ImageBinarizationMethod;
```


**Returns**

[ImageBinarizationMethod](../imagebinarizationmethod/)

**Remarks**

The default value is FloydSteinbergDithering.

### setTiffBinarizationMethod(ImageBinarizationMethod) {#setTiffBinarizationMethod-imagebinarizationmethod-}

<b>@deprecated.</b> Please use the 'tiffBinarizationMethod' property instead. Gets or sets method used while converting images to 1 bpp format when [ImageType](../imagetype/) is Tiff and [TiffCompression](../tiffcompression/) is equal to Ccitt3 or Ccitt4.

```javascript
setTiffBinarizationMethod(value: ImageBinarizationMethod) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageBinarizationMethod](../imagebinarizationmethod/) | The value to set. |

**Remarks**

The default value is FloydSteinbergDithering.

### getPrintingPage() {#getPrintingPage--}

<b>@deprecated.</b> Please use the 'printingPage' property instead. Indicates which pages will not be printed.

```javascript
getPrintingPage() : PrintingPageType;
```


**Returns**

[PrintingPageType](../printingpagetype/)

### setPrintingPage(PrintingPageType) {#setPrintingPage-printingpagetype-}

<b>@deprecated.</b> Please use the 'printingPage' property instead. Indicates which pages will not be printed.

```javascript
setPrintingPage(value: PrintingPageType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintingPageType](../printingpagetype/) | The value to set. |

### getQuality() {#getQuality--}

<b>@deprecated.</b> Please use the 'quality' property instead. Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100

```javascript
getQuality() : number;
```


**Remarks**

Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

### setQuality(number) {#setQuality-number-}

<b>@deprecated.</b> Please use the 'quality' property instead. Gets or sets a value determining the quality of the generated  images to apply only when saving pages to the <c>Jpeg</c> format. The default value is 100

```javascript
setQuality(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

### getOnePagePerSheet() {#getOnePagePerSheet--}

<b>@deprecated.</b> Please use the 'onePagePerSheet' property instead. If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
getOnePagePerSheet() : boolean;
```


### setOnePagePerSheet(boolean) {#setOnePagePerSheet-boolean-}

<b>@deprecated.</b> Please use the 'onePagePerSheet' property instead. If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
setOnePagePerSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}

<b>@deprecated.</b> Please use the 'allColumnsInOnePagePerSheet' property instead. If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
getAllColumnsInOnePagePerSheet() : boolean;
```


### setAllColumnsInOnePagePerSheet(boolean) {#setAllColumnsInOnePagePerSheet-boolean-}

<b>@deprecated.</b> Please use the 'allColumnsInOnePagePerSheet' property instead. If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
setAllColumnsInOnePagePerSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}

<b>@deprecated.</b> Please use the 'drawObjectEventHandler' property instead. Implements this interface to get DrawObject and Bound when rendering.

```javascript
getDrawObjectEventHandler() : DrawObjectEventHandler;
```


**Returns**

[DrawObjectEventHandler](../drawobjecteventhandler/)

### setDrawObjectEventHandler(DrawObjectEventHandler) {#setDrawObjectEventHandler-drawobjecteventhandler-}

<b>@deprecated.</b> Please use the 'drawObjectEventHandler' property instead. Implements this interface to get DrawObject and Bound when rendering.

```javascript
setDrawObjectEventHandler(value: DrawObjectEventHandler) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../drawobjecteventhandler/) | The value to set. |

### getEmbededImageNameInSvg() {#getEmbededImageNameInSvg--}

<b>@deprecated.</b> Please use the 'embededImageNameInSvg' property instead. Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded"

```javascript
getEmbededImageNameInSvg() : string;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please remove this property because images are now always embedded in Svg with base64 format. This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### setEmbededImageNameInSvg(string) {#setEmbededImageNameInSvg-string-}

<b>@deprecated.</b> Please use the 'embededImageNameInSvg' property instead. Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded"

```javascript
setEmbededImageNameInSvg(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please remove this property because images are now always embedded in Svg with base64 format. This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### getSVGFitToViewPort() {#getSVGFitToViewPort--}

<b>@deprecated.</b> Please use the 'sVGFitToViewPort' property instead. if this property is true, the generated svg will fit to view port.

```javascript
getSVGFitToViewPort() : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.FitToViewPort](../svgimageoptions.fittoviewport/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### setSVGFitToViewPort(boolean) {#setSVGFitToViewPort-boolean-}

<b>@deprecated.</b> Please use the 'sVGFitToViewPort' property instead. if this property is true, the generated svg will fit to view port.

```javascript
setSVGFitToViewPort(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.FitToViewPort](../svgimageoptions.fittoviewport/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### getSvgCssPrefix() {#getSvgCssPrefix--}

<b>@deprecated.</b> Please use the 'svgCssPrefix' property instead. Gets and sets the prefix of the css name in svg,the default value is empty string.

```javascript
getSvgCssPrefix() : string;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.CssPrefix](../svgimageoptions.cssprefix/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### setSvgCssPrefix(string) {#setSvgCssPrefix-string-}

<b>@deprecated.</b> Please use the 'svgCssPrefix' property instead. Gets and sets the prefix of the css name in svg,the default value is empty string.

```javascript
setSvgCssPrefix(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use [SvgImageOptions.CssPrefix](../svgimageoptions.cssprefix/). This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.

### getOnlyArea() {#getOnlyArea--}

<b>@deprecated.</b> Please use the 'onlyArea' property instead. If this property is true , one Area will be output, and no scale will take effect.

```javascript
getOnlyArea() : boolean;
```


### setOnlyArea(boolean) {#setOnlyArea-boolean-}

<b>@deprecated.</b> Please use the 'onlyArea' property instead. If this property is true , one Area will be output, and no scale will take effect.

```javascript
setOnlyArea(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTransparent() {#getTransparent--}

<b>@deprecated.</b> Please use the 'transparent' property instead. Indicates if the background of generated image should be transparent.

```javascript
getTransparent() : boolean;
```


**Remarks**

The default value is false. That means the background of the generated images is white.

### setTransparent(boolean) {#setTransparent-boolean-}

<b>@deprecated.</b> Please use the 'transparent' property instead. Indicates if the background of generated image should be transparent.

```javascript
setTransparent(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false. That means the background of the generated images is white.

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

<b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

<b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](../iwarningcallback/)

### getPageSavingCallback() {#getPageSavingCallback--}

<b>@deprecated.</b> Please use the 'pageSavingCallback' property instead. Control/Indicate progress of page saving process.

```javascript
getPageSavingCallback() : IPageSavingCallback;
```


**Returns**

[IPageSavingCallback](../ipagesavingcallback/)

### setPageSavingCallback(IPageSavingCallback) {#setPageSavingCallback-ipagesavingcallback-}

<b>@deprecated.</b> Please use the 'pageSavingCallback' property instead. Control/Indicate progress of page saving process.

```javascript
setPageSavingCallback(value: IPageSavingCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../ipagesavingcallback/) | The value to set. |

### setIsFontSubstitutionCharGranularity(boolean) {#setIsFontSubstitutionCharGranularity-boolean-}

<b>@deprecated.</b> Please use the 'isFontSubstitutionCharGranularity' property instead. Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

```javascript
setIsFontSubstitutionCharGranularity(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}

<b>@deprecated.</b> Please use the 'isFontSubstitutionCharGranularity' property instead. Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

```javascript
isFontSubstitutionCharGranularity() : boolean;
```


**Remarks**

Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### setPageIndex(number) {#setPageIndex-number-}

<b>@deprecated.</b> Please use the 'pageIndex' property instead. Gets or sets the 0-based index of the first page to save.

```javascript
setPageIndex(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Default is 0.

### getPageIndex() {#getPageIndex--}

<b>@deprecated.</b> Please use the 'pageIndex' property instead. Gets or sets the 0-based index of the first page to save.

```javascript
getPageIndex() : number;
```


**Remarks**

Default is 0.

### setPageCount(number) {#setPageCount-number-}

<b>@deprecated.</b> Please use the 'pageCount' property instead. Gets or sets the number of pages to save.

```javascript
setPageCount(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Default is System.Int32.MaxValue which means all pages will be rendered.

### getPageCount() {#getPageCount--}

<b>@deprecated.</b> Please use the 'pageCount' property instead. Gets or sets the number of pages to save.

```javascript
getPageCount() : number;
```


**Remarks**

Default is System.Int32.MaxValue which means all pages will be rendered.

### isOptimized() {#isOptimized--}

<b>@deprecated.</b> Please use the 'isOptimized' property instead. Indicates whether to optimize the output elements.

```javascript
isOptimized() : boolean;
```


**Remarks**

Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.

### setIsOptimized(boolean) {#setIsOptimized-boolean-}

<b>@deprecated.</b> Please use the 'isOptimized' property instead. Indicates whether to optimize the output elements.

```javascript
setIsOptimized(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.

### getDefaultFont() {#getDefaultFont--}

<b>@deprecated.</b> Please use the 'defaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
getDefaultFont() : string;
```


### setDefaultFont(string) {#setDefaultFont-string-}

<b>@deprecated.</b> Please use the 'defaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
setDefaultFont(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}

<b>@deprecated.</b> Please use the 'checkWorkbookDefaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```javascript
getCheckWorkbookDefaultFont() : boolean;
```


**Remarks**

Default is true.

### setCheckWorkbookDefaultFont(boolean) {#setCheckWorkbookDefaultFont-boolean-}

<b>@deprecated.</b> Please use the 'checkWorkbookDefaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```javascript
setCheckWorkbookDefaultFont(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Default is true.

### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}

<b>@deprecated.</b> Please use the 'outputBlankPageWhenNothingToPrint' property instead. Indicates whether to output a blank page when there is nothing to print.

```javascript
getOutputBlankPageWhenNothingToPrint() : boolean;
```


**Remarks**

Default is false.

### setOutputBlankPageWhenNothingToPrint(boolean) {#setOutputBlankPageWhenNothingToPrint-boolean-}

<b>@deprecated.</b> Please use the 'outputBlankPageWhenNothingToPrint' property instead. Indicates whether to output a blank page when there is nothing to print.

```javascript
setOutputBlankPageWhenNothingToPrint(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Default is false.

### getGridlineType() {#getGridlineType--}

<b>@deprecated.</b> Please use the 'gridlineType' property instead. Gets or sets gridline type.

```javascript
getGridlineType() : GridlineType;
```


**Returns**

[GridlineType](../gridlinetype/)

**Remarks**

Default is Dotted type.

### setGridlineType(GridlineType) {#setGridlineType-gridlinetype-}

<b>@deprecated.</b> Please use the 'gridlineType' property instead. Gets or sets gridline type.

```javascript
setGridlineType(value: GridlineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridlineType](../gridlinetype/) | The value to set. |

**Remarks**

Default is Dotted type.

### getGridlineColor() {#getGridlineColor--}

<b>@deprecated.</b> Please use the 'gridlineColor' property instead. Gets or sets gridline colr.

```javascript
getGridlineColor() : Color;
```


**Returns**

[Color](../color/)

**Remarks**

It will ignore the gridline color settings in the source file.

### setGridlineColor(Color) {#setGridlineColor-color-}

<b>@deprecated.</b> Please use the 'gridlineColor' property instead. Gets or sets gridline colr.

```javascript
setGridlineColor(value: Color) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |

**Remarks**

It will ignore the gridline color settings in the source file.

### getTextCrossType() {#getTextCrossType--}

<b>@deprecated.</b> Please use the 'textCrossType' property instead. Gets or sets displaying text type when the text width is larger than cell width.

```javascript
getTextCrossType() : TextCrossType;
```


**Returns**

[TextCrossType](../textcrosstype/)

### setTextCrossType(TextCrossType) {#setTextCrossType-textcrosstype-}

<b>@deprecated.</b> Please use the 'textCrossType' property instead. Gets or sets displaying text type when the text width is larger than cell width.

```javascript
setTextCrossType(value: TextCrossType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextCrossType](../textcrosstype/) | The value to set. |

### getDefaultEditLanguage() {#getDefaultEditLanguage--}

<b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language.

```javascript
getDefaultEditLanguage() : DefaultEditLanguage;
```


**Returns**

[DefaultEditLanguage](../defaulteditlanguage/)

**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).

### setDefaultEditLanguage(DefaultEditLanguage) {#setDefaultEditLanguage-defaulteditlanguage-}

<b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language.

```javascript
setDefaultEditLanguage(value: DefaultEditLanguage) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DefaultEditLanguage](../defaulteditlanguage/) | The value to set. |

**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).

### getSheetSet() {#getSheetSet--}

<b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
getSheetSet() : SheetSet;
```


**Returns**

[SheetSet](../sheetset/)

**Remarks**

The set is ignored when it is used in [SheetRender](../sheetrender/)

### setSheetSet(SheetSet) {#setSheetSet-sheetset-}

<b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
setSheetSet(value: SheetSet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../sheetset/) | The value to set. |

**Remarks**

The set is ignored when it is used in [SheetRender](../sheetrender/)

### getEmfRenderSetting() {#getEmfRenderSetting--}

<b>@deprecated.</b> Please use the 'emfRenderSetting' property instead. Setting for rendering Emf metafiles in source file.

```javascript
getEmfRenderSetting() : EmfRenderSetting;
```


**Returns**

[EmfRenderSetting](../emfrendersetting/)

**Remarks**

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

### setEmfRenderSetting(EmfRenderSetting) {#setEmfRenderSetting-emfrendersetting-}

<b>@deprecated.</b> Please use the 'emfRenderSetting' property instead. Setting for rendering Emf metafiles in source file.

```javascript
setEmfRenderSetting(value: EmfRenderSetting) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EmfRenderSetting](../emfrendersetting/) | The value to set. |

**Remarks**

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/). For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

### getCustomRenderSettings() {#getCustomRenderSettings--}

<b>@deprecated.</b> Please use the 'customRenderSettings' property instead. Gets or sets custom settings during rendering.

```javascript
getCustomRenderSettings() : CustomRenderSettings;
```


**Returns**

[CustomRenderSettings](../customrendersettings/)

### setCustomRenderSettings(CustomRenderSettings) {#setCustomRenderSettings-customrendersettings-}

<b>@deprecated.</b> Please use the 'customRenderSettings' property instead. Gets or sets custom settings during rendering.

```javascript
setCustomRenderSettings(value: CustomRenderSettings) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomRenderSettings](../customrendersettings/) | The value to set. |

### setDesiredSize(number, number, boolean) {#setDesiredSize-number-number-boolean-}

Sets desired width and height of image.

```javascript
setDesiredSize(desiredWidth: number, desiredHeight: number, keepAspectRatio: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | number | desired width in pixels |
| desiredHeight | number | desired height in pixels |
| keepAspectRatio | boolean | whether to keep aspect ratio of origin image |

**Remarks**

ara>The width and height of the output image in pixels will be only based on the set desired width and height.</para> <para>The [HorizontalResolution](../horizontalresolution/) and [VerticalResolution](../verticalresolution/) will not effect the width and height of the output image in this case.</para

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getImageType() {#getImageType--}

Gets or sets the format of the generated images. default value: PNG.

```javascript
getImageType() : ImageType;
```


**Returns**

[ImageType](../imagetype/)

### setImageType(ImageType) {#setImageType-imagetype-}

Gets or sets the format of the generated images. default value: PNG.

```javascript
setImageType(value: ImageType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageType](../imagetype/) | The value to set. |


