﻿---
title: PptxSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the pptx save options.
type: docs
url: /nodejs-cpp/pptxsaveoptions/
---

## PptxSaveOptions class

Represents the pptx save options.

```javascript
class PptxSaveOptions extends PaginatedSaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Represents the pptx save options. |
| [constructor(PaginatedSaveOptions)](#constructor-paginatedsaveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(boolean)](#constructor-boolean-)| Represents options of saving .pptx file. |

## Methods

| Method | Description |
| --- | --- |
| [getIgnoreHiddenRows()](#getIgnoreHiddenRows--)| Inidicates whether ignoring hidden rows when converting Excel to PowerPoint. |
| [setIgnoreHiddenRows(boolean)](#setIgnoreHiddenRows-boolean-)| Inidicates whether ignoring hidden rows when converting Excel to PowerPoint. |
| [getAdjustFontSizeForRowType()](#getAdjustFontSizeForRowType--)| Represents what type of line needs to be adjusted size of font if height of row is small. |
| [setAdjustFontSizeForRowType(AdjustFontSizeForRowType)](#setAdjustFontSizeForRowType-adjustfontsizeforrowtype-)| Represents what type of line needs to be adjusted size of font if height of row is small. |
| [getExportViewType()](#getExportViewType--)| Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing. |
| [setExportViewType(SlideViewType)](#setExportViewType-slideviewtype-)| Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing. |
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
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
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
| [getGridlineColor()](#getGridlineColor--)| Gets or sets gridline colr. |
| [setGridlineColor(Color)](#setGridlineColor-color-)| Gets or sets gridline colr. |
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

Represents the pptx save options.

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

### constructor(boolean) {#constructor-boolean-}

Represents options of saving .pptx file.

```javascript
constructor(saveAsImage: boolean);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveAsImage | boolean | If True, the workbook will be converted into some pictures of .pptx file.         /// If False, the workbook will be converted into some tables of .pptx file. |

### getIgnoreHiddenRows() {#getIgnoreHiddenRows--}

Inidicates whether ignoring hidden rows when converting Excel to PowerPoint.

```javascript
getIgnoreHiddenRows() : boolean;
```


### setIgnoreHiddenRows(boolean) {#setIgnoreHiddenRows-boolean-}

Inidicates whether ignoring hidden rows when converting Excel to PowerPoint.

```javascript
setIgnoreHiddenRows(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAdjustFontSizeForRowType() {#getAdjustFontSizeForRowType--}

Represents what type of line needs to be adjusted size of font if height of row is small.

```javascript
getAdjustFontSizeForRowType() : AdjustFontSizeForRowType;
```


**Returns**

[AdjustFontSizeForRowType](../adjustfontsizeforrowtype/)

### setAdjustFontSizeForRowType(AdjustFontSizeForRowType) {#setAdjustFontSizeForRowType-adjustfontsizeforrowtype-}

Represents what type of line needs to be adjusted size of font if height of row is small.

```javascript
setAdjustFontSizeForRowType(value: AdjustFontSizeForRowType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AdjustFontSizeForRowType](../adjustfontsizeforrowtype/) | The value to set. |

### getExportViewType() {#getExportViewType--}

Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing.

```javascript
getExportViewType() : SlideViewType;
```


**Returns**

[SlideViewType](../slideviewtype/)

### setExportViewType(SlideViewType) {#setExportViewType-slideviewtype-}

Gets and sets the display type when exporting to PowerPoint. The default exporting type is working as printing.

```javascript
setExportViewType(value: SlideViewType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SlideViewType](../slideviewtype/) | The value to set. |

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

### getCheckExcelRestriction() {#getCheckExcelRestriction--}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
getCheckExcelRestriction() : boolean;
```


### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
setCheckExcelRestriction(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

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

### getGridlineColor() {#getGridlineColor--}

Gets or sets gridline colr.

```javascript
getGridlineColor() : Color;
```


**Returns**

[Color](../color/)

**Remarks**

It will ignore the gridline color settings in the source file.

### setGridlineColor(Color) {#setGridlineColor-color-}

Gets or sets gridline colr.

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


