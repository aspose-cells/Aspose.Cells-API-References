---
title: "PdfSaveOptions"
linktitle: "PdfSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the options for saving pdf file."
type: docs
weight: 2590
url: /nodejs/aspose.cells/pdfsaveoptions/
---

## PdfSaveOptions class

Represents the options for saving pdf file.

```js
new PdfSaveOptions()
```

Creates the options for saving pdf file.

## Methods

| Name | Description |
| --- | --- |
| [getAllColumnsInOnePagePerSheet()](#getallcolumnsinonepagepersheet) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The wid |
| [getBookmark()](#getbookmark) | Gets and sets the PdfBookmarkEntry object. |
| [getCachedFileFolder()](#getcachedfilefolder) | The cached file folder is used to store some large data. |
| [getCalculateFormula()](#getcalculateformula) | Indicates whether to calculate formulas before saving pdf file. The default value is false. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) |  |
| [getCheckFontCompatibility()](#getcheckfontcompatibility) | Indicates whether to check font compatibility for every character in text. The default value is true. Disable this prope |
| [getCheckWorkbookDefaultFont()](#getcheckworkbookdefaultfont) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [getClearData()](#getcleardata) | Make the workbook empty after saving the file. |
| [getCompliance()](#getcompliance) | Gets or sets the PDF standards compliance level for output documents. The value of the property is PdfCompliance integer |
| [getCreateDirectory()](#getcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getCreatedTime()](#getcreatedtime) | Gets and sets the time of generating the pdf document. if it is not be set, it will be the time of generating the pdf. |
| [getCustomPropertiesExport()](#getcustompropertiesexport) | Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is Non |
| [getCustomRenderSettings()](#getcustomrendersettings) |  |
| [getDefaultEditLanguage()](#getdefaulteditlanguage) | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [getDefaultFont()](#getdefaultfont) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [getDisplayDocTitle()](#getdisplaydoctitle) | Indicates whether the window's title bar should display the document title. If false, the title bar should instead displ |
| [getDrawObjectEventHandler()](#getdrawobjecteventhandler) | Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbedAttachments()](#getembedattachments) | Indicates whether to embed attachment for Ole objects in Excel. Default value is false. The value must be false when PDF |
| [getEmbedStandardWindowsFonts()](#getembedstandardwindowsfonts) | True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are alwa |
| [getEmfRenderSetting()](#getemfrendersetting) | Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identi |
| [getEncryptDocumentProperties()](#getencryptdocumentproperties) |  |
| [getExportDocumentStructure()](#getexportdocumentstructure) | Indicates whether to export document structure. |
| [getFontEncoding()](#getfontencoding) | Gets or sets embedded font encoding in pdf. The value of the property is PdfFontEncoding integer constant. Default value |
| [getGridlineColor()](#getgridlinecolor) |  |
| [getGridlineType()](#getgridlinetype) | Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type. |
| [getIgnoreError()](#getignoreerror) | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [getImageType()](#getimagetype) | Represents the image type when converting the chart and shape . NOTE: This member is now obsolete. Instead, Chart and Sh |
| [getMergeAreas()](#getmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getOnePagePerSheet()](#getonepagepersheet) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetu |
| [getOptimizationType()](#getoptimizationtype) | Gets and sets pdf optimization type. The value of the property is PdfOptimizationType integer constant. Default value is |
| [getOutputBlankPageWhenNothingToPrint()](#getoutputblankpagewhennothingtoprint) | Indicates whether to output a blank page when there is nothing to print. Default is true. |
| [getPageCount()](#getpagecount) | Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.. |
| [getPageIndex()](#getpageindex) | Gets or sets the 0-based index of the first page to save. Default is 0. |
| [getPageSavingCallback()](#getpagesavingcallback) | Control/Indicate progress of page saving process. |
| [getPdfCompression()](#getpdfcompression) | Indicate the compression algorithm The value of the property is PdfCompressionCore integer constant. |
| [getPrintingPageType()](#getprintingpagetype) | Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in |
| [getProducer()](#getproducer) | Gets and sets producer of generated pdf document. If the value is null, or a valid LICENSE is not set, string Aspose.Cel |
| [getRefreshChartCache()](#getrefreshchartcache) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getsaveformat) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSecurityOptions()](#getsecurityoptions) | Set this options, when security is need in xls2pdf result. |
| [getSheetSet()](#getsheetset) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible. |
| [getSortExternalNames()](#getsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getsortnames) | Indicates whether sorting defined names before saving file. |
| [getTextCrossType()](#gettextcrosstype) | Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossT |
| [getUpdateSmartArt()](#getupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getValidateMergedAreas()](#getvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [getWatermark()](#getwatermark) | Gets or sets watermark to output. |
| [getZoomBehavior()](#getzoombehavior) | The value of the property is PdfZoomBehavior integer constant. |
| [getZoomFactor()](#getzoomfactor) |  |
| [isFontSubstitutionCharGranularity()](#isfontsubstitutionchargranularity) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is fa |
| [setAllColumnsInOnePagePerSheet()](#setallcolumnsinonepagepersheet) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The wid |
| [setBookmark()](#setbookmark) | Gets and sets the PdfBookmarkEntry object. |
| [setCachedFileFolder()](#setcachedfilefolder) | The cached file folder is used to store some large data. |
| [setCalculateFormula()](#setcalculateformula) | Indicates whether to calculate formulas before saving pdf file. The default value is false. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) |  |
| [setCheckFontCompatibility()](#setcheckfontcompatibility) | Indicates whether to check font compatibility for every character in text. The default value is true. Disable this prope |
| [setCheckWorkbookDefaultFont()](#setcheckworkbookdefaultfont) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [setClearData()](#setcleardata) | Make the workbook empty after saving the file. |
| [setCompliance()](#setcompliance) | Gets or sets the PDF standards compliance level for output documents. The value of the property is PdfCompliance integer |
| [setCreateDirectory()](#setcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setCreatedTime()](#setcreatedtime) | Gets and sets the time of generating the pdf document. if it is not be set, it will be the time of generating the pdf. |
| [setCustomPropertiesExport()](#setcustompropertiesexport) | Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is Non |
| [setCustomRenderSettings()](#setcustomrendersettings) |  |
| [setDefaultEditLanguage()](#setdefaulteditlanguage) | Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/re |
| [setDefaultFont()](#setdefaultfont) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf |
| [setDisplayDocTitle()](#setdisplaydoctitle) | Indicates whether the window's title bar should display the document title. If false, the title bar should instead displ |
| [setDrawObjectEventHandler()](#setdrawobjecteventhandler) | Implements this interface to get DrawObject and Bound when rendering. |
| [setEmbedAttachments()](#setembedattachments) | Indicates whether to embed attachment for Ole objects in Excel. Default value is false. The value must be false when PDF |
| [setEmbedStandardWindowsFonts()](#setembedstandardwindowsfonts) | True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are alwa |
| [setEmfRenderSetting()](#setemfrendersetting) | Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identi |
| [setEncryptDocumentProperties()](#setencryptdocumentproperties) |  |
| [setExportDocumentStructure()](#setexportdocumentstructure) | Indicates whether to export document structure. |
| [setFontEncoding()](#setfontencoding) | Gets or sets embedded font encoding in pdf. The value of the property is PdfFontEncoding integer constant. Default value |
| [setFontSubstitutionCharGranularity()](#setfontsubstitutionchargranularity) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is fa |
| [setGridlineColor()](#setgridlinecolor) |  |
| [setGridlineType()](#setgridlinetype) | Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type. |
| [setIgnoreError()](#setignoreerror) | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [setImageResample(desiredPPI, jpegQuality)](#setimageresample) | Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the spe |
| [setImageType()](#setimagetype) | Represents the image type when converting the chart and shape . NOTE: This member is now obsolete. Instead, Chart and Sh |
| [setMergeAreas()](#setmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setOnePagePerSheet()](#setonepagepersheet) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetu |
| [setOptimizationType()](#setoptimizationtype) | Gets and sets pdf optimization type. The value of the property is PdfOptimizationType integer constant. Default value is |
| [setOutputBlankPageWhenNothingToPrint()](#setoutputblankpagewhennothingtoprint) | Indicates whether to output a blank page when there is nothing to print. Default is true. |
| [setPageCount()](#setpagecount) | Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered.. |
| [setPageIndex()](#setpageindex) | Gets or sets the 0-based index of the first page to save. Default is 0. |
| [setPageSavingCallback()](#setpagesavingcallback) | Control/Indicate progress of page saving process. |
| [setPdfCompression()](#setpdfcompression) | Indicate the compression algorithm The value of the property is PdfCompressionCore integer constant. |
| [setPrintingPageType()](#setprintingpagetype) | Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in |
| [setProducer()](#setproducer) | Gets and sets producer of generated pdf document. If the value is null, or a valid LICENSE is not set, string Aspose.Cel |
| [setRefreshChartCache()](#setrefreshchartcache) | Indicates whether refreshing chart cache data |
| [setSecurityOptions()](#setsecurityoptions) | Set this options, when security is need in xls2pdf result. |
| [setSheetSet()](#setsheetset) | Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible. |
| [setSortExternalNames()](#setsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](#setsortnames) | Indicates whether sorting defined names before saving file. |
| [setTextCrossType()](#settextcrosstype) | Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossT |
| [setUpdateSmartArt()](#setupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setValidateMergedAreas()](#setvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setWatermark()](#setwatermark) | Gets or sets watermark to output. |
| [setZoomBehavior()](#setzoombehavior) | The value of the property is PdfZoomBehavior integer constant. |
| [setZoomFactor()](#setzoomfactor) |  |

### getAllColumnsInOnePagePerSheet() {#getallcolumnsinonepagepersheet}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

### getBookmark() {#getbookmark}

Gets and sets the PdfBookmarkEntry object.

### getCachedFileFolder() {#getcachedfilefolder}

The cached file folder is used to store some large data.

### getCalculateFormula() {#getcalculateformula}

Indicates whether to calculate formulas before saving pdf file. The default value is false.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

### getCheckFontCompatibility() {#getcheckfontcompatibility}

Indicates whether to check font compatibility for every character in text. The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

### getCheckWorkbookDefaultFont() {#getcheckworkbookdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. Default is true.

### getClearData() {#getcleardata}

Make the workbook empty after saving the file.

### getCompliance() {#getcompliance}

Gets or sets the PDF standards compliance level for output documents. The value of the property is PdfCompliance integer constant. Default is Pdf17.

### getCreateDirectory() {#getcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### getCreatedTime() {#getcreatedtime}

Gets and sets the time of generating the pdf document. if it is not be set, it will be the time of generating the pdf.

### getCustomPropertiesExport() {#getcustompropertiesexport}

Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is None. The value of the property is PdfCustomPropertiesExport integer constant.

### getCustomRenderSettings() {#getcustomrendersettings}

### getDefaultEditLanguage() {#getdefaulteditlanguage}

Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO.

### getDefaultFont() {#getdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

### getDisplayDocTitle() {#getdisplaydoctitle}

Indicates whether the window's title bar should display the document title. If false, the title bar should instead display the name of the PDF file. Default value is false.

### getDrawObjectEventHandler() {#getdrawobjecteventhandler}

Implements this interface to get DrawObject and Bound when rendering.

### getEmbedAttachments() {#getembedattachments}

Indicates whether to embed attachment for Ole objects in Excel. Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.

### getEmbedStandardWindowsFonts() {#getembedstandardwindowsfonts}

True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.

### getEmfRenderSetting() {#getemfrendersetting}

Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF_PLUS_PREFER is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF_ONLY.

### getEncryptDocumentProperties() {#getencryptdocumentproperties}

### getExportDocumentStructure() {#getexportdocumentstructure}

Indicates whether to export document structure.

### getFontEncoding() {#getfontencoding}

Gets or sets embedded font encoding in pdf. The value of the property is PdfFontEncoding integer constant. Default value is PdfFontEncoding.IDENTITY

### getGridlineColor() {#getgridlinecolor}

### getGridlineType() {#getgridlinetype}

Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type.

### getIgnoreError() {#getignoreerror}

Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

### getImageType() {#getimagetype}

Represents the image type when converting the chart and shape . NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### getMergeAreas() {#getmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### getOnePagePerSheet() {#getonepagepersheet}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

### getOptimizationType() {#getoptimizationtype}

Gets and sets pdf optimization type. The value of the property is PdfOptimizationType integer constant. Default value is PdfOptimizationType.STANDARD

### getOutputBlankPageWhenNothingToPrint() {#getoutputblankpagewhennothingtoprint}

Indicates whether to output a blank page when there is nothing to print. Default is true.

### getPageCount() {#getpagecount}

Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered..

### getPageIndex() {#getpageindex}

Gets or sets the 0-based index of the first page to save. Default is 0.

### getPageSavingCallback() {#getpagesavingcallback}

Control/Indicate progress of page saving process.

### getPdfCompression() {#getpdfcompression}

Indicate the compression algorithm The value of the property is PdfCompressionCore integer constant.

### getPrintingPageType() {#getprintingpagetype}

Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.

### getProducer() {#getproducer}

Gets and sets producer of generated pdf document. If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.

### getRefreshChartCache() {#getrefreshchartcache}

Indicates whether refreshing chart cache data

### getSaveFormat() {#getsaveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

### getSecurityOptions() {#getsecurityoptions}

Set this options, when security is need in xls2pdf result.

### getSheetSet() {#getsheetset}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible.

### getSortExternalNames() {#getsortexternalnames}

Indicates whether sorting external defined names before saving file.

### getSortNames() {#getsortnames}

Indicates whether sorting defined names before saving file.

### getTextCrossType() {#gettextcrosstype}

Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossType integer constant.

### getUpdateSmartArt() {#getupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getValidateMergedAreas() {#getvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### getWatermark() {#getwatermark}

Gets or sets watermark to output.

### getZoomBehavior() {#getzoombehavior}

The value of the property is PdfZoomBehavior integer constant.

### getZoomFactor() {#getzoomfactor}

### isFontSubstitutionCharGranularity() {#isfontsubstitutionchargranularity}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### setAllColumnsInOnePagePerSheet() {#setallcolumnsinonepagepersheet}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

### setBookmark() {#setbookmark}

Gets and sets the PdfBookmarkEntry object.

### setCachedFileFolder() {#setcachedfilefolder}

The cached file folder is used to store some large data.

### setCalculateFormula() {#setcalculateformula}

Indicates whether to calculate formulas before saving pdf file. The default value is false.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

### setCheckFontCompatibility() {#setcheckfontcompatibility}

Indicates whether to check font compatibility for every character in text. The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

### setCheckWorkbookDefaultFont() {#setcheckworkbookdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. Default is true.

### setClearData() {#setcleardata}

Make the workbook empty after saving the file.

### setCompliance() {#setcompliance}

Gets or sets the PDF standards compliance level for output documents. The value of the property is PdfCompliance integer constant. Default is Pdf17.

### setCreateDirectory() {#setcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### setCreatedTime() {#setcreatedtime}

Gets and sets the time of generating the pdf document. if it is not be set, it will be the time of generating the pdf.

### setCustomPropertiesExport() {#setcustompropertiesexport}

Gets or sets a value determining the way CustomDocumentPropertyCollection are exported to PDF file. Default value is None. The value of the property is PdfCustomPropertiesExport integer constant.

### setCustomRenderSettings() {#setcustomrendersettings}

### setDefaultEditLanguage() {#setdefaulteditlanguage}

Gets or sets default edit language. The value of the property is DefaultEditLanguage integer constant. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO.

### setDefaultFont() {#setdefaultfont}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

### setDisplayDocTitle() {#setdisplaydoctitle}

Indicates whether the window's title bar should display the document title. If false, the title bar should instead display the name of the PDF file. Default value is false.

### setDrawObjectEventHandler() {#setdrawobjecteventhandler}

Implements this interface to get DrawObject and Bound when rendering.

### setEmbedAttachments() {#setembedattachments}

Indicates whether to embed attachment for Ole objects in Excel. Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.

### setEmbedStandardWindowsFonts() {#setembedstandardwindowsfonts}

True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.

### setEmfRenderSetting() {#setemfrendersetting}

Setting for rendering Emf metafile. The value of the property is EmfRenderSetting integer constant. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF_PLUS_PREFER is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF_ONLY.

### setEncryptDocumentProperties() {#setencryptdocumentproperties}

### setExportDocumentStructure() {#setexportdocumentstructure}

Indicates whether to export document structure.

### setFontEncoding() {#setfontencoding}

Gets or sets embedded font encoding in pdf. The value of the property is PdfFontEncoding integer constant. Default value is PdfFontEncoding.IDENTITY

### setFontSubstitutionCharGranularity() {#setfontsubstitutionchargranularity}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### setGridlineColor() {#setgridlinecolor}

### setGridlineType() {#setgridlinetype}

Gets or sets gridline type. The value of the property is GridlineType integer constant. Default is Dotted type.

### setIgnoreError() {#setignoreerror}

Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

### setImageResample(desiredPPI, jpegQuality) {#setimageresample}

Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled.

| Parameter | Type | Description |
| --- | --- | --- |
| desiredPPI | Number | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpegQuality | Number | 0 - 100% JPEG quality. |

### setImageType() {#setimagetype}

Represents the image type when converting the chart and shape . NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

### setMergeAreas() {#setmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### setOnePagePerSheet() {#setonepagepersheet}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

### setOptimizationType() {#setoptimizationtype}

Gets and sets pdf optimization type. The value of the property is PdfOptimizationType integer constant. Default value is PdfOptimizationType.STANDARD

### setOutputBlankPageWhenNothingToPrint() {#setoutputblankpagewhennothingtoprint}

Indicates whether to output a blank page when there is nothing to print. Default is true.

### setPageCount() {#setpagecount}

Gets or sets the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered..

### setPageIndex() {#setpageindex}

Gets or sets the 0-based index of the first page to save. Default is 0.

### setPageSavingCallback() {#setpagesavingcallback}

Control/Indicate progress of page saving process.

### setPdfCompression() {#setpdfcompression}

Indicate the compression algorithm The value of the property is PdfCompressionCore integer constant.

### setPrintingPageType() {#setprintingpagetype}

Indicates which pages will not be printed. The value of the property is PrintingPageType integer constant. If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.

### setProducer() {#setproducer}

Gets and sets producer of generated pdf document. If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.

### setRefreshChartCache() {#setrefreshchartcache}

Indicates whether refreshing chart cache data

### setSecurityOptions() {#setsecurityoptions}

Set this options, when security is need in xls2pdf result.

### setSheetSet() {#setsheetset}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: SheetSet.Visible.

### setSortExternalNames() {#setsortexternalnames}

Indicates whether sorting external defined names before saving file.

### setSortNames() {#setsortnames}

Indicates whether sorting defined names before saving file.

### setTextCrossType() {#settextcrosstype}

Gets or sets displaying text type when the text width is larger than cell width. The value of the property is TextCrossType integer constant.

### setUpdateSmartArt() {#setupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setValidateMergedAreas() {#setvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### setWatermark() {#setwatermark}

Gets or sets watermark to output.

### setZoomBehavior() {#setzoombehavior}

The value of the property is PdfZoomBehavior integer constant.

### setZoomFactor() {#setzoomfactor}
