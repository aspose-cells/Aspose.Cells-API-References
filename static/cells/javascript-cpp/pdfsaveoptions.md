##PdfSaveOptions
Represents the options for saving pdf file.
## PdfSaveOptions class
Represents the options for saving pdf file.
```javascript
class PdfSaveOptions extends PaginatedSaveOptions;
```
## Constructors
| Name | Description |
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
| [setImageResample(number, number)](#setImageResample-number-number-)| Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled. |
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
