---
title: PclSaveOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the options for saving Pcl file.
type: docs
url: /java/com.aspose.cells/pclsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.SaveOptions](../../com.aspose.cells/saveoptions), [com.aspose.cells.PaginatedSaveOptions](../../com.aspose.cells/paginatedsaveoptions)
```
public class PclSaveOptions extends PaginatedSaveOptions
```

Represents the options for saving Pcl file.
## Constructors

| Constructor | Description |
| --- | --- |
| [PclSaveOptions()](#PclSaveOptions--) | Creates the options for saving pdf file. |
## Methods

| Method | Description |
| --- | --- |
| [addPrinterFont(String fontFullName, String fontPclName)](#addPrinterFont-java.lang.String-java.lang.String-) | Adds information about font that is already added to the printer by manufacturer. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. |
| [getCachedFileFolder()](#getCachedFileFolder--) | The folder for temporary files that may be used as data cache. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--) | Indicates whether to check font compatibility for every character in text. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getClass()](#getClass--) |  |
| [getClearData()](#getClearData--) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getCreateDirectory--) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getCustomRenderSettings()](#getCustomRenderSettings--) | Gets custom settings during rendering. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | Gets default edit language. |
| [getDefaultFont()](#getDefaultFont--) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--) | Implements this interface to get DrawObject and Bound when rendering. |
| [getEmbedFont()](#getEmbedFont--) | Indicates whether to embed font into the output Pcl file. |
| [getEmfRenderSetting()](#getEmfRenderSetting--) | Setting for rendering Emf metafile. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--) | Indicates whether encrypt document properties when saving as .xls file. |
| [getGridlineColor()](#getGridlineColor--) | Gets gridline color. |
| [getGridlineType()](#getGridlineType--) | Gets gridline type. |
| [getIgnoreError()](#getIgnoreError--) | Indicates if you need to hide the error while rendering. |
| [getMergeAreas()](#getMergeAreas--) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getOnePagePerSheet()](#getOnePagePerSheet--) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--) | Indicates whether to output a blank page when there is nothing to print. |
| [getPageCount()](#getPageCount--) | Gets the number of pages to save. |
| [getPageIndex()](#getPageIndex--) | Gets the 0-based index of the first page to save. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Control/Indicate progress of page saving process. |
| [getPrintingPageType()](#getPrintingPageType--) | Indicates which pages will not be printed. |
| [getRefreshChartCache()](#getRefreshChartCache--) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getSaveFormat--) | Gets the save file format. |
| [getSheetSet()](#getSheetSet--) | Gets the sheets to render. |
| [getSortExternalNames()](#getSortExternalNames--) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getSortNames--) | Indicates whether sorting defined names before saving file. |
| [getTextCrossType()](#getTextCrossType--) | Gets displaying text type when the text width is larger than cell width. |
| [getUpdateSmartArt()](#getUpdateSmartArt--) | Indicates whether updating smart art setting. |
| [getValidateMergedAreas()](#getValidateMergedAreas--) | Indicates whether validate merged cells before saving the file. |
| [getWarningCallback()](#getWarningCallback--) | Gets warning callback. |
| [hashCode()](#hashCode--) |  |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllColumnsInOnePagePerSheet(boolean value)](#setAllColumnsInOnePagePerSheet-boolean-) | If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. |
| [setCachedFileFolder(String value)](#setCachedFileFolder-java.lang.String-) | The folder for temporary files that may be used as data cache. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setCheckFontCompatibility(boolean value)](#setCheckFontCompatibility-boolean-) | Indicates whether to check font compatibility for every character in text. |
| [setCheckWorkbookDefaultFont(boolean value)](#setCheckWorkbookDefaultFont-boolean-) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [setClearData(boolean value)](#setClearData-boolean-) | Make the workbook empty after saving the file. |
| [setCreateDirectory(boolean value)](#setCreateDirectory-boolean-) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCustomRenderSettings(CustomRenderSettings value)](#setCustomRenderSettings-com.aspose.cells.CustomRenderSettings-) | Sets custom settings during rendering. |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | Sets default edit language. |
| [setDefaultFont(String value)](#setDefaultFont-java.lang.String-) | When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. |
| [setDrawObjectEventHandler(DrawObjectEventHandler value)](#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-) | Implements this interface to get DrawObject and Bound when rendering. |
| [setEmbedFont(boolean value)](#setEmbedFont-boolean-) | Indicates whether to embed font into the output Pcl file. |
| [setEmfRenderSetting(int value)](#setEmfRenderSetting-int-) | Setting for rendering Emf metafile. |
| [setEncryptDocumentProperties(boolean value)](#setEncryptDocumentProperties-boolean-) | Indicates whether encrypt document properties when saving as .xls file. |
| [setFontSubstitutionCharGranularity(boolean value)](#setFontSubstitutionCharGranularity-boolean-) | Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [setGridlineColor(Color value)](#setGridlineColor-com.aspose.cells.Color-) | Sets gridline color. |
| [setGridlineType(int value)](#setGridlineType-int-) | Sets gridline type. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indicates if you need to hide the error while rendering. |
| [setMergeAreas(boolean value)](#setMergeAreas-boolean-) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setOnePagePerSheet(boolean value)](#setOnePagePerSheet-boolean-) | If OnePagePerSheet is true , all content of one sheet will output to only one page in result. |
| [setOutputBlankPageWhenNothingToPrint(boolean value)](#setOutputBlankPageWhenNothingToPrint-boolean-) | Indicates whether to output a blank page when there is nothing to print. |
| [setPageCount(int value)](#setPageCount-int-) | Sets the number of pages to save. |
| [setPageIndex(int value)](#setPageIndex-int-) | Sets the 0-based index of the first page to save. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.cells.IPageSavingCallback-) | Control/Indicate progress of page saving process. |
| [setPrintingPageType(int value)](#setPrintingPageType-int-) | Indicates which pages will not be printed. |
| [setRefreshChartCache(boolean value)](#setRefreshChartCache-boolean-) | Indicates whether refreshing chart cache data |
| [setSheetSet(SheetSet value)](#setSheetSet-com.aspose.cells.SheetSet-) | Sets the sheets to render. |
| [setSortExternalNames(boolean value)](#setSortExternalNames-boolean-) | Indicates whether sorting external defined names before saving file. |
| [setSortNames(boolean value)](#setSortNames-boolean-) | Indicates whether sorting defined names before saving file. |
| [setTextCrossType(int value)](#setTextCrossType-int-) | Sets displaying text type when the text width is larger than cell width. |
| [setUpdateSmartArt(boolean value)](#setUpdateSmartArt-boolean-) | Indicates whether updating smart art setting. |
| [setValidateMergedAreas(boolean value)](#setValidateMergedAreas-boolean-) | Indicates whether validate merged cells before saving the file. |
| [setWarningCallback(IWarningCallback value)](#setWarningCallback-com.aspose.cells.IWarningCallback-) | Sets warning callback. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PclSaveOptions() {#PclSaveOptions--}
```
public PclSaveOptions()
```


Creates the options for saving pdf file.

### addPrinterFont(String fontFullName, String fontPclName) {#addPrinterFont-java.lang.String-java.lang.String-}
```
public void addPrinterFont(String fontFullName, String fontPclName)
```


Adds information about font that is already added to the printer by manufacturer.

**Remarks**

There are 52 fonts that are to be built in any printer according to Pcl specification. However manufactures can add some other fonts to their devices.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFullName | java.lang.String | Full name of the font (e.g. "Times New Roman Bold Italic") used in the source file. |
| fontPclName | java.lang.String | Name of the font that will be used in the output Pcl document. |

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
### getCachedFileFolder() {#getCachedFileFolder--}
```
public String getCachedFileFolder()
```


The folder for temporary files that may be used as data cache.

**Remarks**

If the folder has not been specified, the default value for it is void

**Returns:**
java.lang.String
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
### getCreateDirectory() {#getCreateDirectory--}
```
public boolean getCreateDirectory()
```


If true and the directory does not exist, the directory will be automatically created before saving the file.

**Remarks**

The default value is false.

**Returns:**
boolean
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
### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}
```
public DrawObjectEventHandler getDrawObjectEventHandler()
```


Implements this interface to get DrawObject and Bound when rendering.

**Returns:**
[DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler)
### getEmbedFont() {#getEmbedFont--}
```
public boolean getEmbedFont()
```


Indicates whether to embed font into the output Pcl file.

**Remarks**

The default value is true.

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

### setDrawObjectEventHandler(DrawObjectEventHandler value) {#setDrawObjectEventHandler-com.aspose.cells.DrawObjectEventHandler-}
```
public void setDrawObjectEventHandler(DrawObjectEventHandler value)
```


Implements this interface to get DrawObject and Bound when rendering.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../../com.aspose.cells/drawobjecteventhandler) |  |

### setEmbedFont(boolean value) {#setEmbedFont-boolean-}
```
public void setEmbedFont(boolean value)
```


Indicates whether to embed font into the output Pcl file.

**Remarks**

The default value is true.

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

### setRefreshChartCache(boolean value) {#setRefreshChartCache-boolean-}
```
public void setRefreshChartCache(boolean value)
```


Indicates whether refreshing chart cache data

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

