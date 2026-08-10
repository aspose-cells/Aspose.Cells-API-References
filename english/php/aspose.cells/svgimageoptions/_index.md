---
title: "SvgImageOptions Class"
linktitle: "SvgImageOptions"
articleTitle: "SvgImageOptions"
second_title: "Aspose.Cells for PHP via Java"
description: ""
type: docs
weight: 6470
url: /php/aspose.cells/svgimageoptions/
---

## SvgImageOptions class

## Constructors

| Name | Description |
| --- | --- |
| [SvgImageOptions](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ImageType](#imagetype) | Number | The value of the property is ImageType integer constant. |
| [FitToViewPort](#fittoviewport) | boolean |  |
| [CssPrefix](#cssprefix) | String |  |
| [EmbeddedFontType](#embeddedfonttype) | Number | The value of the property is SvgEmbeddedFontType integer constant. |
| [SaveFormat](#saveformat) | Number | Gets or sets the output file format type Support Tiff/XPS The value of the property is SaveFormat integer constant. NOTE |
| [PrintWithStatusDialog](#printwithstatusdialog) | boolean | If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show. |
| [HorizontalResolution](#horizontalresolution) | Number | Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Em |
| [VerticalResolution](#verticalresolution) | Number | Gets or sets the vertical resolution for generated images, in dots per inch. Applies generating image method except Emf  |
| [TiffCompression](#tiffcompression) | Number | Gets or sets the type of compression to apply only when saving pages to the Tiff format. The value of the property is Ti |
| [TiffColorDepth](#tiffcolordepth) | Number | Gets or sets bit depth to apply only when saving pages to the Tiff format. The value of the property is ColorDepth integ |
| [PrintingPage](#printingpage) | Number | Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. |
| [Quality](#quality) | Number | Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. |
| [IsCellAutoFit](#iscellautofit) | boolean | Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. N |
| [OnePagePerSheet](#onepagepersheet) | boolean | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetu |
| [AllColumnsInOnePagePerSheet](#allcolumnsinonepagepersheet) | boolean | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The wid |
| [DrawObjectEventHandler](#drawobjecteventhandler) | DrawObjectEventHandler | Implements this interface to get DrawObject and Bound when rendering. |
| [ChartImageType](#chartimagetype) | ImageFormat | Indicate the chart imagetype when converting. default value: PNG. NOTE: This member is now obsolete. Instead, Chart and  |
| [EmbededImageNameInSvg](#embededimagenameinsvg) | String | Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded" |
| [SVGFitToViewPort](#svgfittoviewport) | boolean | if this property is true, the generated svg will fit to view port. |
| [SvgCssPrefix](#svgcssprefix) | String |  |
| [OnlyArea](#onlyarea) | boolean | If this property is true , one Area will be output, and no scale will take effect. |
| [Transparent](#transparent) | boolean | Indicates if the background of generated image should be transparent. The default value is false. That means the backgro |
| [WarningCallback](#warningcallback) | IWarningCallback | Gets or sets warning callback. |
| [PageSavingCallback](#pagesavingcallback) | IPageSavingCallback | Control/Indicate progress of page saving process. |
| [IsFontSubstitutionCharGranularity](#isfontsubstitutionchargranularity) | boolean | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is fa |
| [PageIndex](#pageindex) | Number | Gets or sets the 0-based index of the first page to save. Default is 0. |
| [PageCount](#pagecount) | Number | Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered. |
| [IsOptimized](#isoptimized) | boolean | Indicates whether to optimize the output elements. Default value is false. Currently when this property is set to true,  |
| [DefaultFont](#defaultfont) | String | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [CheckWorkbookDefaultFont](#checkworkbookdefaultfont) | boolean | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [OutputBlankPageWhenNothingToPrint](#outputblankpagewhennothingtoprint) | boolean | Indicates whether to output a blank page when there is nothing to print. Default is false. |
| [GridlineType](#gridlinetype) | Number | Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type. |
| [GridlineColor](#gridlinecolor) | Color |  |
| [TextCrossType](#textcrosstype) | Number | Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossT |
| [DefaultEditLanguage](#defaulteditlanguage) | Number | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [SheetSet](#sheetset) | SheetSet | Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible . The set is ignored  |
| [EmfRenderSetting](#emfrendersetting) | Number | Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identi |
| [CustomRenderSettings](#customrendersettings) | CustomRenderSettings |  |

## Methods

| Name | Description |
| --- | --- |
| [getTiffPhotometricInterpretation](#gettiffphotometricinterpretation) | Gets the type of PhotometricInterpretation to apply only when saving pages to the Tiff format.

Has effect only when sav |
| [setTiffPhotometricInterpretation](#settiffphotometricinterpretation) | Sets the type of PhotometricInterpretation to apply only when saving pages to the Tiff format.

Has effect only when sav |
| [setRenderingHint](#setrenderinghint) | Sets the value of a single preference for the rendering algorithms. Hint categories include controls for rendering quali |
| [setDesiredSize](#setdesiredsize) | Sets desired width and height of image.

NOTE: This member is now obsolete. Instead, please use setDesiredSize(int, int, |

### SvgImageOptions() {#constructor}

### SvgImageOptions.ImageType property {#imagetype}

The value of the property is ImageType integer constant.

**Type:** Number

### SvgImageOptions.FitToViewPort property {#fittoviewport}

**Type:** boolean

### SvgImageOptions.CssPrefix property {#cssprefix}

**Type:** String

### SvgImageOptions.EmbeddedFontType property {#embeddedfonttype}

The value of the property is SvgEmbeddedFontType integer constant.

**Type:** Number

### SvgImageOptions.SaveFormat property {#saveformat}

Gets or sets the output file format type Support Tiff/XPS The value of the property is SaveFormat integer constant. NOTE: This member is now obsolete. Instead, For Tiff/Svg, use ImageType ; For Xps, use Workbook.save(java.lang.String, com.aspose.cells.SaveOptions) with XpsSaveOptions . This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### SvgImageOptions.PrintWithStatusDialog property {#printwithstatusdialog}

If PrintWithStatusDialog = true , there will be a dialog that shows current print status. else no such dialog will show.

**Type:** boolean

### SvgImageOptions.HorizontalResolution property {#horizontalresolution}

Gets or sets the horizontal resolution for generated images, in dots per inch. Applies generating image method except Emf format images. The default value is 96.

**Type:** Number

### SvgImageOptions.VerticalResolution property {#verticalresolution}

Gets or sets the vertical resolution for generated images, in dots per inch. Applies generating image method except Emf format image. The default value is 96.

**Type:** Number

### SvgImageOptions.TiffCompression property {#tiffcompression}

Gets or sets the type of compression to apply only when saving pages to the Tiff format. The value of the property is TiffCompression integer constant. Has effect only when saving to TIFF. The default value is Lzw.

**Type:** Number

### SvgImageOptions.TiffColorDepth property {#tiffcolordepth}

Gets or sets bit depth to apply only when saving pages to the Tiff format. The value of the property is ColorDepth integer constant. Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.

**Type:** Number

### SvgImageOptions.PrintingPage property {#printingpage}

Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant.

**Type:** Number

### SvgImageOptions.Quality property {#quality}

Gets or sets a value determining the quality of the generated images to apply only when saving pages to the Jpeg format. The default value is 100 Has effect only when saving to JPEG. The value must be between 0 and 100. The default value is 100.

**Type:** Number

### SvgImageOptions.IsCellAutoFit property {#iscellautofit}

Indicates whether the width and height of the cells is automatically fitted by cell value. The default value is false. NOTE: This member is now obsolete. Instead, please use Worksheet.autoFitColumns(com.aspose.cells.AutoFitterOptions) and Worksheet.autoFitRows(com.aspose.cells.AutoFitterOptions) . This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** boolean

### SvgImageOptions.OnePagePerSheet property {#onepagepersheet}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

**Type:** boolean

### SvgImageOptions.AllColumnsInOnePagePerSheet property {#allcolumnsinonepagepersheet}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

**Type:** boolean

### SvgImageOptions.DrawObjectEventHandler property {#drawobjecteventhandler}

Implements this interface to get DrawObject and Bound when rendering.

**Type:** DrawObjectEventHandler

### SvgImageOptions.ChartImageType property {#chartimagetype}

Indicate the chart imagetype when converting. default value: PNG. NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** ImageFormat

### SvgImageOptions.EmbededImageNameInSvg property {#embededimagenameinsvg}

Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded"

**Type:** String

### SvgImageOptions.SVGFitToViewPort property {#svgfittoviewport}

if this property is true, the generated svg will fit to view port.

**Type:** boolean

### SvgImageOptions.SvgCssPrefix property {#svgcssprefix}

**Type:** String

### SvgImageOptions.OnlyArea property {#onlyarea}

If this property is true , one Area will be output, and no scale will take effect.

**Type:** boolean

### SvgImageOptions.Transparent property {#transparent}

Indicates if the background of generated image should be transparent. The default value is false. That means the background of the generated images is white.

**Type:** boolean

### SvgImageOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### SvgImageOptions.PageSavingCallback property {#pagesavingcallback}

Control/Indicate progress of page saving process.

**Type:** IPageSavingCallback

### SvgImageOptions.IsFontSubstitutionCharGranularity property {#isfontsubstitutionchargranularity}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

**Type:** boolean

### SvgImageOptions.PageIndex property {#pageindex}

Gets or sets the 0-based index of the first page to save. Default is 0.

**Type:** Number

### SvgImageOptions.PageCount property {#pagecount}

Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.

**Type:** Number

### SvgImageOptions.IsOptimized property {#isoptimized}

Indicates whether to optimize the output elements. Default value is false. Currently when this property is set to true, the following optimizations will be done: 1. optimize the border lines. 2. optimize the file size while rendering to Svg image.

**Type:** boolean

### SvgImageOptions.DefaultFont property {#defaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

**Type:** String

### SvgImageOptions.CheckWorkbookDefaultFont property {#checkworkbookdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. Default is true.

**Type:** boolean

### SvgImageOptions.OutputBlankPageWhenNothingToPrint property {#outputblankpagewhennothingtoprint}

Indicates whether to output a blank page when there is nothing to print. Default is false.

**Type:** boolean

### SvgImageOptions.GridlineType property {#gridlinetype}

Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type.

**Type:** Number

### SvgImageOptions.GridlineColor property {#gridlinecolor}

**Type:** Color

### SvgImageOptions.TextCrossType property {#textcrosstype}

Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossType integer constant.

**Type:** Number

### SvgImageOptions.DefaultEditLanguage property {#defaulteditlanguage}

Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO .

**Type:** Number

### SvgImageOptions.SheetSet property {#sheetset}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible . The set is ignored when it is used in SheetRender

**Type:** SheetSet

### SvgImageOptions.EmfRenderSetting property {#emfrendersetting}

Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF_PLUS_PREFER is set, then EMF+ records will be parsed while rendering to image, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF_ONLY . For the frameworks that depend on .Net System.Drawing.Common, this setting is ignored.

**Type:** Number

### SvgImageOptions.CustomRenderSettings property {#customrendersettings}

**Type:** CustomRenderSettings

### getTiffPhotometricInterpretation() {#gettiffphotometricinterpretation}

Gets the type of PhotometricInterpretation to apply only when saving pages to the Tiff format.

Has effect only when saving to TIFF. The default value is -1, represent no PhotometricInterpretation is applied.

### setTiffPhotometricInterpretation(value) {#settiffphotometricinterpretation}

Sets the type of PhotometricInterpretation to apply only when saving pages to the Tiff format.

Has effect only when saving to TIFF. The default value is -1, represent no PhotometricInterpretation is applied.

### setRenderingHint(key, value) {#setrenderinghint}

Sets the value of a single preference for the rendering algorithms. Hint categories include controls for rendering quality and overall time/quality trade-off in the rendering process. Refer to the RenderingHints class for definitions of some common keys and values.

| Parameter | Type | Description |
| --- | --- | --- |
| key | Key | the key of the hint to be set. |
| value | Object | the value indicating preferences for the specified hint category. |

### setDesiredSize(desiredWidth, desiredHeight) (1 of 2) {#setdesiredsize}

Sets desired width and height of image.

NOTE: This member is now obsolete. Instead, please use setDesiredSize(int, int, boolean) by setting param keepAspectRatio to false. This property will be removed 12 months later since May 2023. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | Number | desired width in pixels |
| desiredHeight | Number | desired height in pixels |

---

### setDesiredSize(desiredWidth, desiredHeight, keepAspectRatio) (2 of 2) {#setdesiredsize-1}

Sets desired width and height of image.

| Parameter | Type | Description |
| --- | --- | --- |
| desiredWidth | Number | desired width in pixels |
| desiredHeight | Number | desired height in pixels |
| keepAspectRatio | boolean | whether to keep aspect ratio of origin image |
