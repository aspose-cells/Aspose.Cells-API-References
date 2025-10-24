##PdfSaveOptions
Represents the options for saving pdf file.
## PdfSaveOptions class
Represents the options for saving pdf file.
```javascript
class PdfSaveOptions extends PaginatedSaveOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options for saving pdf file. |
| [constructor(PaginatedSaveOptions)](#constructor-paginatedsaveoptions-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [embedStandardWindowsFonts](#embedStandardWindowsFonts--)| boolean | True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true. |
| [bookmark](#bookmark--)| PdfBookmarkEntry | Gets and sets the <see cref ="PdfBookmarkEntry">PdfBookmarkEntry</see> object. |
| [compliance](#compliance--)| PdfCompliance | Gets or sets the PDF standards compliance level for output documents. |
| [securityOptions](#securityOptions--)| PdfSecurityOptions | Set this options, when security is need in xls2pdf result. |
| [calculateFormula](#calculateFormula--)| boolean | Indicates whether to calculate formulas before saving pdf file. |
| [pdfCompression](#pdfCompression--)| PdfCompressionCore | Indicate the compression algorithm |
| [createdTime](#createdTime--)| Date | Gets and sets the time of generating the pdf document. |
| [producer](#producer--)| string | Gets and sets producer of generated pdf document. |
| [optimizationType](#optimizationType--)| PdfOptimizationType | Gets and sets pdf optimization type. |
| [customPropertiesExport](#customPropertiesExport--)| PdfCustomPropertiesExport | Gets or sets a value determining the way [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) are exported to PDF file. Default value is None. |
| [exportDocumentStructure](#exportDocumentStructure--)| boolean | Indicates whether to export document structure. |
| [displayDocTitle](#displayDocTitle--)| boolean | Indicates whether the window's title bar should display the document title. |
| [fontEncoding](#fontEncoding--)| PdfFontEncoding | Gets or sets embedded font encoding in pdf. |
| [watermark](#watermark--)| RenderingWatermark | Gets or sets watermark to output. |
| [embedAttachments](#embedAttachments--)| boolean | Indicates whether to embed attachment for Ole objects in Excel. |
| [saveFormat](#saveFormat--)| SaveFormat | Readonly. Gets the save file format. |
| [clearData](#clearData--)| boolean | Make the workbook empty after saving the file. |
| [cachedFileFolder](#cachedFileFolder--)| string | The folder for temporary files that may be used as data cache. |
| [validateMergedAreas](#validateMergedAreas--)| boolean | Indicates whether validate merged cells before saving the file. |
| [mergeAreas](#mergeAreas--)| boolean | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [createDirectory](#createDirectory--)| boolean | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [sortNames](#sortNames--)| boolean | Indicates whether sorting defined names before saving file. |
| [sortExternalNames](#sortExternalNames--)| boolean | Indicates whether sorting external defined names before saving file. |
| [refreshChartCache](#refreshChartCache--)| boolean | Indicates whether refreshing chart cache data |
| [warningCallback](#warningCallback--)| IWarningCallback | Gets or sets warning callback. |
| [checkExcelRestriction](#checkExcelRestriction--)| boolean | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [updateSmartArt](#updateSmartArt--)| boolean | Indicates whether updating smart art setting. The default value is false. |
| [encryptDocumentProperties](#encryptDocumentProperties--)| boolean | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [defaultFont](#defaultFont--)| string | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [checkWorkbookDefaultFont](#checkWorkbookDefaultFont--)| boolean | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [checkFontCompatibility](#checkFontCompatibility--)| boolean | Indicates whether to check font compatibility for every character in text. |
| [isFontSubstitutionCharGranularity](#isFontSubstitutionCharGranularity--)| boolean | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [onePagePerSheet](#onePagePerSheet--)| boolean | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [allColumnsInOnePagePerSheet](#allColumnsInOnePagePerSheet--)| boolean | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect. |
| [ignoreError](#ignoreError--)| boolean | Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [outputBlankPageWhenNothingToPrint](#outputBlankPageWhenNothingToPrint--)| boolean | Indicates whether to output a blank page when there is nothing to print. |
| [pageIndex](#pageIndex--)| number | Gets or sets the 0-based index of the first page to save. |
| [pageCount](#pageCount--)| number | Gets or sets the number of pages to save. |
| [printingPageType](#printingPageType--)| PrintingPageType | Indicates which pages will not be printed. |
| [gridlineType](#gridlineType--)| GridlineType | Gets or sets gridline type. |
| [gridlineColor](#gridlineColor--)| Color | Gets or sets gridline color. |
| [textCrossType](#textCrossType--)| TextCrossType | Gets or sets displaying text type when the text width is larger than cell width. |
| [defaultEditLanguage](#defaultEditLanguage--)| DefaultEditLanguage | Gets or sets default edit language. |
| [sheetSet](#sheetSet--)| SheetSet | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [drawObjectEventHandler](#drawObjectEventHandler--)| DrawObjectEventHandler | Implements this interface to get DrawObject and Bound when rendering. |
| [pageSavingCallback](#pageSavingCallback--)| IPageSavingCallback | Control/Indicate progress of page saving process. |
| [emfRenderSetting](#emfRenderSetting--)| EmfRenderSetting | Setting for rendering Emf metafile. |
| [customRenderSettings](#customRenderSettings--)| CustomRenderSettings | Gets or sets custom settings during rendering. |
## Methods
| Method | Description |
| --- | --- |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--)| <b>@deprecated.</b> Please use the 'embedStandardWindowsFonts' property instead. True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true. |
| [setEmbedStandardWindowsFonts(boolean)](#setEmbedStandardWindowsFonts-boolean-)| <b>@deprecated.</b> Please use the 'embedStandardWindowsFonts' property instead. True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true. |
| [getBookmark()](#getBookmark--)| <b>@deprecated.</b> Please use the 'bookmark' property instead. Gets and sets the <see cref ="PdfBookmarkEntry">PdfBookmarkEntry</see> object. |
| [setBookmark(PdfBookmarkEntry)](#setBookmark-pdfbookmarkentry-)| <b>@deprecated.</b> Please use the 'bookmark' property instead. Gets and sets the <see cref ="PdfBookmarkEntry">PdfBookmarkEntry</see> object. |
| [getCompliance()](#getCompliance--)| <b>@deprecated.</b> Please use the 'compliance' property instead. Gets or sets the PDF standards compliance level for output documents. |
| [setCompliance(PdfCompliance)](#setCompliance-pdfcompliance-)| <b>@deprecated.</b> Please use the 'compliance' property instead. Gets or sets the PDF standards compliance level for output documents. |
| [getSecurityOptions()](#getSecurityOptions--)| <b>@deprecated.</b> Please use the 'securityOptions' property instead. Set this options, when security is need in xls2pdf result. |
| [setSecurityOptions(PdfSecurityOptions)](#setSecurityOptions-pdfsecurityoptions-)| <b>@deprecated.</b> Please use the 'securityOptions' property instead. Set this options, when security is need in xls2pdf result. |
| [getCalculateFormula()](#getCalculateFormula--)| <b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving pdf file. |
| [setCalculateFormula(boolean)](#setCalculateFormula-boolean-)| <b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving pdf file. |
| [getPdfCompression()](#getPdfCompression--)| <b>@deprecated.</b> Please use the 'pdfCompression' property instead. Indicate the compression algorithm |
| [setPdfCompression(PdfCompressionCore)](#setPdfCompression-pdfcompressioncore-)| <b>@deprecated.</b> Please use the 'pdfCompression' property instead. Indicate the compression algorithm |
| [getCreatedTime()](#getCreatedTime--)| <b>@deprecated.</b> Please use the 'createdTime' property instead. Gets and sets the time of generating the pdf document. |
| [setCreatedTime(Date)](#setCreatedTime-date-)| <b>@deprecated.</b> Please use the 'createdTime' property instead. Gets and sets the time of generating the pdf document. |
| [getProducer()](#getProducer--)| <b>@deprecated.</b> Please use the 'producer' property instead. Gets and sets producer of generated pdf document. |
| [setProducer(string)](#setProducer-string-)| <b>@deprecated.</b> Please use the 'producer' property instead. Gets and sets producer of generated pdf document. |
| [getOptimizationType()](#getOptimizationType--)| <b>@deprecated.</b> Please use the 'optimizationType' property instead. Gets and sets pdf optimization type. |
| [setOptimizationType(PdfOptimizationType)](#setOptimizationType-pdfoptimizationtype-)| <b>@deprecated.</b> Please use the 'optimizationType' property instead. Gets and sets pdf optimization type. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--)| <b>@deprecated.</b> Please use the 'customPropertiesExport' property instead. Gets or sets a value determining the way [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) are exported to PDF file. Default value is None. |
| [setCustomPropertiesExport(PdfCustomPropertiesExport)](#setCustomPropertiesExport-pdfcustompropertiesexport-)| <b>@deprecated.</b> Please use the 'customPropertiesExport' property instead. Gets or sets a value determining the way [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) are exported to PDF file. Default value is None. |
| [getExportDocumentStructure()](#getExportDocumentStructure--)| <b>@deprecated.</b> Please use the 'exportDocumentStructure' property instead. Indicates whether to export document structure. |
| [setExportDocumentStructure(boolean)](#setExportDocumentStructure-boolean-)| <b>@deprecated.</b> Please use the 'exportDocumentStructure' property instead. Indicates whether to export document structure. |
| [getDisplayDocTitle()](#getDisplayDocTitle--)| <b>@deprecated.</b> Please use the 'displayDocTitle' property instead. Indicates whether the window's title bar should display the document title. |
| [setDisplayDocTitle(boolean)](#setDisplayDocTitle-boolean-)| <b>@deprecated.</b> Please use the 'displayDocTitle' property instead. Indicates whether the window's title bar should display the document title. |
| [getFontEncoding()](#getFontEncoding--)| <b>@deprecated.</b> Please use the 'fontEncoding' property instead. Gets or sets embedded font encoding in pdf. |
| [setFontEncoding(PdfFontEncoding)](#setFontEncoding-pdffontencoding-)| <b>@deprecated.</b> Please use the 'fontEncoding' property instead. Gets or sets embedded font encoding in pdf. |
| [getWatermark()](#getWatermark--)| <b>@deprecated.</b> Please use the 'watermark' property instead. Gets or sets watermark to output. |
| [setWatermark(RenderingWatermark)](#setWatermark-renderingwatermark-)| <b>@deprecated.</b> Please use the 'watermark' property instead. Gets or sets watermark to output. |
| [getEmbedAttachments()](#getEmbedAttachments--)| <b>@deprecated.</b> Please use the 'embedAttachments' property instead. Indicates whether to embed attachment for Ole objects in Excel. |
| [setEmbedAttachments(boolean)](#setEmbedAttachments-boolean-)| <b>@deprecated.</b> Please use the 'embedAttachments' property instead. Indicates whether to embed attachment for Ole objects in Excel. |
| [setImageResample(number, number)](#setImageResample-number-number-)| Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSaveFormat()](#getSaveFormat--)| <b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets the save file format. |
| [getClearData()](#getClearData--)| <b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file. |
| [setClearData(boolean)](#setClearData-boolean-)| <b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file. |
| [getCachedFileFolder()](#getCachedFileFolder--)| <b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache. |
| [setCachedFileFolder(string)](#setCachedFileFolder-string-)| <b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache. |
| [getValidateMergedAreas()](#getValidateMergedAreas--)| <b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file. |
| [setValidateMergedAreas(boolean)](#setValidateMergedAreas-boolean-)| <b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file. |
| [getMergeAreas()](#getMergeAreas--)| <b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setMergeAreas(boolean)](#setMergeAreas-boolean-)| <b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getCreateDirectory()](#getCreateDirectory--)| <b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCreateDirectory(boolean)](#setCreateDirectory-boolean-)| <b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getSortNames()](#getSortNames--)| <b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file. |
| [setSortNames(boolean)](#setSortNames-boolean-)| <b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file. |
| [getSortExternalNames()](#getSortExternalNames--)| <b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file. |
| [setSortExternalNames(boolean)](#setSortExternalNames-boolean-)| <b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file. |
| [getRefreshChartCache()](#getRefreshChartCache--)| <b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data |
| [setRefreshChartCache(boolean)](#setRefreshChartCache-boolean-)| <b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| <b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| <b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [getUpdateSmartArt()](#getUpdateSmartArt--)| <b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false. |
| [setUpdateSmartArt(boolean)](#setUpdateSmartArt-boolean-)| <b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--)| <b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [setEncryptDocumentProperties(boolean)](#setEncryptDocumentProperties-boolean-)| <b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [getDefaultFont()](#getDefaultFont--)| <b>@deprecated.</b> Please use the 'defaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [setDefaultFont(string)](#setDefaultFont-string-)| <b>@deprecated.</b> Please use the 'defaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--)| <b>@deprecated.</b> Please use the 'checkWorkbookDefaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [setCheckWorkbookDefaultFont(boolean)](#setCheckWorkbookDefaultFont-boolean-)| <b>@deprecated.</b> Please use the 'checkWorkbookDefaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [setCheckFontCompatibility(boolean)](#setCheckFontCompatibility-boolean-)| <b>@deprecated.</b> Please use the 'checkFontCompatibility' property instead. Indicates whether to check font compatibility for every character in text. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--)| <b>@deprecated.</b> Please use the 'checkFontCompatibility' property instead. Indicates whether to check font compatibility for every character in text. |
| [setIsFontSubstitutionCharGranularity(boolean)](#setIsFontSubstitutionCharGranularity-boolean-)| <b>@deprecated.</b> Please use the 'isFontSubstitutionCharGranularity' property instead. Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--)| <b>@deprecated.</b> Please use the 'isFontSubstitutionCharGranularity' property instead. Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [getOnePagePerSheet()](#getOnePagePerSheet--)| <b>@deprecated.</b> Please use the 'onePagePerSheet' property instead. If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [setOnePagePerSheet(boolean)](#setOnePagePerSheet-boolean-)| <b>@deprecated.</b> Please use the 'onePagePerSheet' property instead. If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--)| <b>@deprecated.</b> Please use the 'allColumnsInOnePagePerSheet' property instead. If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect. |
| [setAllColumnsInOnePagePerSheet(boolean)](#setAllColumnsInOnePagePerSheet-boolean-)| <b>@deprecated.</b> Please use the 'allColumnsInOnePagePerSheet' property instead. If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect. |
| [getIgnoreError()](#getIgnoreError--)| <b>@deprecated.</b> Please use the 'ignoreError' property instead. Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [setIgnoreError(boolean)](#setIgnoreError-boolean-)| <b>@deprecated.</b> Please use the 'ignoreError' property instead. Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--)| <b>@deprecated.</b> Please use the 'outputBlankPageWhenNothingToPrint' property instead. Indicates whether to output a blank page when there is nothing to print. |
| [setOutputBlankPageWhenNothingToPrint(boolean)](#setOutputBlankPageWhenNothingToPrint-boolean-)| <b>@deprecated.</b> Please use the 'outputBlankPageWhenNothingToPrint' property instead. Indicates whether to output a blank page when there is nothing to print. |
| [setPageIndex(number)](#setPageIndex-number-)| <b>@deprecated.</b> Please use the 'pageIndex' property instead. Gets or sets the 0-based index of the first page to save. |
| [getPageIndex()](#getPageIndex--)| <b>@deprecated.</b> Please use the 'pageIndex' property instead. Gets or sets the 0-based index of the first page to save. |
| [setPageCount(number)](#setPageCount-number-)| <b>@deprecated.</b> Please use the 'pageCount' property instead. Gets or sets the number of pages to save. |
| [getPageCount()](#getPageCount--)| <b>@deprecated.</b> Please use the 'pageCount' property instead. Gets or sets the number of pages to save. |
| [getPrintingPageType()](#getPrintingPageType--)| <b>@deprecated.</b> Please use the 'printingPageType' property instead. Indicates which pages will not be printed. |
| [setPrintingPageType(PrintingPageType)](#setPrintingPageType-printingpagetype-)| <b>@deprecated.</b> Please use the 'printingPageType' property instead. Indicates which pages will not be printed. |
| [getGridlineType()](#getGridlineType--)| <b>@deprecated.</b> Please use the 'gridlineType' property instead. Gets or sets gridline type. |
| [setGridlineType(GridlineType)](#setGridlineType-gridlinetype-)| <b>@deprecated.</b> Please use the 'gridlineType' property instead. Gets or sets gridline type. |
| [getGridlineColor()](#getGridlineColor--)| <b>@deprecated.</b> Please use the 'gridlineColor' property instead. Gets or sets gridline color. |
| [setGridlineColor(Color)](#setGridlineColor-color-)| <b>@deprecated.</b> Please use the 'gridlineColor' property instead. Gets or sets gridline color. |
| [getTextCrossType()](#getTextCrossType--)| <b>@deprecated.</b> Please use the 'textCrossType' property instead. Gets or sets displaying text type when the text width is larger than cell width. |
| [setTextCrossType(TextCrossType)](#setTextCrossType-textcrosstype-)| <b>@deprecated.</b> Please use the 'textCrossType' property instead. Gets or sets displaying text type when the text width is larger than cell width. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--)| <b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language. |
| [setDefaultEditLanguage(DefaultEditLanguage)](#setDefaultEditLanguage-defaulteditlanguage-)| <b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language. |
| [getSheetSet()](#getSheetSet--)| <b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [setSheetSet(SheetSet)](#setSheetSet-sheetset-)| <b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--)| <b>@deprecated.</b> Please use the 'drawObjectEventHandler' property instead. Implements this interface to get DrawObject and Bound when rendering. |
| [setDrawObjectEventHandler(DrawObjectEventHandler)](#setDrawObjectEventHandler-drawobjecteventhandler-)| <b>@deprecated.</b> Please use the 'drawObjectEventHandler' property instead. Implements this interface to get DrawObject and Bound when rendering. |
| [getPageSavingCallback()](#getPageSavingCallback--)| <b>@deprecated.</b> Please use the 'pageSavingCallback' property instead. Control/Indicate progress of page saving process. |
| [setPageSavingCallback(IPageSavingCallback)](#setPageSavingCallback-ipagesavingcallback-)| <b>@deprecated.</b> Please use the 'pageSavingCallback' property instead. Control/Indicate progress of page saving process. |
| [getEmfRenderSetting()](#getEmfRenderSetting--)| <b>@deprecated.</b> Please use the 'emfRenderSetting' property instead. Setting for rendering Emf metafile. |
| [setEmfRenderSetting(EmfRenderSetting)](#setEmfRenderSetting-emfrendersetting-)| <b>@deprecated.</b> Please use the 'emfRenderSetting' property instead. Setting for rendering Emf metafile. |
| [getCustomRenderSettings()](#getCustomRenderSettings--)| <b>@deprecated.</b> Please use the 'customRenderSettings' property instead. Gets or sets custom settings during rendering. |
| [setCustomRenderSettings(CustomRenderSettings)](#setCustomRenderSettings-customrendersettings-)| <b>@deprecated.</b> Please use the 'customRenderSettings' property instead. Gets or sets custom settings during rendering. |
### constructor() {#constructor--}
Creates the options for saving pdf file.
```javascript
constructor();
```
### constructor(PaginatedSaveOptions) {#constructor-paginatedsaveoptions-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: PaginatedSaveOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PaginatedSaveOptions | The parent object. |
### embedStandardWindowsFonts {#embedStandardWindowsFonts--}
True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.
```javascript
embedStandardWindowsFonts : boolean;
```
### bookmark {#bookmark--}
Gets and sets the <see cref ="PdfBookmarkEntry">PdfBookmarkEntry</see> object.
```javascript
bookmark : PdfBookmarkEntry;
```
### compliance {#compliance--}
Gets or sets the PDF standards compliance level for output documents.
```javascript
compliance : PdfCompliance;
```
**Remarks**
Default is Pdf17.
### securityOptions {#securityOptions--}
Set this options, when security is need in xls2pdf result.
```javascript
securityOptions : PdfSecurityOptions;
```
### calculateFormula {#calculateFormula--}
Indicates whether to calculate formulas before saving pdf file.
```javascript
calculateFormula : boolean;
```
**Remarks**
The default value is false.
### pdfCompression {#pdfCompression--}
Indicate the compression algorithm
```javascript
pdfCompression : PdfCompressionCore;
```
### createdTime {#createdTime--}
Gets and sets the time of generating the pdf document.
```javascript
createdTime : Date;
```
**Remarks**
if it is not be set, it will be the time of generating the pdf.
### producer {#producer--}
Gets and sets producer of generated pdf document.
```javascript
producer : string;
```
**Remarks**
If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.
### optimizationType {#optimizationType--}
Gets and sets pdf optimization type.
```javascript
optimizationType : PdfOptimizationType;
```
**Remarks**
Default value is [PdfOptimizationType.Standard](../pdfoptimizationtype.standard/)
### customPropertiesExport {#customPropertiesExport--}
Gets or sets a value determining the way [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) are exported to PDF file. Default value is None.
```javascript
customPropertiesExport : PdfCustomPropertiesExport;
```
### exportDocumentStructure {#exportDocumentStructure--}
Indicates whether to export document structure.
```javascript
exportDocumentStructure : boolean;
```
### displayDocTitle {#displayDocTitle--}
Indicates whether the window's title bar should display the document title.
```javascript
displayDocTitle : boolean;
```
**Remarks**
If false, the title bar should instead display the name of the PDF file. Default value is false.
### fontEncoding {#fontEncoding--}
Gets or sets embedded font encoding in pdf.
```javascript
fontEncoding : PdfFontEncoding;
```
**Remarks**
Default value is [PdfFontEncoding.Identity](../pdffontencoding.identity/)
### watermark {#watermark--}
Gets or sets watermark to output.
```javascript
watermark : RenderingWatermark;
```
### embedAttachments {#embedAttachments--}
Indicates whether to embed attachment for Ole objects in Excel.
```javascript
embedAttachments : boolean;
```
**Remarks**
Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.
### saveFormat {#saveFormat--}
Readonly. Gets the save file format.
```javascript
saveFormat : SaveFormat;
```
### clearData {#clearData--}
Make the workbook empty after saving the file.
```javascript
clearData : boolean;
```
### cachedFileFolder {#cachedFileFolder--}
The folder for temporary files that may be used as data cache.
```javascript
cachedFileFolder : string;
```
**Remarks**
If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.
### validateMergedAreas {#validateMergedAreas--}
Indicates whether validate merged cells before saving the file.
```javascript
validateMergedAreas : boolean;
```
**Remarks**
The default value is false.
### mergeAreas {#mergeAreas--}
Indicates whether merge the areas of conditional formatting and validation before saving the file.
```javascript
mergeAreas : boolean;
```
**Remarks**
The default value is false.
### createDirectory {#createDirectory--}
If true and the directory does not exist, the directory will be automatically created before saving the file.
```javascript
createDirectory : boolean;
```
**Remarks**
The default value is false.
### sortNames {#sortNames--}
Indicates whether sorting defined names before saving file.
```javascript
sortNames : boolean;
```
### sortExternalNames {#sortExternalNames--}
Indicates whether sorting external defined names before saving file.
```javascript
sortExternalNames : boolean;
```
### refreshChartCache {#refreshChartCache--}
Indicates whether refreshing chart cache data
```javascript
refreshChartCache : boolean;
```
### warningCallback {#warningCallback--}
Gets or sets warning callback.
```javascript
warningCallback : IWarningCallback;
```
### checkExcelRestriction {#checkExcelRestriction--}
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
```javascript
checkExcelRestriction : boolean;
```
### updateSmartArt {#updateSmartArt--}
Indicates whether updating smart art setting. The default value is false.
```javascript
updateSmartArt : boolean;
```
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
### encryptDocumentProperties {#encryptDocumentProperties--}
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
```javascript
encryptDocumentProperties : boolean;
```
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
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
### checkFontCompatibility {#checkFontCompatibility--}
Indicates whether to check font compatibility for every character in text.
```javascript
checkFontCompatibility : boolean;
```
**Remarks**
The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;
### isFontSubstitutionCharGranularity {#isFontSubstitutionCharGranularity--}
Indicates whether to only substitute the font of character when the cell font is not compatibility for it.
```javascript
isFontSubstitutionCharGranularity : boolean;
```
**Remarks**
Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.
### onePagePerSheet {#onePagePerSheet--}
If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
```javascript
onePagePerSheet : boolean;
```
### allColumnsInOnePagePerSheet {#allColumnsInOnePagePerSheet--}
If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.
```javascript
allColumnsInOnePagePerSheet : boolean;
```
### ignoreError {#ignoreError--}
Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.
```javascript
ignoreError : boolean;
```
### outputBlankPageWhenNothingToPrint {#outputBlankPageWhenNothingToPrint--}
Indicates whether to output a blank page when there is nothing to print.
```javascript
outputBlankPageWhenNothingToPrint : boolean;
```
**Remarks**
Default is true.
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
Default is System.Int32.MaxValue which means all pages will be rendered..
### printingPageType {#printingPageType--}
Indicates which pages will not be printed.
```javascript
printingPageType : PrintingPageType;
```
**Remarks**
If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.
### gridlineType {#gridlineType--}
Gets or sets gridline type.
```javascript
gridlineType : GridlineType;
```
**Remarks**
Default is Dotted type.
### gridlineColor {#gridlineColor--}
Gets or sets gridline color.
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
### drawObjectEventHandler {#drawObjectEventHandler--}
Implements this interface to get DrawObject and Bound when rendering.
```javascript
drawObjectEventHandler : DrawObjectEventHandler;
```
### pageSavingCallback {#pageSavingCallback--}
Control/Indicate progress of page saving process.
```javascript
pageSavingCallback : IPageSavingCallback;
```
### emfRenderSetting {#emfRenderSetting--}
Setting for rendering Emf metafile.
```javascript
emfRenderSetting : EmfRenderSetting;
```
**Remarks**
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/).
### customRenderSettings {#customRenderSettings--}
Gets or sets custom settings during rendering.
```javascript
customRenderSettings : CustomRenderSettings;
```
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```javascript
getEmbedStandardWindowsFonts() : boolean;
```
### setEmbedStandardWindowsFonts(boolean) {#setEmbedStandardWindowsFonts-boolean-}
```javascript
setEmbedStandardWindowsFonts(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getBookmark() {#getBookmark--}
```javascript
getBookmark() : PdfBookmarkEntry;
```
**Returns**
[PdfBookmarkEntry](../pdfbookmarkentry/)
### setBookmark(PdfBookmarkEntry) {#setBookmark-pdfbookmarkentry-}
```javascript
setBookmark(value: PdfBookmarkEntry) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../pdfbookmarkentry/) | The value to set. |
### getCompliance() {#getCompliance--}
```javascript
getCompliance() : PdfCompliance;
```
**Returns**
[PdfCompliance](../pdfcompliance/)
**Remarks**
Default is Pdf17.
### setCompliance(PdfCompliance) {#setCompliance-pdfcompliance-}
```javascript
setCompliance(value: PdfCompliance) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfCompliance](../pdfcompliance/) | The value to set. |
**Remarks**
Default is Pdf17.
### getSecurityOptions() {#getSecurityOptions--}
```javascript
getSecurityOptions() : PdfSecurityOptions;
```
**Returns**
[PdfSecurityOptions](../pdfsecurityoptions/)
### setSecurityOptions(PdfSecurityOptions) {#setSecurityOptions-pdfsecurityoptions-}
```javascript
setSecurityOptions(value: PdfSecurityOptions) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfSecurityOptions](../pdfsecurityoptions/) | The value to set. |
### getCalculateFormula() {#getCalculateFormula--}
```javascript
getCalculateFormula() : boolean;
```
**Remarks**
The default value is false.
### setCalculateFormula(boolean) {#setCalculateFormula-boolean-}
```javascript
setCalculateFormula(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false.
### getPdfCompression() {#getPdfCompression--}
```javascript
getPdfCompression() : PdfCompressionCore;
```
**Returns**
[PdfCompressionCore](../pdfcompressioncore/)
### setPdfCompression(PdfCompressionCore) {#setPdfCompression-pdfcompressioncore-}
```javascript
setPdfCompression(value: PdfCompressionCore) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfCompressionCore](../pdfcompressioncore/) | The value to set. |
### getCreatedTime() {#getCreatedTime--}
```javascript
getCreatedTime() : Date;
```
**Remarks**
if it is not be set, it will be the time of generating the pdf.
### setCreatedTime(Date) {#setCreatedTime-date-}
```javascript
setCreatedTime(value: Date) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Date | The value to set. |
**Remarks**
if it is not be set, it will be the time of generating the pdf.
### getProducer() {#getProducer--}
```javascript
getProducer() : string;
```
**Remarks**
If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.
### setProducer(string) {#setProducer-string-}
```javascript
setProducer(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.
### getOptimizationType() {#getOptimizationType--}
```javascript
getOptimizationType() : PdfOptimizationType;
```
**Returns**
[PdfOptimizationType](../pdfoptimizationtype/)
**Remarks**
Default value is [PdfOptimizationType.Standard](../pdfoptimizationtype.standard/)
### setOptimizationType(PdfOptimizationType) {#setOptimizationType-pdfoptimizationtype-}
```javascript
setOptimizationType(value: PdfOptimizationType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfOptimizationType](../pdfoptimizationtype/) | The value to set. |
**Remarks**
Default value is [PdfOptimizationType.Standard](../pdfoptimizationtype.standard/)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```javascript
getCustomPropertiesExport() : PdfCustomPropertiesExport;
```
**Returns**
[PdfCustomPropertiesExport](../pdfcustompropertiesexport/)
### setCustomPropertiesExport(PdfCustomPropertiesExport) {#setCustomPropertiesExport-pdfcustompropertiesexport-}
```javascript
setCustomPropertiesExport(value: PdfCustomPropertiesExport) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfCustomPropertiesExport](../pdfcustompropertiesexport/) | The value to set. |
### getExportDocumentStructure() {#getExportDocumentStructure--}
```javascript
getExportDocumentStructure() : boolean;
```
### setExportDocumentStructure(boolean) {#setExportDocumentStructure-boolean-}
```javascript
setExportDocumentStructure(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getDisplayDocTitle() {#getDisplayDocTitle--}
```javascript
getDisplayDocTitle() : boolean;
```
**Remarks**
If false, the title bar should instead display the name of the PDF file. Default value is false.
### setDisplayDocTitle(boolean) {#setDisplayDocTitle-boolean-}
```javascript
setDisplayDocTitle(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
If false, the title bar should instead display the name of the PDF file. Default value is false.
### getFontEncoding() {#getFontEncoding--}
```javascript
getFontEncoding() : PdfFontEncoding;
```
**Returns**
[PdfFontEncoding](../pdffontencoding/)
**Remarks**
Default value is [PdfFontEncoding.Identity](../pdffontencoding.identity/)
### setFontEncoding(PdfFontEncoding) {#setFontEncoding-pdffontencoding-}
```javascript
setFontEncoding(value: PdfFontEncoding) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfFontEncoding](../pdffontencoding/) | The value to set. |
**Remarks**
Default value is [PdfFontEncoding.Identity](../pdffontencoding.identity/)
### getWatermark() {#getWatermark--}
```javascript
getWatermark() : RenderingWatermark;
```
**Returns**
[RenderingWatermark](../renderingwatermark/)
### setWatermark(RenderingWatermark) {#setWatermark-renderingwatermark-}
```javascript
setWatermark(value: RenderingWatermark) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RenderingWatermark](../renderingwatermark/) | The value to set. |
### getEmbedAttachments() {#getEmbedAttachments--}
```javascript
getEmbedAttachments() : boolean;
```
**Remarks**
Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.
### setEmbedAttachments(boolean) {#setEmbedAttachments-boolean-}
```javascript
setEmbedAttachments(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.
### setImageResample(number, number) {#setImageResample-number-number-}
Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled.
```javascript
setImageResample(desiredPPI: number, jpegQuality: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredPPI | number | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpegQuality | number | 0 - 100% JPEG quality. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getSaveFormat() {#getSaveFormat--}
```javascript
getSaveFormat() : SaveFormat;
```
**Returns**
[SaveFormat](../saveformat/)
### getClearData() {#getClearData--}
```javascript
getClearData() : boolean;
```
### setClearData(boolean) {#setClearData-boolean-}
```javascript
setClearData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCachedFileFolder() {#getCachedFileFolder--}
```javascript
getCachedFileFolder() : string;
```
**Remarks**
If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.
### setCachedFileFolder(string) {#setCachedFileFolder-string-}
```javascript
setCachedFileFolder(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.
### getValidateMergedAreas() {#getValidateMergedAreas--}
```javascript
getValidateMergedAreas() : boolean;
```
**Remarks**
The default value is false.
### setValidateMergedAreas(boolean) {#setValidateMergedAreas-boolean-}
```javascript
setValidateMergedAreas(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false.
### getMergeAreas() {#getMergeAreas--}
```javascript
getMergeAreas() : boolean;
```
**Remarks**
The default value is false.
### setMergeAreas(boolean) {#setMergeAreas-boolean-}
```javascript
setMergeAreas(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false.
### getCreateDirectory() {#getCreateDirectory--}
```javascript
getCreateDirectory() : boolean;
```
**Remarks**
The default value is false.
### setCreateDirectory(boolean) {#setCreateDirectory-boolean-}
```javascript
setCreateDirectory(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is false.
### getSortNames() {#getSortNames--}
```javascript
getSortNames() : boolean;
```
### setSortNames(boolean) {#setSortNames-boolean-}
```javascript
setSortNames(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSortExternalNames() {#getSortExternalNames--}
```javascript
getSortExternalNames() : boolean;
```
### setSortExternalNames(boolean) {#setSortExternalNames-boolean-}
```javascript
setSortExternalNames(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getRefreshChartCache() {#getRefreshChartCache--}
```javascript
getRefreshChartCache() : boolean;
```
### setRefreshChartCache(boolean) {#setRefreshChartCache-boolean-}
```javascript
setRefreshChartCache(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}
```javascript
setWarningCallback(value: IWarningCallback) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |
### getWarningCallback() {#getWarningCallback--}
```javascript
getWarningCallback() : IWarningCallback;
```
**Returns**
[IWarningCallback](../iwarningcallback/)
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```javascript
getCheckExcelRestriction() : boolean;
```
### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}
```javascript
setCheckExcelRestriction(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getUpdateSmartArt() {#getUpdateSmartArt--}
```javascript
getUpdateSmartArt() : boolean;
```
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
### setUpdateSmartArt(boolean) {#setUpdateSmartArt-boolean-}
```javascript
setUpdateSmartArt(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```javascript
getEncryptDocumentProperties() : boolean;
```
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
### setEncryptDocumentProperties(boolean) {#setEncryptDocumentProperties-boolean-}
```javascript
setEncryptDocumentProperties(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
### getDefaultFont() {#getDefaultFont--}
```javascript
getDefaultFont() : string;
```
### setDefaultFont(string) {#setDefaultFont-string-}
```javascript
setDefaultFont(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}
```javascript
getCheckWorkbookDefaultFont() : boolean;
```
**Remarks**
Default is true.
### setCheckWorkbookDefaultFont(boolean) {#setCheckWorkbookDefaultFont-boolean-}
```javascript
setCheckWorkbookDefaultFont(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Default is true.
### setCheckFontCompatibility(boolean) {#setCheckFontCompatibility-boolean-}
```javascript
setCheckFontCompatibility(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```javascript
getCheckFontCompatibility() : boolean;
```
**Remarks**
The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;
### setIsFontSubstitutionCharGranularity(boolean) {#setIsFontSubstitutionCharGranularity-boolean-}
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
```javascript
isFontSubstitutionCharGranularity() : boolean;
```
**Remarks**
Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.
### getOnePagePerSheet() {#getOnePagePerSheet--}
```javascript
getOnePagePerSheet() : boolean;
```
### setOnePagePerSheet(boolean) {#setOnePagePerSheet-boolean-}
```javascript
setOnePagePerSheet(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}
```javascript
getAllColumnsInOnePagePerSheet() : boolean;
```
### setAllColumnsInOnePagePerSheet(boolean) {#setAllColumnsInOnePagePerSheet-boolean-}
```javascript
setAllColumnsInOnePagePerSheet(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIgnoreError() {#getIgnoreError--}
```javascript
getIgnoreError() : boolean;
```
### setIgnoreError(boolean) {#setIgnoreError-boolean-}
```javascript
setIgnoreError(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```javascript
getOutputBlankPageWhenNothingToPrint() : boolean;
```
**Remarks**
Default is true.
### setOutputBlankPageWhenNothingToPrint(boolean) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```javascript
setOutputBlankPageWhenNothingToPrint(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
Default is true.
### setPageIndex(number) {#setPageIndex-number-}
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
```javascript
getPageIndex() : number;
```
**Remarks**
Default is 0.
### setPageCount(number) {#setPageCount-number-}
```javascript
setPageCount(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
Default is System.Int32.MaxValue which means all pages will be rendered..
### getPageCount() {#getPageCount--}
```javascript
getPageCount() : number;
```
**Remarks**
Default is System.Int32.MaxValue which means all pages will be rendered..
### getPrintingPageType() {#getPrintingPageType--}
```javascript
getPrintingPageType() : PrintingPageType;
```
**Returns**
[PrintingPageType](../printingpagetype/)
**Remarks**
If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.
### setPrintingPageType(PrintingPageType) {#setPrintingPageType-printingpagetype-}
```javascript
setPrintingPageType(value: PrintingPageType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PrintingPageType](../printingpagetype/) | The value to set. |
**Remarks**
If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.
### getGridlineType() {#getGridlineType--}
```javascript
getGridlineType() : GridlineType;
```
**Returns**
[GridlineType](../gridlinetype/)
**Remarks**
Default is Dotted type.
### setGridlineType(GridlineType) {#setGridlineType-gridlinetype-}
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
```javascript
getGridlineColor() : Color;
```
**Returns**
[Color](../color/)
**Remarks**
It will ignore the gridline color settings in the source file.
### setGridlineColor(Color) {#setGridlineColor-color-}
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
```javascript
getTextCrossType() : TextCrossType;
```
**Returns**
[TextCrossType](../textcrosstype/)
### setTextCrossType(TextCrossType) {#setTextCrossType-textcrosstype-}
```javascript
setTextCrossType(value: TextCrossType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextCrossType](../textcrosstype/) | The value to set. |
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```javascript
getDefaultEditLanguage() : DefaultEditLanguage;
```
**Returns**
[DefaultEditLanguage](../defaulteditlanguage/)
**Remarks**
It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).
### setDefaultEditLanguage(DefaultEditLanguage) {#setDefaultEditLanguage-defaulteditlanguage-}
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
```javascript
getSheetSet() : SheetSet;
```
**Returns**
[SheetSet](../sheetset/)
### setSheetSet(SheetSet) {#setSheetSet-sheetset-}
```javascript
setSheetSet(value: SheetSet) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../sheetset/) | The value to set. |
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```javascript
getDrawObjectEventHandler() : DrawObjectEventHandler;
```
**Returns**
[DrawObjectEventHandler](../drawobjecteventhandler/)
### setDrawObjectEventHandler(DrawObjectEventHandler) {#setDrawObjectEventHandler-drawobjecteventhandler-}
```javascript
setDrawObjectEventHandler(value: DrawObjectEventHandler) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../drawobjecteventhandler/) | The value to set. |
### getPageSavingCallback() {#getPageSavingCallback--}
```javascript
getPageSavingCallback() : IPageSavingCallback;
```
**Returns**
[IPageSavingCallback](../ipagesavingcallback/)
### setPageSavingCallback(IPageSavingCallback) {#setPageSavingCallback-ipagesavingcallback-}
```javascript
setPageSavingCallback(value: IPageSavingCallback) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../ipagesavingcallback/) | The value to set. |
### getEmfRenderSetting() {#getEmfRenderSetting--}
```javascript
getEmfRenderSetting() : EmfRenderSetting;
```
**Returns**
[EmfRenderSetting](../emfrendersetting/)
**Remarks**
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/).
### setEmfRenderSetting(EmfRenderSetting) {#setEmfRenderSetting-emfrendersetting-}
```javascript
setEmfRenderSetting(value: EmfRenderSetting) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EmfRenderSetting](../emfrendersetting/) | The value to set. |
**Remarks**
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/).
### getCustomRenderSettings() {#getCustomRenderSettings--}
```javascript
getCustomRenderSettings() : CustomRenderSettings;
```
**Returns**
[CustomRenderSettings](../customrendersettings/)
### setCustomRenderSettings(CustomRenderSettings) {#setCustomRenderSettings-customrendersettings-}
```javascript
setCustomRenderSettings(value: CustomRenderSettings) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomRenderSettings](../customrendersettings/) | The value to set. |
