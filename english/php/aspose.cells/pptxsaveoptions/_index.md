---
title: "PptxSaveOptions Class"
linktitle: "PptxSaveOptions"
articleTitle: "PptxSaveOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the pptx save options."
type: docs
weight: 5050
url: /php/aspose.cells/pptxsaveoptions/
---

## PptxSaveOptions class

Represents the pptx save options.

## Constructors

| Name | Description |
| --- | --- |
| [PptxSaveOptions](#constructor) | Represents the pptx save options. |
| [PptxSaveOptions](#constructor) | Represents options of saving .pptx file. |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IgnoreHiddenRows](#ignorehiddenrows) | boolean | Inidicates whether ignoring hidden rows when converting Excel to PowerPoint. |
| [SaveAsEditableShapes](#saveaseditableshapes) | boolean |  |
| [EmbedXlsxAsChartDataSource](#embedxlsxaschartdatasource) | boolean |  |
| [AdjustFontSizeForRowType](#adjustfontsizeforrowtype) | Number | Represents what type of line needs to be adjusted size of font if height of row is small. The value of the property is A |
| [ExportViewType](#exportviewtype) | Number | Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing. The valu |
| [AsFlatOpc](#asflatopc) | boolean |  |
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
| [WarningCallback](#warningcallback) | IWarningCallback | Gets or sets warning callback. |
| [CheckExcelRestriction](#checkexcelrestriction) | boolean |  |
| [UpdateSmartArt](#updatesmartart) | boolean | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [EncryptDocumentProperties](#encryptdocumentproperties) | boolean |  |

### PptxSaveOptions() (1 of 2) {#constructor}

Represents the pptx save options.

---

### PptxSaveOptions(saveAsImage) (2 of 2) {#constructor-1}

Represents options of saving .pptx file.

| Parameter | Type | Description |
| --- | --- | --- |
| saveAsImage | boolean | If True, the workbook will be converted into some pictures of .pptx file. If False, the workbook will be converted into some tables of .pptx file. |

### PptxSaveOptions.IgnoreHiddenRows property {#ignorehiddenrows}

Inidicates whether ignoring hidden rows when converting Excel to PowerPoint.

**Type:** boolean

### PptxSaveOptions.SaveAsEditableShapes property {#saveaseditableshapes}

**Type:** boolean

### PptxSaveOptions.EmbedXlsxAsChartDataSource property {#embedxlsxaschartdatasource}

**Type:** boolean

### PptxSaveOptions.AdjustFontSizeForRowType property {#adjustfontsizeforrowtype}

Represents what type of line needs to be adjusted size of font if height of row is small. The value of the property is AdjustFontSizeForRowType integer constant.

**Type:** Number

### PptxSaveOptions.ExportViewType property {#exportviewtype}

Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing. The value of the property is SlideViewType integer constant.

**Type:** Number

### PptxSaveOptions.AsFlatOpc property {#asflatopc}

**Type:** boolean

### PptxSaveOptions.DefaultFont property {#defaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

**Type:** String

### PptxSaveOptions.CheckWorkbookDefaultFont property {#checkworkbookdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. Default is true.

**Type:** boolean

### PptxSaveOptions.CheckFontCompatibility property {#checkfontcompatibility}

Indicates whether to check font compatibility for every character in text. The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

**Type:** boolean

### PptxSaveOptions.IsFontSubstitutionCharGranularity property {#isfontsubstitutionchargranularity}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

**Type:** boolean

### PptxSaveOptions.OnePagePerSheet property {#onepagepersheet}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

**Type:** boolean

### PptxSaveOptions.AllColumnsInOnePagePerSheet property {#allcolumnsinonepagepersheet}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

**Type:** boolean

### PptxSaveOptions.IgnoreError property {#ignoreerror}

Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

**Type:** boolean

### PptxSaveOptions.OutputBlankPageWhenNothingToPrint property {#outputblankpagewhennothingtoprint}

Indicates whether to output a blank page when there is nothing to print. Default is true.

**Type:** boolean

### PptxSaveOptions.PageIndex property {#pageindex}

Gets or sets the 0-based index of the first page to save. Default is 0.

**Type:** Number

### PptxSaveOptions.PageCount property {#pagecount}

Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered..

**Type:** Number

### PptxSaveOptions.PrintingPageType property {#printingpagetype}

Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.

**Type:** Number

### PptxSaveOptions.GridlineType property {#gridlinetype}

Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type.

**Type:** Number

### PptxSaveOptions.GridlineColor property {#gridlinecolor}

**Type:** Color

### PptxSaveOptions.TextCrossType property {#textcrosstype}

Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossType integer constant.

**Type:** Number

### PptxSaveOptions.DefaultEditLanguage property {#defaulteditlanguage}

Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO .

**Type:** Number

### PptxSaveOptions.SheetSet property {#sheetset}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible .

**Type:** SheetSet

### PptxSaveOptions.DrawObjectEventHandler property {#drawobjecteventhandler}

Implements this interface to get DrawObject and Bound when rendering.

**Type:** DrawObjectEventHandler

### PptxSaveOptions.PageSavingCallback property {#pagesavingcallback}

Control/Indicate progress of page saving process.

**Type:** IPageSavingCallback

### PptxSaveOptions.EmfRenderSetting property {#emfrendersetting}

Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF_PLUS_PREFER is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF_ONLY .

**Type:** Number

### PptxSaveOptions.CustomRenderSettings property {#customrendersettings}

**Type:** CustomRenderSettings

### PptxSaveOptions.SaveFormat property {#saveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

**Type:** Number

### PptxSaveOptions.ClearData property {#cleardata}

Make the workbook empty after saving the file.

**Type:** boolean

### PptxSaveOptions.CachedFileFolder property {#cachedfilefolder}

The cached file folder is used to store some large data.

**Type:** String

### PptxSaveOptions.ValidateMergedAreas property {#validatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

**Type:** boolean

### PptxSaveOptions.MergeAreas property {#mergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

**Type:** boolean

### PptxSaveOptions.CreateDirectory property {#createdirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Type:** boolean

### PptxSaveOptions.SortNames property {#sortnames}

Indicates whether sorting defined names before saving file.

**Type:** boolean

### PptxSaveOptions.SortExternalNames property {#sortexternalnames}

Indicates whether sorting external defined names before saving file.

**Type:** boolean

### PptxSaveOptions.RefreshChartCache property {#refreshchartcache}

Indicates whether refreshing chart cache data

**Type:** boolean

### PptxSaveOptions.WarningCallback property {#warningcallback}

Gets or sets warning callback.

**Type:** IWarningCallback

### PptxSaveOptions.CheckExcelRestriction property {#checkexcelrestriction}

**Type:** boolean

### PptxSaveOptions.UpdateSmartArt property {#updatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Type:** boolean

### PptxSaveOptions.EncryptDocumentProperties property {#encryptdocumentproperties}

**Type:** boolean
