---
title: "ImageOrPrintOptions"
linktitle: "ImageOrPrintOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image."
type: docs
weight: 1900
url: /nodejs/aspose.cells/imageorprintoptions/
---

## ImageOrPrintOptions class

Allows to specify options when rendering worksheet to images, printing worksheet or rendering chart to image.

```js
new ImageOrPrintOptions()
```

## Methods

| Name | Description |
| --- | --- |
| [getAllColumnsInOnePagePerSheet()](#getallcolumnsinonepagepersheet) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The wid |
| [getChartImageType()](#getchartimagetype) | Indicate the chart imagetype when converting. default value: PNG. NOTE: This member is now obsolete. Instead, Chart and  |
| [getCheckWorkbookDefaultFont()](#getcheckworkbookdefaultfont) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [getCustomRenderSettings()](#getcustomrendersettings) |  |
| [getDefaultEditLanguage()](#getdefaulteditlanguage) | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [getDefaultFont()](#getdefaultfont) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [getDrawObjectEventHandler()](#getdrawobjecteventhandler) | Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbededImageNameInSvg()](#getembededimagenameinsvg) | Indicate the filename of embedded image in svg. This should be full path with directory like "c:\xpsEmbedded" |
| [getEmfRenderSetting()](#getemfrendersetting) | Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identi |
| [getGridlineColor()](#getgridlinecolor) |  |
| [getGridlineType()](#getgridlinetype) | Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type. |
| [getHorizontalResolution()](#gethorizontalresolution) | Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Em |
| [getImageType()](#getimagetype) | Gets or sets the format of the generated images. default value: PNG. The value of the property is ImageType integer cons |
| [getOnePagePerSheet()](#getonepagepersheet) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetu |
| [getOnlyArea()](#getonlyarea) | If this property is true , one Area will be output, and no scale will take effect. |
| [getOutputBlankPageWhenNothingToPrint()](#getoutputblankpagewhennothingtoprint) | Indicates whether to output a blank page when there is nothing to print. Default is false. |
| [getPageCount()](#getpagecount) | Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered. |
| [getPageIndex()](#getpageindex) | Gets or sets the 0-based index of the first page to save. Default is 0. |
| [getPageSavingCallback()](#getpagesavingcallback) | Control/Indicate progress of page saving process. |
| [getPrintWithStatusDialog()](#getprintwithstatusdialog) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [getPrintingPage()](#getprintingpage) | Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. |
| [getQuality()](#getquality) | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. |
| [getSVGFitToViewPort()](#getsvgfittoviewport) | if this property is true, the generated svg will fit to view port. |
| [getSaveFormat()](#getsaveformat) | Gets or sets the output file format type Support Tiff/XPS The value of the property is SaveFormat integer constant. NOTE |
| [getSheetSet()](#getsheetset) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible. The set is ignored w |
| [getSvgCssPrefix()](#getsvgcssprefix) |  |
| [getTextCrossType()](#gettextcrosstype) | Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossT |
| [getTiffColorDepth()](#gettiffcolordepth) | Gets or sets bit depth to apply only when saving pages to the Tiff format. The value of the property is ColorDepth integ |
| [getTiffCompression()](#gettiffcompression) | Gets or sets the type of compression to apply only when saving pages to the Tiff format. The value of the property is Ti |
| [getTiffPhotometricInterpretation()](#gettiffphotometricinterpretation) | Gets the type of PhotometricInterpretation to apply only when saving pages to the Tiff format. Has effect only when savi |
| [getTransparent()](#gettransparent) | Indicates if the background of generated image should be transparent. The default value is false. That means the backgro |
| [getVerticalResolution()](#getverticalresolution) | Gets or sets the vertical resolution for generated images, in dots per inch. Applies generating image method except Emf  |
| [isCellAutoFit()](#iscellautofit) | Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. N |
| [isFontSubstitutionCharGranularity()](#isfontsubstitutionchargranularity) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is fa |
| [isOptimized()](#isoptimized) | Indicates whether to optimize the output elements. Default value is false. Currently when this property is set to true,  |
| [setAllColumnsInOnePagePerSheet()](#setallcolumnsinonepagepersheet) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The wid |
| [setCellAutoFit()](#setcellautofit) | Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. N |
| [setChartImageType()](#setchartimagetype) | Indicate the chart imagetype when converting. default value: PNG. NOTE: This member is now obsolete. Instead, Chart and  |
| [setCheckWorkbookDefaultFont()](#setcheckworkbookdefaultfont) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [setCustomRenderSettings()](#setcustomrendersettings) |  |
| [setDefaultEditLanguage()](#setdefaulteditlanguage) | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [setDefaultFont()](#setdefaultfont) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [setDesiredSize(desiredWidth, desiredHeight)](#setdesiredsize) | Sets desired width and height of image. NOTE: This member is now obsolete. Instead, please use setDesiredSize(int, int,  |
| [setDesiredSize(desiredWidth, desiredHeight, keepAspectRatio)](#setdesiredsize-1) | Sets desired width and height of image. |
| [setDrawObjectEventHandler()](#setdrawobjecteventhandler) | Implements this interface to get DrawObject and Bound when rendering. |
| [setEmbededImageNameInSvg()](#setembededimagenameinsvg) | Indicate the filename of embedded image in svg. This should be full path with directory like "c:\xpsEmbedded" |
| [setEmfRenderSetting()](#setemfrendersetting) | Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identi |
| [setFontSubstitutionCharGranularity()](#setfontsubstitutionchargranularity) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is fa |
| [setGridlineColor()](#setgridlinecolor) |  |
| [setGridlineType()](#setgridlinetype) | Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type. |
| [setHorizontalResolution()](#sethorizontalresolution) | Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Em |
| [setImageType()](#setimagetype) | Gets or sets the format of the generated images. default value: PNG. The value of the property is ImageType integer cons |
| [setOnePagePerSheet()](#setonepagepersheet) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetu |
| [setOnlyArea()](#setonlyarea) | If this property is true , one Area will be output, and no scale will take effect. |
| [setOptimized()](#setoptimized) | Indicates whether to optimize the output elements. Default value is false. Currently when this property is set to true,  |
| [setOutputBlankPageWhenNothingToPrint()](#setoutputblankpagewhennothingtoprint) | Indicates whether to output a blank page when there is nothing to print. Default is false. |
| [setPageCount()](#setpagecount) | Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered. |
| [setPageIndex()](#setpageindex) | Gets or sets the 0-based index of the first page to save. Default is 0. |
| [setPageSavingCallback()](#setpagesavingcallback) | Control/Indicate progress of page saving process. |
| [setPrintWithStatusDialog()](#setprintwithstatusdialog) | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [setPrintingPage()](#setprintingpage) | Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. |
| [setQuality()](#setquality) | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. |
| [setRenderingHint(key, value)](#setrenderinghint) | Sets the value of a single preference for the rendering algorithms. Hint categories include controls for rendering quali |
| [setSVGFitToViewPort()](#setsvgfittoviewport) | if this property is true, the generated svg will fit to view port. |
| [setSaveFormat()](#setsaveformat) | Gets or sets the output file format type Support Tiff/XPS The value of the property is SaveFormat integer constant. NOTE |
| [setSheetSet()](#setsheetset) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible. The set is ignored w |
| [setSvgCssPrefix()](#setsvgcssprefix) |  |
| [setTextCrossType()](#settextcrosstype) | Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossT |
| [setTiffColorDepth()](#settiffcolordepth) | Gets or sets bit depth to apply only when saving pages to the Tiff format. The value of the property is ColorDepth integ |
| [setTiffCompression()](#settiffcompression) | Gets or sets the type of compression to apply only when saving pages to the Tiff format. The value of the property is Ti |
| [setTiffPhotometricInterpretation()](#settiffphotometricinterpretation) | Sets the type of PhotometricInterpretation to apply only when saving pages to the Tiff format. Has effect only when savi |
| [setTransparent()](#settransparent) | Indicates if the background of generated image should be transparent. The default value is false. That means the backgro |
| [setVerticalResolution()](#setverticalresolution) | Gets or sets the vertical resolution for generated images, in dots per inch. Applies generating image method except Emf  |

### getAllColumnsInOnePagePerSheet() {#getallcolumnsinonepagepersheet}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

### getChartImageType() {#getchartimagetype}

Indicate the chart imagetype when converting. default value: PNG. NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### getCheckWorkbookDefaultFont() {#getcheckworkbookdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. Default is true.

### getCustomRenderSettings() {#getcustomrendersettings}

### getDefaultEditLanguage() {#getdefaulteditlanguage}

Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO.

### getDefaultFont() {#getdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

### getDrawObjectEventHandler() {#getdrawobjecteventhandler}

Implements this interface to get DrawObject and Bound when rendering.

### getEmbededImageNameInSvg() {#getembededimagenameinsvg}

Indicate the filename of embedded image in svg. This should be full path with directory like "c:\xpsEmbedded"

### getEmfRenderSetting() {#getemfrendersetting}

Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF_PLUS_PREFER is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF_ONLY. For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

### getGridlineColor() {#getgridlinecolor}

### getGridlineType() {#getgridlinetype}

Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type.

### getHorizontalResolution() {#gethorizontalresolution}

Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images. The default value is 96.

### getImageType() {#getimagetype}

Gets or sets the format of the generated images. default value: PNG. The value of the property is ImageType integer constant.

### getOnePagePerSheet() {#getonepagepersheet}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

### getOnlyArea() {#getonlyarea}

If this property is true , one Area will be output, and no scale will take effect.

### getOutputBlankPageWhenNothingToPrint() {#getoutputblankpagewhennothingtoprint}

Indicates whether to output a blank page when there is nothing to print. Default is false.

### getPageCount() {#getpagecount}

Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.

### getPageIndex() {#getpageindex}

Gets or sets the 0-based index of the first page to save. Default is 0.

### getPageSavingCallback() {#getpagesavingcallback}

Control/Indicate progress of page saving process.

### getPrintWithStatusDialog() {#getprintwithstatusdialog}

If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.

### getPrintingPage() {#getprintingpage}

Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant.

### getQuality() {#getquality}

Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. The default value is 100 Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

### getSVGFitToViewPort() {#getsvgfittoviewport}

if this property is true, the generated svg will fit to view port.

### getSaveFormat() {#getsaveformat}

Gets or sets the output file format type Support Tiff/XPS The value of the property is SaveFormat integer constant. NOTE: This member is now obsolete. Instead, For Tiff/Svg, use ImageType; For Xps, use Workbook.save(java.lang.String, com.aspose.cells.SaveOptions) with XpsSaveOptions. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

### getSheetSet() {#getsheetset}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible. The set is ignored when it is used in SheetRender

### getSvgCssPrefix() {#getsvgcssprefix}

### getTextCrossType() {#gettextcrosstype}

Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossType integer constant.

### getTiffColorDepth() {#gettiffcolordepth}

Gets or sets bit depth to apply only when saving pages to the Tiff format. The value of the property is ColorDepth integer constant. Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

### getTiffCompression() {#gettiffcompression}

Gets or sets the type of compression to apply only when saving pages to the Tiff format. The value of the property is TiffCompression integer constant. Has effect only when saving to TIFF. The default value is Lzw.

### getTiffPhotometricInterpretation() {#gettiffphotometricinterpretation}

Gets the type of PhotometricInterpretation to apply only when saving pages to the Tiff format. Has effect only when saving to TIFF. The default value is -1, represent no PhotometricInterpretation is applied.

### getTransparent() {#gettransparent}

Indicates if the background of generated image should be transparent. The default value is false. That means the background of the generated images is white.

### getVerticalResolution() {#getverticalresolution}

Gets or sets the vertical resolution for generated images, in dots per inch. Applies generating image method except Emf format image. The default value is 96.

### isCellAutoFit() {#iscellautofit}

Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. NOTE: This member is now obsolete. Instead, please use Worksheet.autoFitColumns(com.aspose.cells.AutoFitterOptions) and Worksheet.autoFitRows(com.aspose.cells.AutoFitterOptions). This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

### isFontSubstitutionCharGranularity() {#isfontsubstitutionchargranularity}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### isOptimized() {#isoptimized}

Indicates whether to optimize the output elements. Default value is false. Currently when this property is set to true, the following optimizations will be done:

### setAllColumnsInOnePagePerSheet() {#setallcolumnsinonepagepersheet}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

### setCellAutoFit() {#setcellautofit}

Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. NOTE: This member is now obsolete. Instead, please use Worksheet.autoFitColumns(com.aspose.cells.AutoFitterOptions) and Worksheet.autoFitRows(com.aspose.cells.AutoFitterOptions). This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

### setChartImageType() {#setchartimagetype}

Indicate the chart imagetype when converting. default value: PNG. NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### setCheckWorkbookDefaultFont() {#setcheckworkbookdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. Default is true.

### setCustomRenderSettings() {#setcustomrendersettings}

### setDefaultEditLanguage() {#setdefaulteditlanguage}

Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO.

### setDefaultFont() {#setdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

### setDesiredSize(desiredWidth, desiredHeight) {#setdesiredsize}

Sets desired width and height of image. NOTE: This member is now obsolete. Instead, please use setDesiredSize(int, int, boolean) by setting param keepAspectRatio to false. This property will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | Number | desired width in pixels |
| desiredHeight | Number | desired height in pixels |

### setDesiredSize(desiredWidth, desiredHeight, keepAspectRatio) {#setdesiredsize-1}

Sets desired width and height of image.

| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | Number | desired width in pixels |
| desiredHeight | Number | desired height in pixels |
| keepAspectRatio | boolean | whether to keep aspect ratio of origin image |

### setDrawObjectEventHandler() {#setdrawobjecteventhandler}

Implements this interface to get DrawObject and Bound when rendering.

### setEmbededImageNameInSvg() {#setembededimagenameinsvg}

Indicate the filename of embedded image in svg. This should be full path with directory like "c:\xpsEmbedded"

### setEmfRenderSetting() {#setemfrendersetting}

Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF_PLUS_PREFER is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF_ONLY. For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

### setFontSubstitutionCharGranularity() {#setfontsubstitutionchargranularity}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### setGridlineColor() {#setgridlinecolor}

### setGridlineType() {#setgridlinetype}

Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type.

### setHorizontalResolution() {#sethorizontalresolution}

Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images. The default value is 96.

### setImageType() {#setimagetype}

Gets or sets the format of the generated images. default value: PNG. The value of the property is ImageType integer constant.

### setOnePagePerSheet() {#setonepagepersheet}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

### setOnlyArea() {#setonlyarea}

If this property is true , one Area will be output, and no scale will take effect.

### setOptimized() {#setoptimized}

Indicates whether to optimize the output elements. Default value is false. Currently when this property is set to true, the following optimizations will be done:

### setOutputBlankPageWhenNothingToPrint() {#setoutputblankpagewhennothingtoprint}

Indicates whether to output a blank page when there is nothing to print. Default is false.

### setPageCount() {#setpagecount}

Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.

### setPageIndex() {#setpageindex}

Gets or sets the 0-based index of the first page to save. Default is 0.

### setPageSavingCallback() {#setpagesavingcallback}

Control/Indicate progress of page saving process.

### setPrintWithStatusDialog() {#setprintwithstatusdialog}

If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.

### setPrintingPage() {#setprintingpage}

Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant.

### setQuality() {#setquality}

Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. The default value is 100 Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

### setRenderingHint(key, value) {#setrenderinghint}

Sets the value of a single preference for the rendering algorithms. Hint categories include controls for rendering quality and overall time/quality trade-off in the rendering process. Refer to the RenderingHints class for definitions of some common keys and values.

| Parameter | Type | Description |
| --- | --- | --- |
| key | Key | the key of the hint to be set. |
| value | Object | the value indicating preferences for the specified hint category. |

### setSVGFitToViewPort() {#setsvgfittoviewport}

if this property is true, the generated svg will fit to view port.

### setSaveFormat() {#setsaveformat}

Gets or sets the output file format type Support Tiff/XPS The value of the property is SaveFormat integer constant. NOTE: This member is now obsolete. Instead, For Tiff/Svg, use ImageType; For Xps, use Workbook.save(java.lang.String, com.aspose.cells.SaveOptions) with XpsSaveOptions. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

### setSheetSet() {#setsheetset}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible. The set is ignored when it is used in SheetRender

### setSvgCssPrefix() {#setsvgcssprefix}

### setTextCrossType() {#settextcrosstype}

Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossType integer constant.

### setTiffColorDepth() {#settiffcolordepth}

Gets or sets bit depth to apply only when saving pages to the Tiff format. The value of the property is ColorDepth integer constant. Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

### setTiffCompression() {#settiffcompression}

Gets or sets the type of compression to apply only when saving pages to the Tiff format. The value of the property is TiffCompression integer constant. Has effect only when saving to TIFF. The default value is Lzw.

### setTiffPhotometricInterpretation() {#settiffphotometricinterpretation}

Sets the type of PhotometricInterpretation to apply only when saving pages to the Tiff format. Has effect only when saving to TIFF. The default value is -1, represent no PhotometricInterpretation is applied.

### setTransparent() {#settransparent}

Indicates if the background of generated image should be transparent. The default value is false. That means the background of the generated images is white.

### setVerticalResolution() {#setverticalresolution}

Gets or sets the vertical resolution for generated images, in dots per inch. Applies generating image method except Emf format image. The default value is 96.
