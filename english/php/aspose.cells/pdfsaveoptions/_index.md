---
title: "PdfSaveOptions Class"
linktitle: "PdfSaveOptions"
articleTitle: "PdfSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the options for saving pdf file."
type: docs
weight: 4360
url: /php/aspose.cells/pdfsaveoptions/
---

## PdfSaveOptions class

Represents the options for saving pdf file.

## Constructors

| Name | Description |
| --- | --- |
| [PdfSaveOptions](#constructor) | Creates the options for saving pdf file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [EmbedStandardWindowsFonts](#embedstandardwindowsfonts) | boolean | True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are alwa |
| [Bookmark](#bookmark) | PdfBookmarkEntry | Gets and sets the PdfBookmarkEntry object. |
| [Compliance](#compliance) | Number | Gets or sets the PDF standards compliance level for output documents. The value of the property is PdfCompliance integer |
| [SecurityOptions](#securityoptions) | PdfSecurityOptions | Set this options, when security is need in xls2pdf result. |
| [ImageType](#imagetype) | ImageFormat | Represents the image type when converting the chart and shape . NOTE: This member is now obsolete. Instead, Chart and Sh |
| [CalculateFormula](#calculateformula) | boolean | Indicates whether to calculate formulas before saving pdf file. The default value is false. |
| [PdfCompression](#pdfcompression) | Number | Indicate the compression algorithm The value of the property is PdfCompressionCore integer constant. |
| [CreatedTime](#createdtime) | DateTime | Gets and sets the time of generating the pdf document. if it is not be set, it will be the time of generating the pdf. |
| [Producer](#producer) | String | Gets and sets producer of generated pdf document. If the value is null, or a valid LICENSE is not set, string Aspose.Cel |
| [OptimizationType](#optimizationtype) | Number | Gets and sets pdf optimization type. The value of the property is PdfOptimizationType integer constant. Default value is |
| [CustomPropertiesExport](#custompropertiesexport) | Number | Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is Non |
| [ExportDocumentStructure](#exportdocumentstructure) | boolean | Indicates whether to export document structure. |
| [DisplayDocTitle](#displaydoctitle) | boolean | Indicates whether the window's title bar should display the document title. If false, the title bar should instead displ |
| [FontEncoding](#fontencoding) | Number | Gets or sets embedded font encoding in pdf. The value of the property is PdfFontEncoding integer constant. Default value |
| [Watermark](#watermark) | RenderingWatermark | Gets or sets watermark to output. |
| [EmbedAttachments](#embedattachments) | boolean | Indicates whether to embed attachment for Ole objects in Excel. Default value is false. The value must be false when PDF |
| [ZoomBehavior](#zoombehavior) | Number | The value of the property is PdfZoomBehavior integer constant. |
| [ZoomFactor](#zoomfactor) | Number |  |
| [DefaultFont](#defaultfont) | String | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [CheckWorkbookDefaultFont](#checkworkbookdefaultfont) | boolean | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [CheckFontCompatibility](#checkfontcompatibility) | boolean | Indicates whether to check font compatibility for every character in text. The default value is true. Disable this prope |
| [IsFontSubstitutionCharGranularity](#isfontsubstitutionchargranularity) | boolean | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is fa |
| [OnePagePerSheet](#onepagepersheet) | boolean | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetu |
| [AllColumnsInOnePagePerSheet](#allcolumnsinonepagepersheet) | boolean | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The wid |
| [IgnoreError](#ignoreerror) | boolean | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [OutputBlankPageWhenNothingToPrint](#outputblankpagewhennothingtoprint) | boolean | Indicates whether to output a blank page when there is nothing to print. Default is true. |
| [PageIndex](#pageindex) | Number | Gets or sets the 0-based index of the first page to save. Default is 0. |
| [PageCount](#pagecount) | Number | Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.. |
| [PrintingPageType](#printingpagetype) | Number | Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in |
| [GridlineType](#gridlinetype) | Number | Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type. |
| [GridlineColor](#gridlinecolor) | Color |  |
| [TextCrossType](#textcrosstype) | Number | Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossT |
| [DefaultEditLanguage](#defaulteditlanguage) | Number | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [SheetSet](#sheetset) | SheetSet | Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible . |
| [DrawObjectEventHandler](#drawobjecteventhandler) | DrawObjectEventHandler | Implements this interface to get DrawObject and Bound when rendering. |
| [PageSavingCallback](#pagesavingcallback) | IPageSavingCallback | Control/Indicate progress of page saving process. |
| [EmfRenderSetting](#emfrendersetting) | Number | Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identi |
| [CustomRenderSettings](#customrendersettings) | CustomRenderSettings |  |
| [SaveFormat](#saveformat) | Number | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [ClearData](#cleardata) | boolean | Make the workbook empty after saving the file. |
| [CachedFileFolder](#cachedfilefolder) | String | The cached file folder is used to store some large data. |
| [ValidateMergedAreas](#validatemergedareas) | boolean | Indicates whether validate merged cells before saving the file. The default value is false. |
| [MergeAreas](#mergeareas) | boolean | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [CreateDirectory](#createdirectory) | boolean | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [SortNames](#sortnames) | boolean | Indicates whether sorting defined names before saving file. |
| [SortExternalNames](#sortexternalnames) | boolean | Indicates whether sorting external defined names before saving file. |
| [RefreshChartCache](#refreshchartcache) | boolean | Indicates whether refreshing chart cache data |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean |  |
| [UpdateSmartArt](#updatesmartart) | boolean | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [EncryptDocumentProperties](#encryptdocumentproperties) | boolean |  |

## Methods

| Name | Description |
| --- | --- |
| [setImageResample](#setimageresample) | Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the spe |

### PdfSaveOptions() {#constructor}

Creates the options for saving pdf file.

### PdfSaveOptions.EmbedStandardWindowsFonts property {#embedstandardwindowsfonts}

True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.

**Type:** boolean

### PdfSaveOptions.Bookmark property {#bookmark}

Gets and sets the PdfBookmarkEntry object.

**Type:** PdfBookmarkEntry

### PdfSaveOptions.Compliance property {#compliance}

Gets or sets the PDF standards compliance level for output documents. The value of the property is PdfCompliance integer constant. Default is Pdf17.

**Type:** Number

### PdfSaveOptions.SecurityOptions property {#securityoptions}

Set this options, when security is need in xls2pdf result.

**Type:** PdfSecurityOptions

### PdfSaveOptions.ImageType property {#imagetype}

Represents the image type when converting the chart and shape . NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

**Type:** ImageFormat

### PdfSaveOptions.CalculateFormula property {#calculateformula}

Indicates whether to calculate formulas before saving pdf file. The default value is false.

**Type:** boolean

### PdfSaveOptions.PdfCompression property {#pdfcompression}

Indicate the compression algorithm The value of the property is PdfCompressionCore integer constant.

**Type:** Number

### PdfSaveOptions.CreatedTime property {#createdtime}

Gets and sets the time of generating the pdf document. if it is not be set, it will be the time of generating the pdf.

**Type:** DateTime

### PdfSaveOptions.Producer property {#producer}

Gets and sets producer of generated pdf document. If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.

**Type:** String

### PdfSaveOptions.OptimizationType property {#optimizationtype}

Gets and sets pdf optimization type. The value of the property is PdfOptimizationType integer constant. Default value is PdfOptimizationType.STANDARD

**Type:** Number

### PdfSaveOptions.CustomPropertiesExport property {#custompropertiesexport}

Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is None. The value of the property is PdfCustomPropertiesExport integer constant.

**Type:** Number

### PdfSaveOptions.ExportDocumentStructure property {#exportdocumentstructure}

Indicates whether to export document structure.

**Type:** boolean

### PdfSaveOptions.DisplayDocTitle property {#displaydoctitle}

Indicates whether the window's title bar should display the document title. If false, the title bar should instead display the name of the PDF file. Default value is false.

**Type:** boolean

### PdfSaveOptions.FontEncoding property {#fontencoding}

Gets or sets embedded font encoding in pdf. The value of the property is PdfFontEncoding integer constant. Default value is PdfFontEncoding.IDENTITY

**Type:** Number

### PdfSaveOptions.Watermark property {#watermark}

Gets or sets watermark to output.

**Type:** RenderingWatermark

### PdfSaveOptions.EmbedAttachments property {#embedattachments}

Indicates whether to embed attachment for Ole objects in Excel. Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.

**Type:** boolean

### PdfSaveOptions.ZoomBehavior property {#zoombehavior}

The value of the property is PdfZoomBehavior integer constant.

**Type:** Number

### PdfSaveOptions.ZoomFactor property {#zoomfactor}

**Type:** Number

### PdfSaveOptions.DefaultFont property {#defaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

**Type:** String

### PdfSaveOptions.CheckWorkbookDefaultFont property {#checkworkbookdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. Default is true.

**Type:** boolean

### PdfSaveOptions.CheckFontCompatibility property {#checkfontcompatibility}

Indicates whether to check font compatibility for every character in text. The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

**Type:** boolean

### PdfSaveOptions.IsFontSubstitutionCharGranularity property {#isfontsubstitutionchargranularity}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

**Type:** boolean

### PdfSaveOptions.OnePagePerSheet property {#onepagepersheet}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

**Type:** boolean

### PdfSaveOptions.AllColumnsInOnePagePerSheet property {#allcolumnsinonepagepersheet}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

**Type:** boolean

### PdfSaveOptions.IgnoreError property {#ignoreerror}

Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

**Type:** boolean

### PdfSaveOptions.OutputBlankPageWhenNothingToPrint property {#outputblankpagewhennothingtoprint}

Indicates whether to output a blank page when there is nothing to print. Default is true.

**Type:** boolean

### PdfSaveOptions.PageIndex property {#pageindex}

Gets or sets the 0-based index of the first page to save. Default is 0.

**Type:** Number

### PdfSaveOptions.PageCount property {#pagecount}

Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered..

**Type:** Number

### PdfSaveOptions.PrintingPageType property {#printingpagetype}

Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.

**Type:** Number

### PdfSaveOptions.GridlineType property {#gridlinetype}

Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type.

**Type:** Number

### PdfSaveOptions.GridlineColor property {#gridlinecolor}

**Type:** Color

### PdfSaveOptions.TextCrossType property {#textcrosstype}

Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossType integer constant.

**Type:** Number

### PdfSaveOptions.DefaultEditLanguage property {#defaulteditlanguage}

Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO .

**Type:** Number

### PdfSaveOptions.SheetSet property {#sheetset}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible .

**Type:** SheetSet

### PdfSaveOptions.DrawObjectEventHandler property {#drawobjecteventhandler}

Implements this interface to get DrawObject and Bound when rendering.

**Type:** DrawObjectEventHandler

### PdfSaveOptions.PageSavingCallback property {#pagesavingcallback}

Control/Indicate progress of page saving process.

**Type:** IPageSavingCallback

### PdfSaveOptions.EmfRenderSetting property {#emfrendersetting}

Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF_PLUS_PREFER is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF_ONLY .

**Type:** Number

### PdfSaveOptions.CustomRenderSettings property {#customrendersettings}

**Type:** CustomRenderSettings

### PdfSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### PdfSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### PdfSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### PdfSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### PdfSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### PdfSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### PdfSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### PdfSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### PdfSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### PdfSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### PdfSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### PdfSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean

### setImageResample(desiredPPI, jpegQuality) {#setimageresample}

Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled.

| Parameter | Type | Description |
| --- | --- | --- |
| desiredPPI | Number | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpegQuality | Number | 0 - 100% JPEG quality. |
