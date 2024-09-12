---
title: PdfSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options for saving pdf file.
type: docs
url: /nodejs-cpp/pdfsaveoptions/
---

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

## Methods

| Method | Description |
| --- | --- |
| [getEmbedStandardWindowsFonts()](#getEmbedStandardWindowsFonts--)| True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true. |
| [setEmbedStandardWindowsFonts(boolean)](#setEmbedStandardWindowsFonts-boolean-)| True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true. |
| [getBookmark()](#getBookmark--)| Gets and sets the <see cref ="PdfBookmarkEntry">PdfBookmarkEntry</see> object. |
| [setBookmark(PdfBookmarkEntry)](#setBookmark-pdfbookmarkentry-)| Gets and sets the <see cref ="PdfBookmarkEntry">PdfBookmarkEntry</see> object. |
| [getCompliance()](#getCompliance--)| Gets or sets the PDF standards compliance level for output documents. |
| [setCompliance(PdfCompliance)](#setCompliance-pdfcompliance-)| Gets or sets the PDF standards compliance level for output documents. |
| [getSecurityOptions()](#getSecurityOptions--)| Set this options, when security is need in xls2pdf result. |
| [setSecurityOptions(PdfSecurityOptions)](#setSecurityOptions-pdfsecurityoptions-)| Set this options, when security is need in xls2pdf result. |
| [getCalculateFormula()](#getCalculateFormula--)| Indicates whether to calculate formulas before saving pdf file. |
| [setCalculateFormula(boolean)](#setCalculateFormula-boolean-)| Indicates whether to calculate formulas before saving pdf file. |
| [getPdfCompression()](#getPdfCompression--)| Indicate the compression algorithm |
| [setPdfCompression(PdfCompressionCore)](#setPdfCompression-pdfcompressioncore-)| Indicate the compression algorithm |
| [getCreatedTime()](#getCreatedTime--)| Gets and sets the time of generating the pdf document. |
| [setCreatedTime(Date)](#setCreatedTime-date-)| Gets and sets the time of generating the pdf document. |
| [getProducer()](#getProducer--)| Gets and sets producer of generated pdf document. |
| [setProducer(string)](#setProducer-string-)| Gets and sets producer of generated pdf document. |
| [getOptimizationType()](#getOptimizationType--)| Gets and sets pdf optimization type. |
| [setOptimizationType(PdfOptimizationType)](#setOptimizationType-pdfoptimizationtype-)| Gets and sets pdf optimization type. |
| [getCustomPropertiesExport()](#getCustomPropertiesExport--)| Gets or sets a value determining the way [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) are exported to PDF file. Default value is None. |
| [setCustomPropertiesExport(PdfCustomPropertiesExport)](#setCustomPropertiesExport-pdfcustompropertiesexport-)| Gets or sets a value determining the way [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) are exported to PDF file. Default value is None. |
| [getExportDocumentStructure()](#getExportDocumentStructure--)| Indicates whether to export document structure. |
| [setExportDocumentStructure(boolean)](#setExportDocumentStructure-boolean-)| Indicates whether to export document structure. |
| [getDisplayDocTitle()](#getDisplayDocTitle--)| Indicates whether the window's title bar should display the document title. |
| [setDisplayDocTitle(boolean)](#setDisplayDocTitle-boolean-)| Indicates whether the window's title bar should display the document title. |
| [getFontEncoding()](#getFontEncoding--)| Gets or sets embedded font encoding in pdf. |
| [setFontEncoding(PdfFontEncoding)](#setFontEncoding-pdffontencoding-)| Gets or sets embedded font encoding in pdf. |
| [getWatermark()](#getWatermark--)| Gets or sets watermark to output. |
| [setWatermark(RenderingWatermark)](#setWatermark-renderingwatermark-)| Gets or sets watermark to output. |
| [getEmbedAttachments()](#getEmbedAttachments--)| Indicates whether to embed attachment for Ole objects in Excel. |
| [setEmbedAttachments(boolean)](#setEmbedAttachments-boolean-)| Indicates whether to embed attachment for Ole objects in Excel. |
| [setImageResample(number, number)](#setImageResample-number-number-)| Sets desired PPI(pixels per inch) of resample images and jpeg quality. All images will be converted to JPEG with the specified quality setting, and images that are greater than the specified PPI (pixels per inch) will be resampled. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getSaveFormat()](#getSaveFormat--)| Gets the save file format. |
| [getClearData()](#getClearData--)| Make the workbook empty after saving the file. |
| [setClearData(boolean)](#setClearData-boolean-)| Make the workbook empty after saving the file. |
| [getCachedFileFolder()](#getCachedFileFolder--)| The cached file folder is used to store some large data. |
| [setCachedFileFolder(string)](#setCachedFileFolder-string-)| The cached file folder is used to store some large data. |
| [getValidateMergedAreas()](#getValidateMergedAreas--)| Indicates whether validate merged cells before saving the file. |
| [setValidateMergedAreas(boolean)](#setValidateMergedAreas-boolean-)| Indicates whether validate merged cells before saving the file. |
| [getMergeAreas()](#getMergeAreas--)| Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setMergeAreas(boolean)](#setMergeAreas-boolean-)| Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getCreateDirectory()](#getCreateDirectory--)| If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCreateDirectory(boolean)](#setCreateDirectory-boolean-)| If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getSortNames()](#getSortNames--)| Indicates whether sorting defined names before saving file. |
| [setSortNames(boolean)](#setSortNames-boolean-)| Indicates whether sorting defined names before saving file. |
| [getSortExternalNames()](#getSortExternalNames--)| Indicates whether sorting external defined names before saving file. |
| [setSortExternalNames(boolean)](#setSortExternalNames-boolean-)| Indicates whether sorting external defined names before saving file. |
| [getRefreshChartCache()](#getRefreshChartCache--)| Indicates whether refreshing chart cache data |
| [setRefreshChartCache(boolean)](#setRefreshChartCache-boolean-)| Indicates whether refreshing chart cache data |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| Gets or sets warning callback. |
| [getUpdateSmartArt()](#getUpdateSmartArt--)| Indicates whether updating smart art setting. The default value is false. |
| [setUpdateSmartArt(boolean)](#setUpdateSmartArt-boolean-)| Indicates whether updating smart art setting. The default value is false. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--)| Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [setEncryptDocumentProperties(boolean)](#setEncryptDocumentProperties-boolean-)| Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [getDefaultFont()](#getDefaultFont--)| When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [setDefaultFont(string)](#setDefaultFont-string-)| When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters. |
| [getCheckWorkbookDefaultFont()](#getCheckWorkbookDefaultFont--)| When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [setCheckWorkbookDefaultFont(boolean)](#setCheckWorkbookDefaultFont-boolean-)| When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first. |
| [setCheckFontCompatibility(boolean)](#setCheckFontCompatibility-boolean-)| Indicates whether to check font compatibility for every character in text. |
| [getCheckFontCompatibility()](#getCheckFontCompatibility--)| Indicates whether to check font compatibility for every character in text. |
| [setIsFontSubstitutionCharGranularity(boolean)](#setIsFontSubstitutionCharGranularity-boolean-)| Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [isFontSubstitutionCharGranularity()](#isFontSubstitutionCharGranularity--)| Indicates whether to only substitute the font of character when the cell font is not compatibility for it. |
| [getOnePagePerSheet()](#getOnePagePerSheet--)| If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [setOnePagePerSheet(boolean)](#setOnePagePerSheet-boolean-)| If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect. |
| [getAllColumnsInOnePagePerSheet()](#getAllColumnsInOnePagePerSheet--)| If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect. |
| [setAllColumnsInOnePagePerSheet(boolean)](#setAllColumnsInOnePagePerSheet-boolean-)| If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect. |
| [getIgnoreError()](#getIgnoreError--)| Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [setIgnoreError(boolean)](#setIgnoreError-boolean-)| Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc. |
| [getOutputBlankPageWhenNothingToPrint()](#getOutputBlankPageWhenNothingToPrint--)| Indicates whether to output a blank page when there is nothing to print. |
| [setOutputBlankPageWhenNothingToPrint(boolean)](#setOutputBlankPageWhenNothingToPrint-boolean-)| Indicates whether to output a blank page when there is nothing to print. |
| [setPageIndex(number)](#setPageIndex-number-)| Gets or sets the 0-based index of the first page to save. |
| [getPageIndex()](#getPageIndex--)| Gets or sets the 0-based index of the first page to save. |
| [setPageCount(number)](#setPageCount-number-)| Gets or sets the number of pages to save. |
| [getPageCount()](#getPageCount--)| Gets or sets the number of pages to save. |
| [getPrintingPageType()](#getPrintingPageType--)| Indicates which pages will not be printed. |
| [setPrintingPageType(PrintingPageType)](#setPrintingPageType-printingpagetype-)| Indicates which pages will not be printed. |
| [getGridlineType()](#getGridlineType--)| Gets or sets gridline type. |
| [setGridlineType(GridlineType)](#setGridlineType-gridlinetype-)| Gets or sets gridline type. |
| [getTextCrossType()](#getTextCrossType--)| Gets or sets displaying text type when the text width is larger than cell width. |
| [setTextCrossType(TextCrossType)](#setTextCrossType-textcrosstype-)| Gets or sets displaying text type when the text width is larger than cell width. |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--)| Gets or sets default edit language. |
| [setDefaultEditLanguage(DefaultEditLanguage)](#setDefaultEditLanguage-defaulteditlanguage-)| Gets or sets default edit language. |
| [getSheetSet()](#getSheetSet--)| Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [setSheetSet(SheetSet)](#setSheetSet-sheetset-)| Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/). |
| [getDrawObjectEventHandler()](#getDrawObjectEventHandler--)| Implements this interface to get DrawObject and Bound when rendering. |
| [setDrawObjectEventHandler(DrawObjectEventHandler)](#setDrawObjectEventHandler-drawobjecteventhandler-)| Implements this interface to get DrawObject and Bound when rendering. |
| [getPageSavingCallback()](#getPageSavingCallback--)| Control/Indicate progress of page saving process. |
| [setPageSavingCallback(IPageSavingCallback)](#setPageSavingCallback-ipagesavingcallback-)| Control/Indicate progress of page saving process. |
| [getEmfRenderSetting()](#getEmfRenderSetting--)| Setting for rendering Emf metafile. |
| [setEmfRenderSetting(EmfRenderSetting)](#setEmfRenderSetting-emfrendersetting-)| Setting for rendering Emf metafile. |


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

### getEmbedStandardWindowsFonts() {#getEmbedStandardWindowsFonts--}

True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.

```javascript
getEmbedStandardWindowsFonts() : boolean;
```


### setEmbedStandardWindowsFonts(boolean) {#setEmbedStandardWindowsFonts-boolean-}

True to embed true type fonts. Affects only ASCII characters 32-127. Fonts for character codes greater than 127 are always embedded. Fonts are always embedded for PDF/A-1a, PDF/A-1b standard. Default is true.

```javascript
setEmbedStandardWindowsFonts(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getBookmark() {#getBookmark--}

Gets and sets the <see cref ="PdfBookmarkEntry">PdfBookmarkEntry</see> object.

```javascript
getBookmark() : PdfBookmarkEntry;
```


**Returns**

[PdfBookmarkEntry](../pdfbookmarkentry/)

### setBookmark(PdfBookmarkEntry) {#setBookmark-pdfbookmarkentry-}

Gets and sets the <see cref ="PdfBookmarkEntry">PdfBookmarkEntry</see> object.

```javascript
setBookmark(value: PdfBookmarkEntry) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfBookmarkEntry](../pdfbookmarkentry/) | The value to set. |

### getCompliance() {#getCompliance--}

Gets or sets the PDF standards compliance level for output documents.

```javascript
getCompliance() : PdfCompliance;
```


**Returns**

[PdfCompliance](../pdfcompliance/)

**Remarks**

Default is Pdf17.

### setCompliance(PdfCompliance) {#setCompliance-pdfcompliance-}

Gets or sets the PDF standards compliance level for output documents.

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

Set this options, when security is need in xls2pdf result.

```javascript
getSecurityOptions() : PdfSecurityOptions;
```


**Returns**

[PdfSecurityOptions](../pdfsecurityoptions/)

### setSecurityOptions(PdfSecurityOptions) {#setSecurityOptions-pdfsecurityoptions-}

Set this options, when security is need in xls2pdf result.

```javascript
setSecurityOptions(value: PdfSecurityOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfSecurityOptions](../pdfsecurityoptions/) | The value to set. |

### getCalculateFormula() {#getCalculateFormula--}

Indicates whether to calculate formulas before saving pdf file.

```javascript
getCalculateFormula() : boolean;
```


**Remarks**

The default value is false.

### setCalculateFormula(boolean) {#setCalculateFormula-boolean-}

Indicates whether to calculate formulas before saving pdf file.

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

Indicate the compression algorithm

```javascript
getPdfCompression() : PdfCompressionCore;
```


**Returns**

[PdfCompressionCore](../pdfcompressioncore/)

### setPdfCompression(PdfCompressionCore) {#setPdfCompression-pdfcompressioncore-}

Indicate the compression algorithm

```javascript
setPdfCompression(value: PdfCompressionCore) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfCompressionCore](../pdfcompressioncore/) | The value to set. |

### getCreatedTime() {#getCreatedTime--}

Gets and sets the time of generating the pdf document.

```javascript
getCreatedTime() : Date;
```


**Remarks**

if it is not be set, it will be the time of generating the pdf.

### setCreatedTime(Date) {#setCreatedTime-date-}

Gets and sets the time of generating the pdf document.

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

Gets and sets producer of generated pdf document.

```javascript
getProducer() : string;
```


**Remarks**

If the value is null, or a valid LICENSE is not set, string Aspose.Cells vVERSION will be used.

### setProducer(string) {#setProducer-string-}

Gets and sets producer of generated pdf document.

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

Gets and sets pdf optimization type.

```javascript
getOptimizationType() : PdfOptimizationType;
```


**Returns**

[PdfOptimizationType](../pdfoptimizationtype/)

**Remarks**

Default value is [PdfOptimizationType.Standard](../pdfoptimizationtype.standard/)

### setOptimizationType(PdfOptimizationType) {#setOptimizationType-pdfoptimizationtype-}

Gets and sets pdf optimization type.

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

Gets or sets a value determining the way [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) are exported to PDF file. Default value is None.

```javascript
getCustomPropertiesExport() : PdfCustomPropertiesExport;
```


**Returns**

[PdfCustomPropertiesExport](../pdfcustompropertiesexport/)

### setCustomPropertiesExport(PdfCustomPropertiesExport) {#setCustomPropertiesExport-pdfcustompropertiesexport-}

Gets or sets a value determining the way [CustomDocumentPropertyCollection](../customdocumentpropertycollection/) are exported to PDF file. Default value is None.

```javascript
setCustomPropertiesExport(value: PdfCustomPropertiesExport) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PdfCustomPropertiesExport](../pdfcustompropertiesexport/) | The value to set. |

### getExportDocumentStructure() {#getExportDocumentStructure--}

Indicates whether to export document structure.

```javascript
getExportDocumentStructure() : boolean;
```


### setExportDocumentStructure(boolean) {#setExportDocumentStructure-boolean-}

Indicates whether to export document structure.

```javascript
setExportDocumentStructure(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDisplayDocTitle() {#getDisplayDocTitle--}

Indicates whether the window's title bar should display the document title.

```javascript
getDisplayDocTitle() : boolean;
```


**Remarks**

If false, the title bar should instead display the name of the PDF file. Default value is false.

### setDisplayDocTitle(boolean) {#setDisplayDocTitle-boolean-}

Indicates whether the window's title bar should display the document title.

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

Gets or sets embedded font encoding in pdf.

```javascript
getFontEncoding() : PdfFontEncoding;
```


**Returns**

[PdfFontEncoding](../pdffontencoding/)

**Remarks**

Default value is [PdfFontEncoding.Identity](../pdffontencoding.identity/)

### setFontEncoding(PdfFontEncoding) {#setFontEncoding-pdffontencoding-}

Gets or sets embedded font encoding in pdf.

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

Gets or sets watermark to output.

```javascript
getWatermark() : RenderingWatermark;
```


**Returns**

[RenderingWatermark](../renderingwatermark/)

### setWatermark(RenderingWatermark) {#setWatermark-renderingwatermark-}

Gets or sets watermark to output.

```javascript
setWatermark(value: RenderingWatermark) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [RenderingWatermark](../renderingwatermark/) | The value to set. |

### getEmbedAttachments() {#getEmbedAttachments--}

Indicates whether to embed attachment for Ole objects in Excel.

```javascript
getEmbedAttachments() : boolean;
```


**Remarks**

Default value is false. The value must be false when PDF/A compliance is set or pdf encryption is enabled.

### setEmbedAttachments(boolean) {#setEmbedAttachments-boolean-}

Indicates whether to embed attachment for Ole objects in Excel.

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

Gets the save file format.

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](../saveformat/)

### getClearData() {#getClearData--}

Make the workbook empty after saving the file.

```javascript
getClearData() : boolean;
```


### setClearData(boolean) {#setClearData-boolean-}

Make the workbook empty after saving the file.

```javascript
setClearData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCachedFileFolder() {#getCachedFileFolder--}

The cached file folder is used to store some large data.

```javascript
getCachedFileFolder() : string;
```


### setCachedFileFolder(string) {#setCachedFileFolder-string-}

The cached file folder is used to store some large data.

```javascript
setCachedFileFolder(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getValidateMergedAreas() {#getValidateMergedAreas--}

Indicates whether validate merged cells before saving the file.

```javascript
getValidateMergedAreas() : boolean;
```


**Remarks**

The default value is false.

### setValidateMergedAreas(boolean) {#setValidateMergedAreas-boolean-}

Indicates whether validate merged cells before saving the file.

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

Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
getMergeAreas() : boolean;
```


**Remarks**

The default value is false.

### setMergeAreas(boolean) {#setMergeAreas-boolean-}

Indicates whether merge the areas of conditional formatting and validation before saving the file.

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

If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
getCreateDirectory() : boolean;
```


**Remarks**

The default value is false.

### setCreateDirectory(boolean) {#setCreateDirectory-boolean-}

If true and the directory does not exist, the directory will be automatically created before saving the file.

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

Indicates whether sorting defined names before saving file.

```javascript
getSortNames() : boolean;
```


### setSortNames(boolean) {#setSortNames-boolean-}

Indicates whether sorting defined names before saving file.

```javascript
setSortNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSortExternalNames() {#getSortExternalNames--}

Indicates whether sorting external defined names before saving file.

```javascript
getSortExternalNames() : boolean;
```


### setSortExternalNames(boolean) {#setSortExternalNames-boolean-}

Indicates whether sorting external defined names before saving file.

```javascript
setSortExternalNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshChartCache() {#getRefreshChartCache--}

Indicates whether refreshing chart cache data

```javascript
getRefreshChartCache() : boolean;
```


### setRefreshChartCache(boolean) {#setRefreshChartCache-boolean-}

Indicates whether refreshing chart cache data

```javascript
setRefreshChartCache(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](../iwarningcallback/)

### getUpdateSmartArt() {#getUpdateSmartArt--}

Indicates whether updating smart art setting. The default value is false.

```javascript
getUpdateSmartArt() : boolean;
```


**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setUpdateSmartArt(boolean) {#setUpdateSmartArt-boolean-}

Indicates whether updating smart art setting. The default value is false.

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

Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
getEncryptDocumentProperties() : boolean;
```


**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.

### setEncryptDocumentProperties(boolean) {#setEncryptDocumentProperties-boolean-}

Indicates whether encrypt document properties when saving as .xls file. The default value is true.

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

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
getDefaultFont() : string;
```


### setDefaultFont(string) {#setDefaultFont-string-}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
setDefaultFont(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```javascript
getCheckWorkbookDefaultFont() : boolean;
```


**Remarks**

Default is true.

### setCheckWorkbookDefaultFont(boolean) {#setCheckWorkbookDefaultFont-boolean-}

When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

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

Indicates whether to check font compatibility for every character in text.

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

Indicates whether to check font compatibility for every character in text.

```javascript
getCheckFontCompatibility() : boolean;
```


**Remarks**

The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

### setIsFontSubstitutionCharGranularity(boolean) {#setIsFontSubstitutionCharGranularity-boolean-}

Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

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

Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

```javascript
isFontSubstitutionCharGranularity() : boolean;
```


**Remarks**

Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### getOnePagePerSheet() {#getOnePagePerSheet--}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
getOnePagePerSheet() : boolean;
```


### setOnePagePerSheet(boolean) {#setOnePagePerSheet-boolean-}

If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
setOnePagePerSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

```javascript
getAllColumnsInOnePagePerSheet() : boolean;
```


### setAllColumnsInOnePagePerSheet(boolean) {#setAllColumnsInOnePagePerSheet-boolean-}

If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

```javascript
setAllColumnsInOnePagePerSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIgnoreError() {#getIgnoreError--}

Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

```javascript
getIgnoreError() : boolean;
```


### setIgnoreError(boolean) {#setIgnoreError-boolean-}

Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

```javascript
setIgnoreError(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}

Indicates whether to output a blank page when there is nothing to print.

```javascript
getOutputBlankPageWhenNothingToPrint() : boolean;
```


**Remarks**

Default is true.

### setOutputBlankPageWhenNothingToPrint(boolean) {#setOutputBlankPageWhenNothingToPrint-boolean-}

Indicates whether to output a blank page when there is nothing to print.

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

Gets or sets the 0-based index of the first page to save.

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

Gets or sets the 0-based index of the first page to save.

```javascript
getPageIndex() : number;
```


**Remarks**

Default is 0.

### setPageCount(number) {#setPageCount-number-}

Gets or sets the number of pages to save.

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

Gets or sets the number of pages to save.

```javascript
getPageCount() : number;
```


**Remarks**

Default is System.Int32.MaxValue which means all pages will be rendered..

### getPrintingPageType() {#getPrintingPageType--}

Indicates which pages will not be printed.

```javascript
getPrintingPageType() : PrintingPageType;
```


**Returns**

[PrintingPageType](../printingpagetype/)

**Remarks**

If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.

### setPrintingPageType(PrintingPageType) {#setPrintingPageType-printingpagetype-}

Indicates which pages will not be printed.

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

Gets or sets gridline type.

```javascript
getGridlineType() : GridlineType;
```


**Returns**

[GridlineType](../gridlinetype/)

**Remarks**

Default is Dotted type.

### setGridlineType(GridlineType) {#setGridlineType-gridlinetype-}

Gets or sets gridline type.

```javascript
setGridlineType(value: GridlineType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridlineType](../gridlinetype/) | The value to set. |

**Remarks**

Default is Dotted type.

### getTextCrossType() {#getTextCrossType--}

Gets or sets displaying text type when the text width is larger than cell width.

```javascript
getTextCrossType() : TextCrossType;
```


**Returns**

[TextCrossType](../textcrosstype/)

### setTextCrossType(TextCrossType) {#setTextCrossType-textcrosstype-}

Gets or sets displaying text type when the text width is larger than cell width.

```javascript
setTextCrossType(value: TextCrossType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextCrossType](../textcrosstype/) | The value to set. |

### getDefaultEditLanguage() {#getDefaultEditLanguage--}

Gets or sets default edit language.

```javascript
getDefaultEditLanguage() : DefaultEditLanguage;
```


**Returns**

[DefaultEditLanguage](../defaulteditlanguage/)

**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).

### setDefaultEditLanguage(DefaultEditLanguage) {#setDefaultEditLanguage-defaulteditlanguage-}

Gets or sets default edit language.

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

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
getSheetSet() : SheetSet;
```


**Returns**

[SheetSet](../sheetset/)

### setSheetSet(SheetSet) {#setSheetSet-sheetset-}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
setSheetSet(value: SheetSet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../sheetset/) | The value to set. |

### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}

Implements this interface to get DrawObject and Bound when rendering.

```javascript
getDrawObjectEventHandler() : DrawObjectEventHandler;
```


**Returns**

[DrawObjectEventHandler](../drawobjecteventhandler/)

### setDrawObjectEventHandler(DrawObjectEventHandler) {#setDrawObjectEventHandler-drawobjecteventhandler-}

Implements this interface to get DrawObject and Bound when rendering.

```javascript
setDrawObjectEventHandler(value: DrawObjectEventHandler) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../drawobjecteventhandler/) | The value to set. |

### getPageSavingCallback() {#getPageSavingCallback--}

Control/Indicate progress of page saving process.

```javascript
getPageSavingCallback() : IPageSavingCallback;
```


**Returns**

[IPageSavingCallback](../ipagesavingcallback/)

### setPageSavingCallback(IPageSavingCallback) {#setPageSavingCallback-ipagesavingcallback-}

Control/Indicate progress of page saving process.

```javascript
setPageSavingCallback(value: IPageSavingCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../ipagesavingcallback/) | The value to set. |

### getEmfRenderSetting() {#getEmfRenderSetting--}

Setting for rendering Emf metafile.

```javascript
getEmfRenderSetting() : EmfRenderSetting;
```


**Returns**

[EmfRenderSetting](../emfrendersetting/)

**Remarks**

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/).

### setEmfRenderSetting(EmfRenderSetting) {#setEmfRenderSetting-emfrendersetting-}

Setting for rendering Emf metafile.

```javascript
setEmfRenderSetting(value: EmfRenderSetting) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EmfRenderSetting](../emfrendersetting/) | The value to set. |

**Remarks**

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/).


