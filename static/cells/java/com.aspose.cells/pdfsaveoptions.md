##PdfSaveOptions
Represents the options for saving pdf file.
**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PdfSaveOptions extends PaginatedSaveOptions
```
Represents the options for saving pdf file.
## Constructors
| Constructor | Description |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Creates the options for saving pdf file. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. |
| [getBookmark()](#getBookmark--) | Gets the [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) object. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The folder for temporary files that may be used as data cache. |
| [getCalculateFormula()](#getCalculateFormula--) | Indicates whether to calculate formulas before saving pdf file. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indicates whether to check font compatibility for every character in text. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCompliance()](#getCompliance--) | Gets the PDF standards compliance level for output documents. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getCreatedTime()](#getCreatedTime--) | Gets the time of generating the pdf document. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | Gets a value determining the way [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) are exported to PDF file. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Gets custom settings during rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Gets default edit language. |
| [getDefaultFont()](#getDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | Indicates whether the window's title bar should display the document title. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbedAttachments()](#getEmbedAttachments--) | Indicates whether to embed attachment for Ole objects in Excel. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | True to embed true type fonts. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Setting for rendering Emf metafile. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indicates whether encrypt document properties when saving as .xls file. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | Indicates whether to export document structure. |
| [getFontEncoding()](#getFontEncoding--) | Gets embedded font encoding in pdf. |
| [getGridlineColor()](#getGridlineColor--) | Gets gridline color. |
| [getGridlineType()](#getGridlineType--) | Gets gridline type. |
| [getIgnoreError()](#getIgnoreError--) | Indicates if you need to hide the error while rendering. |
| [getImageType()](#getImageType--) | Represents the image type when converting the chart and shape . |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. |
| [getOptimizationType()](#getOptimizationType--) | Gets pdf optimization type. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indicates whether to output a blank page when there is nothing to print. |
| [getPageCount()](#getPageCount--) | Gets the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | Gets the 0-based index of the first page to save. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Control/Indicate progress of page saving process. |
| [getPdfCompression()](#getPdfCompression--) | Indicate the compression algorithm |
| [getPrintingPageType()](#getPrintingPageType--) | Indicates which pages will not be printed. |
| [getProducer()](#getProducer--) | Gets producer of generated pdf document. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSecurityOptions()](#getSecurityOptions--) | Set this options, when security is need in xls2pdf result. |
| [getSheetSet()](#getSheetSet--) | Gets the sheets to render. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getTextCrossType()](#getTextCrossType--) | Gets displaying text type when the text width is larger than cell width. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [getWatermark()](#getWatermark--) | Gets watermark to output. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | Sets the [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) object. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | The folder for temporary files that may be used as data cache. |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | Indicates whether to calculate formulas before saving pdf file. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Indicates whether to check font compatibility for every character in text. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [setClearData(boolean value)](#setClearData-boolean-) | Make the workbook empty after saving the file. |
| [setCompliance(int value)](#setCompliance-int-) | Sets the PDF standards compliance level for output documents. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | Sets the time of generating the pdf document. |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | Sets a value determining the way [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) are exported to PDF file. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Sets custom settings during rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Sets default edit language. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | Indicates whether the window's title bar should display the document title. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implements this interface to get DrawObject and Bound when rendering. |
| [setEmbedAttachments(boolean value)](#setEmbedAttachments-boolean-) | Indicates whether to embed attachment for Ole objects in Excel. |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | True to embed true type fonts. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Setting for rendering Emf metafile. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indicates whether encrypt document properties when saving as .xls file. |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | Indicates whether to export document structure. |
| [setFontEncoding(int value)](#setFontEncoding-int-) | Sets embedded font encoding in pdf. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Sets gridline color. |
| [setGridlineType(int value)](#setGridlineType-int-) | Sets gridline type. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indicates if you need to hide the error while rendering. |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | Sets desired PPI(pixels per inch) of resample images and jpeg quality. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | Represents the image type when converting the chart and shape . |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. |
| [setOptimizationType(int value)](#setOptimizationType-int-) | Sets pdf optimization type. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indicates whether to output a blank page when there is nothing to print. |
| [setPageCount(int value)](#setPageCount-int-) | Sets the number of pages to save. |
| [setPageIndex(int value)](#setPageIndex-int-) | Sets the 0-based index of the first page to save. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Control/Indicate progress of page saving process. |
| [setPdfCompression(int value)](#setPdfCompression-int-) | Indicate the compression algorithm |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Indicates which pages will not be printed. |
| [setProducer(String value)](#setProducer-java.lang.String-) | Sets producer of generated pdf document. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indicates whether refreshing chart cache data |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | Set this options, when security is need in xls2pdf result. |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Sets the sheets to render. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indicates whether sorting external defined names before saving file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indicates whether sorting defined names before saving file. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Sets displaying text type when the text width is larger than cell width. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indicates whether updating smart art setting. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indicates whether validate merged cells before saving the file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [setWatermark(RenderingWatermark value)](#setWatermark-com.aspose.cells.RenderingWatermark-) | Sets watermark to output. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```
Creates the options for saving pdf file.
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
If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.
**Returns:**
boolean
### getBookmark() {#getBookmark--}
```
public PdfBookmarkEntry getBookmark()
```
Gets the [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) object.
**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```
The folder for temporary files that may be used as data cache.
**Remarks**
If the folder has not been specified, the default value for it is void
**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```
Indicates whether to calculate formulas before saving pdf file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```
Indicates whether to check font compatibility for every character in text.
**Remarks**
The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;
**Returns:**
boolean
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
### getClearData() {#getClearData--}
```
public boolean getClearData()
```
Make the workbook empty after saving the file.
**Returns:**
boolean
### getCompliance() {#getCompliance--}
```
public int getCompliance()
```
Gets the PDF standards compliance level for output documents.
See [PdfCompliance](../../com.aspose.cells/pdfcompliance).
**Remarks**
Default is Pdf17.
**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```
If true and the directory does not exist, the directory will be automatically created before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```
Gets the time of generating the pdf document.
**Remarks**
if it is not be set, it will be the time of generating the pdf.
**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```
Gets a value determining the way [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) are exported to PDF file. Default value is None.
See [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).
**Returns:**
int
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
### getDisplayDocTitle() {#getDisplayDocTitle--}
```
public boolean getDisplayDocTitle()
```
Indicates whether the window's title bar should display the document title.
**Remarks**
If false, the title bar should instead display the name of the PDF file. Default value is false.
**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```
Implements this interface to get DrawObject and Bound when rendering.
**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedAttachments() {#getEmbedAttachments--}
```
public boolean getEmbedAttachments()
```
Indicates whether to embed attachment for Ole objects in Excel.
**Remarks**
Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.
**Returns:**
boolean
### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}
```
public boolean getEmbedStandardWindowsFonts()
```
True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.
**Returns:**
boolean
### getEmfRenderSetting() {#getEmfRenderSetting--}
```
public int getEmfRenderSetting()
```
Setting for rendering Emf metafile.
See [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).
**Remarks**
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).
**Returns:**
int
### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}
```
public boolean getEncryptDocumentProperties()
```
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
**Returns:**
boolean
### getExportDocumentStructure() {#getExportDocumentStructure--}
```
public boolean getExportDocumentStructure()
```
Indicates whether to export document structure.
**Returns:**
boolean
### getFontEncoding() {#getFontEncoding--}
```
public int getFontEncoding()
```
Gets embedded font encoding in pdf.
See [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).
**Remarks**
Default value is [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)
**Returns:**
int
### getGridlineColor() {#getGridlineColor--}
```
public Color getGridlineColor()
```
Gets gridline color.
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
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```
Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.
**Returns:**
boolean
### getImageType() {#getImageType--}
```
public ImageFormat getImageType()
```
Represents the image type when converting the chart and shape .
**Remarks**
NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```
Indicates whether merge the areas of conditional formatting and validation before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getOnePagePerSheet() {#getOnePagePerSheet--}
```
public boolean getOnePagePerSheet()
```
If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
**Returns:**
boolean
### getOptimizationType() {#getOptimizationType--}
```
public int getOptimizationType()
```
Gets pdf optimization type.
See [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).
**Remarks**
Default value is [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)
**Returns:**
int
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```
Indicates whether to output a blank page when there is nothing to print.
**Remarks**
Default is true.
**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```
Gets the number of pages to save.
**Remarks**
Default is System.Int32.MaxValue which means all pages will be rendered..
**Example**
The following example shows how to render a range of pages (3 and 4) in a Microsoft Excel file to PDF.
```
//Open an Excel file
Workbook wb = new Workbook("Book1.xlsx");
PdfSaveOptions options = new PdfSaveOptions();
//Print only Page 3 and Page 4 in the output PDF
//Starting page index (0-based index)
options.setPageIndex(3);
//Number of pages to be printed
options.setPageCount(2);
//Save the PDF file
wb.save("output.pdf", options);
```
**Returns:**
int
### getPageIndex() {#getPageIndex--}
```
public int getPageIndex()
```
Gets the 0-based index of the first page to save.
**Remarks**
Default is 0.
**Example**
The following example shows how to render a range of pages (3 and 4) in a Microsoft Excel file to PDF.
```
//Open an Excel file
Workbook wb = new Workbook("Book1.xlsx");
PdfSaveOptions options = new PdfSaveOptions();
//Print only Page 3 and Page 4 in the output PDF
//Starting page index (0-based index)
options.setPageIndex(3);
//Number of pages to be printed
options.setPageCount(2);
//Save the PDF file
wb.save("output.pdf", options);
```
**Returns:**
int
### getPageSavingCallback() {#getPageSavingCallback--}
```
public IPageSavingCallback getPageSavingCallback()
```
Control/Indicate progress of page saving process.
**Returns:**
[IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback)
### getPdfCompression() {#getPdfCompression--}
```
public int getPdfCompression()
```
Indicate the compression algorithm
See [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).
**Returns:**
int
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```
Indicates which pages will not be printed.
See [PrintingPageType](../../com.aspose.cells/printingpagetype).
**Remarks**
If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.
**Example**
The following code omits blank pages or pages which only contains some style content like cell background, borders.
```
Workbook wb = new Workbook("Book1.xlsx");
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
//ignore blank pages
pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_BLANK);
wb.save("output_ignore_blank_page.pdf", pdfSaveOptions);
//ignore blank pages and pages which only contains some style content like cell background
pdfSaveOptions.setPrintingPageType(PrintingPageType.IGNORE_STYLE);
wb.save("output_ignore_blank_and_style_page.pdf", pdfSaveOptions);
```
**Returns:**
int
### getProducer() {#getProducer--}
```
public String getProducer()
```
Gets producer of generated pdf document.
**Remarks**
If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.
**Returns:**
java.lang.String
### getRefreshChartCache() {#getRefreshChartCache--}
```
public boolean getRefreshChartCache()
```
Indicates whether refreshing chart cache data
**Returns:**
boolean
### getSaveFormat() {#getSaveFormat--}
```
public int getSaveFormat()
```
Gets the save file format.
See [SaveFormat](../../com.aspose.cells/saveformat).
**Returns:**
int
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```
Set this options, when security is need in xls2pdf result.
**Example**
The following code sets hight resolution print permisson for the output pdf.
```
Workbook wb = new Workbook();
wb.getWorksheets().get(0).getCells().get("A1").setValue("Aspose");
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
PdfSecurityOptions pdfSecurityOptions = new PdfSecurityOptions();
//set owner password
pdfSecurityOptions.setOwnerPassword("YourOwnerPassword");
//set user password
pdfSecurityOptions.setUserPassword("YourUserPassword");
//set print permisson
pdfSecurityOptions.setPrintPermission(true);
//set high resolution for print
pdfSecurityOptions.setFullQualityPrintPermission(true);
pdfSaveOptions.setSecurityOptions(pdfSecurityOptions);
wb.save("output.pdf", pdfSaveOptions);
```
**Returns:**
[PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions)
### getSheetSet() {#getSheetSet--}
```
public SheetSet getSheetSet()
```
Gets the sheets to render. Default is all visible sheets in the workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).
**Example**
The following code only renders active sheet to pdf.
```
Workbook workbook = new Workbook("Book1.xlsx");
int activeSheetIndex = workbook.getWorksheets().getActiveSheetIndex();
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
//set active sheet index to sheet set.
pdfSaveOptions.setSheetSet(new SheetSet(new int[] { activeSheetIndex }));
workbook.save("output.pdf", pdfSaveOptions);
```
**Returns:**
[SheetSet](../../com.aspose.cells/sheetset)
### getSortExternalNames() {#getSortExternalNames--}
```
public boolean getSortExternalNames()
```
Indicates whether sorting external defined names before saving file.
**Returns:**
boolean
### getSortNames() {#getSortNames--}
```
public boolean getSortNames()
```
Indicates whether sorting defined names before saving file.
**Returns:**
boolean
### getTextCrossType() {#getTextCrossType--}
```
public int getTextCrossType()
```
Gets displaying text type when the text width is larger than cell width.
See [TextCrossType](../../com.aspose.cells/textcrosstype).
**Returns:**
int
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```
Indicates whether updating smart art setting. The default value is false.
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```
Indicates whether validate merged cells before saving the file.
**Remarks**
The default value is false.
**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```
Gets warning callback.
**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
### getWatermark() {#getWatermark--}
```
public RenderingWatermark getWatermark()
```
Gets watermark to output.
**Example**
The following code sets watermark in the output pdf.
```
//prepare a workbook with 3 pages.
Workbook wb = new Workbook();
wb.getWorksheets().get(0).getCells().get("A1").putValue("Page1");
int index = wb.getWorksheets().add();
wb.getWorksheets().get(index).getCells().get("A1").putValue("Page2");
index = wb.getWorksheets().add();
wb.getWorksheets().get(index).getCells().get("A1").putValue("Page3");
wb.getWorksheets().get(index).getPageSetup().setPaperSize(PaperSizeType.PAPER_A_3);
//create a font for watermark, and specify bold, italic, color
RenderingFont font = new RenderingFont("Calibri", 68);
font.setItalic(true);
font.setBold(true);
font.setColor(Color.getBlue());
//create a watermark from text and the specified font
RenderingWatermark watermark = new RenderingWatermark("Watermark", font);
//specify horizontal and vertical alignment
watermark.setHAlignment(TextAlignmentType.CENTER);
watermark.setVAlignment(TextAlignmentType.CENTER);
//specify rotation
watermark.setRotation(30);
//specify opacity
watermark.setOpacity(0.6f);
//specify the scale to page(e.g. 100, 50) in percent.
watermark.setScaleToPagePercent(50);
//spcify watermark for rendering to pdf.
PdfSaveOptions options = new PdfSaveOptions();
options.setWatermark(watermark);
wb.save("output_watermark.pdf", options);
```
**Returns:**
[RenderingWatermark](../../com.aspose.cells/renderingwatermark)
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isFontSubstitutionCharGranularity() {#isFontSubstitutionCharGranularity--}
```
public boolean isFontSubstitutionCharGranularity()
```
Indicates whether to only substitute the font of character when the cell font is not compatibility for it.
**Remarks**
Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.
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
If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```
Sets the [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |
### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```
The folder for temporary files that may be used as data cache.
**Remarks**
If the folder has not been specified, the default value for it is void
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```
Indicates whether to calculate formulas before saving pdf file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```
Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```
Indicates whether to check font compatibility for every character in text.
**Remarks**
The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```
Make the workbook empty after saving the file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```
Sets the PDF standards compliance level for output documents.
See [PdfCompliance](../../com.aspose.cells/pdfcompliance).
**Remarks**
Default is Pdf17.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```
If true and the directory does not exist, the directory will be automatically created before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```
Sets the time of generating the pdf document.
**Remarks**
if it is not be set, it will be the time of generating the pdf.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |
### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```
Sets a value determining the way [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) are exported to PDF file. Default value is None.
See [PdfCustomPropertiesExport](../../com.aspose.cells/pdfcustompropertiesexport).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```
Indicates whether the window's title bar should display the document title.
**Remarks**
If false, the title bar should instead display the name of the PDF file. Default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```
Implements this interface to get DrawObject and Bound when rendering.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |
### setEmbedAttachments(boolean value) {#setEmbedAttachments-boolean-}
```
public void setEmbedAttachments(boolean value)
```
Indicates whether to embed attachment for Ole objects in Excel.
**Remarks**
Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```
True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```
Setting for rendering Emf metafile.
See [EmfRenderSetting](../../com.aspose.cells/emfrendersetting).
**Remarks**
EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [EmfRenderSetting.EMF\_PLUS\_PREFER](../../com.aspose.cells/emfrendersetting\#EMF-PLUS-PREFER) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [EmfRenderSetting.EMF\_ONLY](../../com.aspose.cells/emfrendersetting\#EMF-ONLY).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setEncryptDocumentProperties(boolean value) {#setEncryptDocumentProperties-boolean-}
```
public void setEncryptDocumentProperties(boolean value)
```
Indicates whether encrypt document properties when saving as .xls file. The default value is true.
**Remarks**
Only for .xls,xlsx,xlsb and xlsm file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```
Indicates whether to export document structure.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```
Sets embedded font encoding in pdf.
See [PdfFontEncoding](../../com.aspose.cells/pdffontencoding).
**Remarks**
Default value is [PdfFontEncoding.IDENTITY](../../com.aspose.cells/pdffontencoding\#IDENTITY)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
Sets gridline color.
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
### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```
Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```
Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled.
**Example**
The following code sets desired PPI as 96 and jpeg quality as 80 for images in the output pdf.
```
//load the source file with images.
Workbook wb = new Workbook("Book1.xlsx");
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
//set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.setImageResample(96, 80);
wb.save("output.pdf", pdfSaveOptions);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| desiredPPI | int | Desired pixels per inch. 220 high quality. 150 screen quality. 96 email quality. |
| jpegQuality | int | 0 - 100% JPEG quality. |
### setImageType(ImageFormat value) {#setImageType-com.aspose.cells.ImageFormat-}
```
public void setImageType(ImageFormat value)
```
Represents the image type when converting the chart and shape .
**Remarks**
NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |
### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```
Indicates whether merge the areas of conditional formatting and validation before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```
If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```
Sets pdf optimization type.
See [PdfOptimizationType](../../com.aspose.cells/pdfoptimizationtype).
**Remarks**
Default value is [PdfOptimizationType.STANDARD](../../com.aspose.cells/pdfoptimizationtype\#STANDARD)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```
Indicates whether to output a blank page when there is nothing to print.
**Remarks**
Default is true.
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
Default is System.Int32.MaxValue which means all pages will be rendered..
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
### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```
Indicate the compression algorithm
See [PdfCompressionCore](../../com.aspose.cells/pdfcompressioncore).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```
Indicates which pages will not be printed.
See [PrintingPageType](../../com.aspose.cells/printingpagetype).
**Remarks**
If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```
Sets producer of generated pdf document.
**Remarks**
If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```
Indicates whether refreshing chart cache data
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```
Set this options, when security is need in xls2pdf result.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |
### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```
Sets the sheets to render. Default is all visible sheets in the workbook: [SheetSet.getVisible()](../../com.aspose.cells/sheetset\#getVisible--).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |
### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```
Indicates whether sorting external defined names before saving file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```
Indicates whether sorting defined names before saving file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```
Indicates whether updating smart art setting. The default value is false.
**Remarks**
Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```
Indicates whether validate merged cells before saving the file.
**Remarks**
The default value is false.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setWarningCallback(IWarningCallback value) {#setWarningCallback-com.aspose.cells.IWarningCallback-}
```
public void setWarningCallback(IWarningCallback value)
```
Sets warning callback.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../../com.aspose.cells/iwarningcallback) |  |
### setWatermark(RenderingWatermark value) {#setWatermark-com.aspose.cells.RenderingWatermark-}
```
public void setWatermark(RenderingWatermark value)
```
Sets watermark to output.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RenderingWatermark](../../com.aspose.cells/renderingwatermark) |  |
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
