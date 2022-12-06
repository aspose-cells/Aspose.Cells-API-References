---
title: PdfSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options for saving pdf file.
type: docs
url: /java/com.aspose.cells/pdfsaveoptions/
---

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
| [getBookmark()](#getBookmark--) | the [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) object. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The cached file folder is used to store some large data. |
| [getCalculateFormula()](#getCalculateFormula--) | Indicates whether to calculate formulas before saving pdf file. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indicates whether to check font compatibility for every character in text. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCompliance()](#getCompliance--) | Workbook converts to pdf will according to PdfCompliance in this property. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getCreatedTime()](#getCreatedTime--) | the time of generating the pdf document. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--) | a value determining the way [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) are exported to PDF file. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | default edit language. |
| [getDefaultFont()](#getDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getDisplayDocTitle()](#getDisplayDocTitle--) | Indicates whether the window's title bar should display the document title. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--) | True to embed true type fonts. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Setting for rendering Emf metafile. |
| [getExportDocumentStructure()](#getExportDocumentStructure--) | Indicates whether to export document structure. |
| [getFontEncoding()](#getFontEncoding--) | embedded font encoding in pdf. |
| [getGridlineType()](#getGridlineType--) | gridline type. |
| [getIgnoreError()](#getIgnoreError--) | Indicates if you need to hide the error while rendering. |
| [getImageType()](#getImageType--) | Represents the image type when converting the chart and shape . |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. |
| [getOptimizationType()](#getOptimizationType--) | pdf optimization type. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indicates whether to output a blank page when there is nothing to print. |
| [getPageCount()](#getPageCount--) | the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | the 0-based index of the first page to save. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Control/Indicate progress of page saving process. |
| [getPdfCompression()](#getPdfCompression--) | Indicate the compression algorithm |
| [getPrintingPageType()](#getPrintingPageType--) | Indicates which pages will not be printed. |
| [getProducer()](#getProducer--) | producer of generated pdf document. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSecurityOptions()](#getSecurityOptions--) | Set this options, when security is need in xls2pdf result. |
| [getSheetSet()](#getSheetSet--) | the sheets to render. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getTextCrossType()](#getTextCrossType--) | displaying text type when the text width is larger than cell width. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | warning callback. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | For the description of this property, please see [getAllColumnsInOnePagePerSheet()](../../com.aspose.cells/paginatedsaveoptions\#getAllColumnsInOnePagePerSheet--) |
| [setBookmark(PdfBookmarkEntry value)](#setBookmark-com.aspose.cells.PdfBookmarkEntry-) | For the description of this property, please see [getBookmark()](../../com.aspose.cells/pdfsaveoptions\#getBookmark--) |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | For the description of this property, please see [getCachedFileFolder()](../../com.aspose.cells/saveoptions\#getCachedFileFolder--) |
| [setCalculateFormula(boolean value)](#setCalculateFormula-boolean-) | For the description of this property, please see [getCalculateFormula()](../../com.aspose.cells/pdfsaveoptions\#getCalculateFormula--) |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) |  |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | For the description of this property, please see [getCheckWorkbookDefaultFont()](../../com.aspose.cells/paginatedsaveoptions\#getCheckWorkbookDefaultFont--) |
| [setClearData(boolean value)](#setClearData-boolean-) | For the description of this property, please see [getClearData()](../../com.aspose.cells/saveoptions\#getClearData--) |
| [setCompliance(int value)](#setCompliance-int-) | For the description of this property, please see [getCompliance()](../../com.aspose.cells/pdfsaveoptions\#getCompliance--) |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | For the description of this property, please see [getCreateDirectory()](../../com.aspose.cells/saveoptions\#getCreateDirectory--) |
| [setCreatedTime(DateTime value)](#setCreatedTime-com.aspose.cells.DateTime-) | For the description of this property, please see [getCreatedTime()](../../com.aspose.cells/pdfsaveoptions\#getCreatedTime--) |
| [setCustomPropertiesExport(int value)](#setCustomPropertiesExport-int-) | For the description of this property, please see [getCustomPropertiesExport()](../../com.aspose.cells/pdfsaveoptions\#getCustomPropertiesExport--) |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | For the description of this property, please see [getDefaultEditLanguage()](../../com.aspose.cells/paginatedsaveoptions\#getDefaultEditLanguage--) |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | For the description of this property, please see [getDefaultFont()](../../com.aspose.cells/paginatedsaveoptions\#getDefaultFont--) |
| [setDisplayDocTitle(boolean value)](#setDisplayDocTitle-boolean-) | For the description of this property, please see [getDisplayDocTitle()](../../com.aspose.cells/pdfsaveoptions\#getDisplayDocTitle--) |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | For the description of this property, please see [getDrawObjectEventHandler()](../../com.aspose.cells/paginatedsaveoptions\#getDrawObjectEventHandler--) |
| [setEmbedStandardWindowsFonts(boolean value)](#setEmbedStandardWindowsFonts-boolean-) | For the description of this property, please see [getEmbedStandardWindowsFonts()](../../com.aspose.cells/pdfsaveoptions\#getEmbedStandardWindowsFonts--) |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | For the description of this property, please see [getEmfRenderSetting()](../../com.aspose.cells/pdfsaveoptions\#getEmfRenderSetting--) |
| [setExportDocumentStructure(boolean value)](#setExportDocumentStructure-boolean-) | For the description of this property, please see [getExportDocumentStructure()](../../com.aspose.cells/pdfsaveoptions\#getExportDocumentStructure--) |
| [setFontEncoding(int value)](#setFontEncoding-int-) | For the description of this property, please see [getFontEncoding()](../../com.aspose.cells/pdfsaveoptions\#getFontEncoding--) |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) |  |
| [setGridlineType(int value)](#setGridlineType-int-) | For the description of this property, please see [getGridlineType()](../../com.aspose.cells/paginatedsaveoptions\#getGridlineType--) |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | For the description of this property, please see [getIgnoreError()](../../com.aspose.cells/paginatedsaveoptions\#getIgnoreError--) |
| [setImageResample(int desiredPPI, int jpegQuality)](#setImageResample-int-int-) | Sets desired PPI(pixels per inch) of resample images and jpeg quality. |
| [setImageType(ImageFormat value)](#setImageType-com.aspose.cells.ImageFormat-) | For the description of this property, please see [getImageType()](../../com.aspose.cells/pdfsaveoptions\#getImageType--) |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | For the description of this property, please see [getMergeAreas()](../../com.aspose.cells/saveoptions\#getMergeAreas--) |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | For the description of this property, please see [getOnePagePerSheet()](../../com.aspose.cells/paginatedsaveoptions\#getOnePagePerSheet--) |
| [setOptimizationType(int value)](#setOptimizationType-int-) | For the description of this property, please see [getOptimizationType()](../../com.aspose.cells/pdfsaveoptions\#getOptimizationType--) |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | For the description of this property, please see [getOutputBlankPageWhenNothingToPrint()](../../com.aspose.cells/paginatedsaveoptions\#getOutputBlankPageWhenNothingToPrint--) |
| [setPageCount(int value)](#setPageCount-int-) |  |
| [setPageIndex(int value)](#setPageIndex-int-) |  |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | For the description of this property, please see [getPageSavingCallback()](../../com.aspose.cells/paginatedsaveoptions\#getPageSavingCallback--) |
| [setPdfCompression(int value)](#setPdfCompression-int-) | For the description of this property, please see [getPdfCompression()](../../com.aspose.cells/pdfsaveoptions\#getPdfCompression--) |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | For the description of this property, please see [getPrintingPageType()](../../com.aspose.cells/paginatedsaveoptions\#getPrintingPageType--) |
| [setProducer(String value)](#setProducer-java.lang.String-) | For the description of this property, please see [getProducer()](../../com.aspose.cells/pdfsaveoptions\#getProducer--) |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | For the description of this property, please see [getRefreshChartCache()](../../com.aspose.cells/saveoptions\#getRefreshChartCache--) |
| [setSecurityOptions(PdfSecurityOptions value)](#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-) | For the description of this property, please see [getSecurityOptions()](../../com.aspose.cells/pdfsaveoptions\#getSecurityOptions--) |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | For the description of this property, please see [getSheetSet()](../../com.aspose.cells/paginatedsaveoptions\#getSheetSet--) |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | For the description of this property, please see [getSortExternalNames()](../../com.aspose.cells/saveoptions\#getSortExternalNames--) |
| [setSortNames(boolean value)](#setSortNames-boolean-) | For the description of this property, please see [getSortNames()](../../com.aspose.cells/saveoptions\#getSortNames--) |
| [setTextCrossType(int value)](#setTextCrossType-int-) | For the description of this property, please see [getTextCrossType()](../../com.aspose.cells/paginatedsaveoptions\#getTextCrossType--) |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | For the description of this property, please see [getUpdateSmartArt()](../../com.aspose.cells/saveoptions\#getUpdateSmartArt--) |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.cells/saveoptions\#getValidateMergedAreas--) |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) |  |
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


the [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) object.

**Returns:**
[PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry)
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


The cached file folder is used to store some large data.

**Returns:**
java.lang.String
### getCalculateFormula() {#getCalculateFormula--}
```
public boolean getCalculateFormula()
```


Indicates whether to calculate formulas before saving pdf file. The default value is false.

**Returns:**
boolean
### getCheckFontCompatibility() {#getCheckFontCompatibility--}
```
public boolean getCheckFontCompatibility()
```


Indicates whether to check font compatibility for every character in text. The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

**Returns:**
boolean
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


Workbook converts to pdf will according to PdfCompliance in this property.

**Returns:**
int
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

**Returns:**
boolean
### getCreatedTime() {#getCreatedTime--}
```
public DateTime getCreatedTime()
```


the time of generating the pdf document. if it is not be set, it will be the time of generating the pdf.

**Returns:**
[DateTime](../../com.aspose.cells/datetime)
### getCustomPropertiesExport() {#getCustomPropertiesExport--}
```
public int getCustomPropertiesExport()
```


a value determining the way [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) are exported to PDF file. Default value is None.

**Returns:**
int
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


default edit language. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO.

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


Indicates whether the window's title bar should display the document title. If false, the title bar should instead display the name of the PDF file. Default value is false.

**Returns:**
boolean
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implements this interface to get DrawObject and Bound when rendering.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
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


Setting for rendering Emf metafile. EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When EmfRenderSetting.EMF\_PLUS\_PREFER is set, then EMF+ records will be parsed while rendering to pdf, otherwise only EMF records will be parsed. Default value is EmfRenderSetting.EMF\_ONLY.

**Returns:**
int
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


embedded font encoding in pdf. Default value is PdfFontEncoding.IDENTITY

**Returns:**
int
### getGridlineType() {#getGridlineType--}
```
public int getGridlineType()
```


gridline type. Default is Dotted type.

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


Represents the image type when converting the chart and shape . NOTE: This member is now obsolete. Instead, Chart and Shape are always rendered as vector elements(e.g. point, line) for rendering quality. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[ImageFormat](../../com.aspose.cells/imageformat)
### getMergeAreas() {#getMergeAreas--}
```
public boolean getMergeAreas()
```


Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

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


pdf optimization type. Default value is PdfOptimizationType.STANDARD

**Returns:**
int
### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}
```
public boolean getOutputBlankPageWhenNothingToPrint()
```


Indicates whether to output a blank page when there is nothing to print. Default is true.

**Returns:**
boolean
### getPageCount() {#getPageCount--}
```
public int getPageCount()
```


the number of pages to save. Default is System.Int32.MaxValue which means all pages will be rendered..

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


the 0-based index of the first page to save. Default is 0.

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

**Returns:**
int
### getPrintingPageType() {#getPrintingPageType--}
```
public int getPrintingPageType()
```


Indicates which pages will not be printed. If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.

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


producer of generated pdf document. If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.

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

**Returns:**
int
### getSecurityOptions() {#getSecurityOptions--}
```
public PdfSecurityOptions getSecurityOptions()
```


Set this options, when security is need in xls2pdf result.

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


the sheets to render. Default is all visible sheets in the workbook: \{@link com.aspose.cells.SheetSet.getVisible()\}.

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


displaying text type when the text width is larger than cell width.

**Returns:**
int
### getUpdateSmartArt() {#getUpdateSmartArt--}
```
public boolean getUpdateSmartArt()
```


Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

**Returns:**
boolean
### getValidateMergedAreas() {#getValidateMergedAreas--}
```
public boolean getValidateMergedAreas()
```


Indicates whether validate merged cells before saving the file. The default value is false.

**Returns:**
boolean
### getWarningCallback() {#getWarningCallback--}
```
public IWarningCallback getWarningCallback()
```


warning callback.

**Returns:**
[IWarningCallback](../../com.aspose.cells/iwarningcallback)
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


Indicates whether to only substitute the font of character when the cell font is not compatibility for it. Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

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


For the description of this property, please see [getAllColumnsInOnePagePerSheet()](../../com.aspose.cells/paginatedsaveoptions\#getAllColumnsInOnePagePerSheet--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBookmark(PdfBookmarkEntry value) {#setBookmark-com.aspose.cells.PdfBookmarkEntry-}
```
public void setBookmark(PdfBookmarkEntry value)
```


For the description of this property, please see [getBookmark()](../../com.aspose.cells/pdfsaveoptions\#getBookmark--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../../com.aspose.cells/pdfbookmarkentry) |  |

### setCachedFileFolder(String value) {#setCachedFileFolder-java.lang.String-}
```
public void setCachedFileFolder(String value)
```


For the description of this property, please see [getCachedFileFolder()](../../com.aspose.cells/saveoptions\#getCachedFileFolder--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCalculateFormula(boolean value) {#setCalculateFormula-boolean-}
```
public void setCalculateFormula(boolean value)
```


For the description of this property, please see [getCalculateFormula()](../../com.aspose.cells/pdfsaveoptions\#getCalculateFormula--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckFontCompatibility(boolean value) {#setCheckFontCompatibility-boolean-}
```
public void setCheckFontCompatibility(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckWorkbookDefaultFont(boolean value) {#setCheckWorkbookDefaultFont-boolean-}
```
public void setCheckWorkbookDefaultFont(boolean value)
```


For the description of this property, please see [getCheckWorkbookDefaultFont()](../../com.aspose.cells/paginatedsaveoptions\#getCheckWorkbookDefaultFont--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setClearData(boolean value) {#setClearData-boolean-}
```
public void setClearData(boolean value)
```


For the description of this property, please see [getClearData()](../../com.aspose.cells/saveoptions\#getClearData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCompliance(int value) {#setCompliance-int-}
```
public void setCompliance(int value)
```


For the description of this property, please see [getCompliance()](../../com.aspose.cells/pdfsaveoptions\#getCompliance--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCreateDirectory(boolean value) {#setCreateDirectory-boolean-}
```
public void setCreateDirectory(boolean value)
```


For the description of this property, please see [getCreateDirectory()](../../com.aspose.cells/saveoptions\#getCreateDirectory--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreatedTime(DateTime value) {#setCreatedTime-com.aspose.cells.DateTime-}
```
public void setCreatedTime(DateTime value)
```


For the description of this property, please see [getCreatedTime()](../../com.aspose.cells/pdfsaveoptions\#getCreatedTime--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DateTime](../../com.aspose.cells/datetime) |  |

### setCustomPropertiesExport(int value) {#setCustomPropertiesExport-int-}
```
public void setCustomPropertiesExport(int value)
```


For the description of this property, please see [getCustomPropertiesExport()](../../com.aspose.cells/pdfsaveoptions\#getCustomPropertiesExport--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


For the description of this property, please see [getDefaultEditLanguage()](../../com.aspose.cells/paginatedsaveoptions\#getDefaultEditLanguage--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDefaultFont(String value) {#setDefaultFont-java.lang.String-}
```
public void setDefaultFont(String value)
```


For the description of this property, please see [getDefaultFont()](../../com.aspose.cells/paginatedsaveoptions\#getDefaultFont--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setDisplayDocTitle(boolean value) {#setDisplayDocTitle-boolean-}
```
public void setDisplayDocTitle(boolean value)
```


For the description of this property, please see [getDisplayDocTitle()](../../com.aspose.cells/pdfsaveoptions\#getDisplayDocTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


For the description of this property, please see [getDrawObjectEventHandler()](../../com.aspose.cells/paginatedsaveoptions\#getDrawObjectEventHandler--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedStandardWindowsFonts(boolean value) {#setEmbedStandardWindowsFonts-boolean-}
```
public void setEmbedStandardWindowsFonts(boolean value)
```


For the description of this property, please see [getEmbedStandardWindowsFonts()](../../com.aspose.cells/pdfsaveoptions\#getEmbedStandardWindowsFonts--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEmfRenderSetting(int value) {#setEmfRenderSetting-int-}
```
public void setEmfRenderSetting(int value)
```


For the description of this property, please see [getEmfRenderSetting()](../../com.aspose.cells/pdfsaveoptions\#getEmfRenderSetting--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setExportDocumentStructure(boolean value) {#setExportDocumentStructure-boolean-}
```
public void setExportDocumentStructure(boolean value)
```


For the description of this property, please see [getExportDocumentStructure()](../../com.aspose.cells/pdfsaveoptions\#getExportDocumentStructure--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFontEncoding(int value) {#setFontEncoding-int-}
```
public void setFontEncoding(int value)
```


For the description of this property, please see [getFontEncoding()](../../com.aspose.cells/pdfsaveoptions\#getFontEncoding--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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


For the description of this property, please see [getGridlineType()](../../com.aspose.cells/paginatedsaveoptions\#getGridlineType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


For the description of this property, please see [getIgnoreError()](../../com.aspose.cells/paginatedsaveoptions\#getIgnoreError--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setImageResample(int desiredPPI, int jpegQuality) {#setImageResample-int-int-}
```
public void setImageResample(int desiredPPI, int jpegQuality)
```


Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled.

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


For the description of this property, please see [getImageType()](../../com.aspose.cells/pdfsaveoptions\#getImageType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ImageFormat](../../com.aspose.cells/imageformat) |  |

### setMergeAreas(boolean value) {#setMergeAreas-boolean-}
```
public void setMergeAreas(boolean value)
```


For the description of this property, please see [getMergeAreas()](../../com.aspose.cells/saveoptions\#getMergeAreas--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOnePagePerSheet(boolean value) {#setOnePagePerSheet-boolean-}
```
public void setOnePagePerSheet(boolean value)
```


For the description of this property, please see [getOnePagePerSheet()](../../com.aspose.cells/paginatedsaveoptions\#getOnePagePerSheet--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOptimizationType(int value) {#setOptimizationType-int-}
```
public void setOptimizationType(int value)
```


For the description of this property, please see [getOptimizationType()](../../com.aspose.cells/pdfsaveoptions\#getOptimizationType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setOutputBlankPageWhenNothingToPrint(boolean value) {#setOutputBlankPageWhenNothingToPrint-boolean-}
```
public void setOutputBlankPageWhenNothingToPrint(boolean value)
```


For the description of this property, please see [getOutputBlankPageWhenNothingToPrint()](../../com.aspose.cells/paginatedsaveoptions\#getOutputBlankPageWhenNothingToPrint--)

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


For the description of this property, please see [getPageSavingCallback()](../../com.aspose.cells/paginatedsaveoptions\#getPageSavingCallback--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.cells/ipagesavingcallback) |  |

### setPdfCompression(int value) {#setPdfCompression-int-}
```
public void setPdfCompression(int value)
```


For the description of this property, please see [getPdfCompression()](../../com.aspose.cells/pdfsaveoptions\#getPdfCompression--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrintingPageType(int value) {#setPrintingPageType-int-}
```
public void setPrintingPageType(int value)
```


For the description of this property, please see [getPrintingPageType()](../../com.aspose.cells/paginatedsaveoptions\#getPrintingPageType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setProducer(String value) {#setProducer-java.lang.String-}
```
public void setProducer(String value)
```


For the description of this property, please see [getProducer()](../../com.aspose.cells/pdfsaveoptions\#getProducer--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


For the description of this property, please see [getRefreshChartCache()](../../com.aspose.cells/saveoptions\#getRefreshChartCache--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSecurityOptions(PdfSecurityOptions value) {#setSecurityOptions-com.aspose.cells.PdfSecurityOptions-}
```
public void setSecurityOptions(PdfSecurityOptions value)
```


For the description of this property, please see [getSecurityOptions()](../../com.aspose.cells/pdfsaveoptions\#getSecurityOptions--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfSecurityOptions](../../com.aspose.cells/pdfsecurityoptions) |  |

### setSheetSet(SheetSet value) {#setSheetSet-com.aspose.cells.SheetSet-}
```
public void setSheetSet(SheetSet value)
```


For the description of this property, please see [getSheetSet()](../../com.aspose.cells/paginatedsaveoptions\#getSheetSet--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../../com.aspose.cells/sheetset) |  |

### setSortExternalNames(boolean value) {#setSortExternalNames-boolean-}
```
public void setSortExternalNames(boolean value)
```


For the description of this property, please see [getSortExternalNames()](../../com.aspose.cells/saveoptions\#getSortExternalNames--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setSortNames(boolean value) {#setSortNames-boolean-}
```
public void setSortNames(boolean value)
```


For the description of this property, please see [getSortNames()](../../com.aspose.cells/saveoptions\#getSortNames--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTextCrossType(int value) {#setTextCrossType-int-}
```
public void setTextCrossType(int value)
```


For the description of this property, please see [getTextCrossType()](../../com.aspose.cells/paginatedsaveoptions\#getTextCrossType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpdateSmartArt(boolean value) {#setUpdateSmartArt-boolean-}
```
public void setUpdateSmartArt(boolean value)
```


For the description of this property, please see [getUpdateSmartArt()](../../com.aspose.cells/saveoptions\#getUpdateSmartArt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidateMergedAreas(boolean value) {#setValidateMergedAreas-boolean-}
```
public void setValidateMergedAreas(boolean value)
```


For the description of this property, please see [getValidateMergedAreas()](../../com.aspose.cells/saveoptions\#getValidateMergedAreas--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

