---
title: PclSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options for saving a Pcl file.
type: docs
url: /nodejs-cpp/pclsaveoptions/
---

## PclSaveOptions class

Represents the options for saving a Pcl file.

```javascript
class PclSaveOptions extends PaginatedSaveOptions;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options for saving pdf file. |
| [constructor(PaginatedSaveOptions)](#constructor-paginatedsaveoptions-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [embedFont](#embedFont--)| boolean | Indicates whether to embed font into the output Pcl file. |
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
| [getEmbedFont()](#getEmbedFont--)| <b>@deprecated.</b> Please use the 'embedFont' property instead. Indicates whether to embed font into the output Pcl file. |
| [setEmbedFont(boolean)](#setEmbedFont-boolean-)| <b>@deprecated.</b> Please use the 'embedFont' property instead. Indicates whether to embed font into the output Pcl file. |
| [addPrinterFont(string, string)](#addPrinterFont-string-string-)| Adds information about font that is already added to the printer by manufacturer. |
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

### embedFont {#embedFont--}

Indicates whether to embed font into the output Pcl file.

```javascript
embedFont : boolean;
```


**Remarks**

The default value is true.

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


### getEmbedFont() {#getEmbedFont--}

<b>@deprecated.</b> Please use the 'embedFont' property instead. Indicates whether to embed font into the output Pcl file.

```javascript
getEmbedFont() : boolean;
```


**Remarks**

The default value is true.

### setEmbedFont(boolean) {#setEmbedFont-boolean-}

<b>@deprecated.</b> Please use the 'embedFont' property instead. Indicates whether to embed font into the output Pcl file.

```javascript
setEmbedFont(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is true.

### addPrinterFont(string, string) {#addPrinterFont-string-string-}

Adds information about font that is already added to the printer by manufacturer.

```javascript
addPrinterFont(fontFullName: string, fontPclName: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fontFullName | string | Full name of the font (e.g. "Times New Roman Bold Italic") used in the source file. |
| fontPclName | string | Name of the font that will be used in the output Pcl document. |

**Remarks**

There are 52 fonts that are to be built in any printer according to Pcl specification. However manufactures can add some other fonts to their devices.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getSaveFormat() {#getSaveFormat--}

<b>@deprecated.</b> Please use the 'saveFormat' property instead. Gets the save file format.

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](../saveformat/)

### getClearData() {#getClearData--}

<b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file.

```javascript
getClearData() : boolean;
```


### setClearData(boolean) {#setClearData-boolean-}

<b>@deprecated.</b> Please use the 'clearData' property instead. Make the workbook empty after saving the file.

```javascript
setClearData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCachedFileFolder() {#getCachedFileFolder--}

<b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache.

```javascript
getCachedFileFolder() : string;
```


**Remarks**

If the folder has not been specified, the default value for it is [CellsHelper.GetCacheFolder()](../cellshelper.getcachefolder()/). If its default value is null or empty, or has been specified as null or empty, then no cache file will be used when saving the workbook.

### setCachedFileFolder(string) {#setCachedFileFolder-string-}

<b>@deprecated.</b> Please use the 'cachedFileFolder' property instead. The folder for temporary files that may be used as data cache.

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

<b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file.

```javascript
getValidateMergedAreas() : boolean;
```


**Remarks**

The default value is false.

### setValidateMergedAreas(boolean) {#setValidateMergedAreas-boolean-}

<b>@deprecated.</b> Please use the 'validateMergedAreas' property instead. Indicates whether validate merged cells before saving the file.

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

<b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
getMergeAreas() : boolean;
```


**Remarks**

The default value is false.

### setMergeAreas(boolean) {#setMergeAreas-boolean-}

<b>@deprecated.</b> Please use the 'mergeAreas' property instead. Indicates whether merge the areas of conditional formatting and validation before saving the file.

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

<b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
getCreateDirectory() : boolean;
```


**Remarks**

The default value is false.

### setCreateDirectory(boolean) {#setCreateDirectory-boolean-}

<b>@deprecated.</b> Please use the 'createDirectory' property instead. If true and the directory does not exist, the directory will be automatically created before saving the file.

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

<b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file.

```javascript
getSortNames() : boolean;
```


### setSortNames(boolean) {#setSortNames-boolean-}

<b>@deprecated.</b> Please use the 'sortNames' property instead. Indicates whether sorting defined names before saving file.

```javascript
setSortNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSortExternalNames() {#getSortExternalNames--}

<b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file.

```javascript
getSortExternalNames() : boolean;
```


### setSortExternalNames(boolean) {#setSortExternalNames-boolean-}

<b>@deprecated.</b> Please use the 'sortExternalNames' property instead. Indicates whether sorting external defined names before saving file.

```javascript
setSortExternalNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshChartCache() {#getRefreshChartCache--}

<b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data

```javascript
getRefreshChartCache() : boolean;
```


### setRefreshChartCache(boolean) {#setRefreshChartCache-boolean-}

<b>@deprecated.</b> Please use the 'refreshChartCache' property instead. Indicates whether refreshing chart cache data

```javascript
setRefreshChartCache(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

<b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

<b>@deprecated.</b> Please use the 'warningCallback' property instead. Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](../iwarningcallback/)

### getCheckExcelRestriction() {#getCheckExcelRestriction--}

<b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
getCheckExcelRestriction() : boolean;
```


### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}

<b>@deprecated.</b> Please use the 'checkExcelRestriction' property instead. Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
setCheckExcelRestriction(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getUpdateSmartArt() {#getUpdateSmartArt--}

<b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false.

```javascript
getUpdateSmartArt() : boolean;
```


**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setUpdateSmartArt(boolean) {#setUpdateSmartArt-boolean-}

<b>@deprecated.</b> Please use the 'updateSmartArt' property instead. Indicates whether updating smart art setting. The default value is false.

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

<b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
getEncryptDocumentProperties() : boolean;
```


**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.

### setEncryptDocumentProperties(boolean) {#setEncryptDocumentProperties-boolean-}

<b>@deprecated.</b> Please use the 'encryptDocumentProperties' property instead. Indicates whether encrypt document properties when saving as .xls file. The default value is true.

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

<b>@deprecated.</b> Please use the 'defaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
getDefaultFont() : string;
```


### setDefaultFont(string) {#setDefaultFont-string-}

<b>@deprecated.</b> Please use the 'defaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set the DefaultFont such as MingLiu or MS Gothic to show these characters. If this property is not set, Aspose.Cells will use system default font to show these unicode characters.

```javascript
setDefaultFont(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCheckWorkbookDefaultFont() {#getCheckWorkbookDefaultFont--}

<b>@deprecated.</b> Please use the 'checkWorkbookDefaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

```javascript
getCheckWorkbookDefaultFont() : boolean;
```


**Remarks**

Default is true.

### setCheckWorkbookDefaultFont(boolean) {#setCheckWorkbookDefaultFont-boolean-}

<b>@deprecated.</b> Please use the 'checkWorkbookDefaultFont' property instead. When characters in the Excel are Unicode and not be set with correct font in cell style, They may appear as block in pdf,image. Set this to true to try to use workbook's default font to show these characters first.

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

<b>@deprecated.</b> Please use the 'checkFontCompatibility' property instead. Indicates whether to check font compatibility for every character in text.

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

<b>@deprecated.</b> Please use the 'checkFontCompatibility' property instead. Indicates whether to check font compatibility for every character in text.

```javascript
getCheckFontCompatibility() : boolean;
```


**Remarks**

The default value is true. Disable this property may give better performance. But when the default or specified font of text/character cannot be used to render it, unreadable characters(such as block) maybe occur in the generated pdf. For such situation user should keep this property as true so that alternative font can be searched and used to render the text instead;

### setIsFontSubstitutionCharGranularity(boolean) {#setIsFontSubstitutionCharGranularity-boolean-}

<b>@deprecated.</b> Please use the 'isFontSubstitutionCharGranularity' property instead. Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

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

<b>@deprecated.</b> Please use the 'isFontSubstitutionCharGranularity' property instead. Indicates whether to only substitute the font of character when the cell font is not compatibility for it.

```javascript
isFontSubstitutionCharGranularity() : boolean;
```


**Remarks**

Default is false. We will try default font of Workbook and PdfSaveOption/system for cell font first.

### getOnePagePerSheet() {#getOnePagePerSheet--}

<b>@deprecated.</b> Please use the 'onePagePerSheet' property instead. If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
getOnePagePerSheet() : boolean;
```


### setOnePagePerSheet(boolean) {#setOnePagePerSheet-boolean-}

<b>@deprecated.</b> Please use the 'onePagePerSheet' property instead. If OnePagePerSheet is true , all content of one sheet will output to only one page in result. The paper size of pagesetup will be invalid, and the other settings of pagesetup will still take effect.

```javascript
setOnePagePerSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllColumnsInOnePagePerSheet() {#getAllColumnsInOnePagePerSheet--}

<b>@deprecated.</b> Please use the 'allColumnsInOnePagePerSheet' property instead. If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

```javascript
getAllColumnsInOnePagePerSheet() : boolean;
```


### setAllColumnsInOnePagePerSheet(boolean) {#setAllColumnsInOnePagePerSheet-boolean-}

<b>@deprecated.</b> Please use the 'allColumnsInOnePagePerSheet' property instead. If AllColumnsInOnePagePerSheet is true , all column content of one sheet will output to only one page in result. The width of paper size of pagesetup will be ignored, and the other settings of pagesetup will still take effect.

```javascript
setAllColumnsInOnePagePerSheet(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIgnoreError() {#getIgnoreError--}

<b>@deprecated.</b> Please use the 'ignoreError' property instead. Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

```javascript
getIgnoreError() : boolean;
```


### setIgnoreError(boolean) {#setIgnoreError-boolean-}

<b>@deprecated.</b> Please use the 'ignoreError' property instead. Indicates if you need to hide the error while rendering. The error can be error in shape, image, chart rendering, etc.

```javascript
setIgnoreError(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOutputBlankPageWhenNothingToPrint() {#getOutputBlankPageWhenNothingToPrint--}

<b>@deprecated.</b> Please use the 'outputBlankPageWhenNothingToPrint' property instead. Indicates whether to output a blank page when there is nothing to print.

```javascript
getOutputBlankPageWhenNothingToPrint() : boolean;
```


**Remarks**

Default is true.

### setOutputBlankPageWhenNothingToPrint(boolean) {#setOutputBlankPageWhenNothingToPrint-boolean-}

<b>@deprecated.</b> Please use the 'outputBlankPageWhenNothingToPrint' property instead. Indicates whether to output a blank page when there is nothing to print.

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

<b>@deprecated.</b> Please use the 'pageIndex' property instead. Gets or sets the 0-based index of the first page to save.

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

<b>@deprecated.</b> Please use the 'pageIndex' property instead. Gets or sets the 0-based index of the first page to save.

```javascript
getPageIndex() : number;
```


**Remarks**

Default is 0.

### setPageCount(number) {#setPageCount-number-}

<b>@deprecated.</b> Please use the 'pageCount' property instead. Gets or sets the number of pages to save.

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

<b>@deprecated.</b> Please use the 'pageCount' property instead. Gets or sets the number of pages to save.

```javascript
getPageCount() : number;
```


**Remarks**

Default is System.Int32.MaxValue which means all pages will be rendered..

### getPrintingPageType() {#getPrintingPageType--}

<b>@deprecated.</b> Please use the 'printingPageType' property instead. Indicates which pages will not be printed.

```javascript
getPrintingPageType() : PrintingPageType;
```


**Returns**

[PrintingPageType](../printingpagetype/)

**Remarks**

If content in the sheet is sparse, there will be some pages are totally blank in the output pdf file. If you don't want these blank pages, you can use this option to omit them.

### setPrintingPageType(PrintingPageType) {#setPrintingPageType-printingpagetype-}

<b>@deprecated.</b> Please use the 'printingPageType' property instead. Indicates which pages will not be printed.

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

<b>@deprecated.</b> Please use the 'gridlineType' property instead. Gets or sets gridline type.

```javascript
getGridlineType() : GridlineType;
```


**Returns**

[GridlineType](../gridlinetype/)

**Remarks**

Default is Dotted type.

### setGridlineType(GridlineType) {#setGridlineType-gridlinetype-}

<b>@deprecated.</b> Please use the 'gridlineType' property instead. Gets or sets gridline type.

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

<b>@deprecated.</b> Please use the 'gridlineColor' property instead. Gets or sets gridline color.

```javascript
getGridlineColor() : Color;
```


**Returns**

[Color](../color/)

**Remarks**

It will ignore the gridline color settings in the source file.

### setGridlineColor(Color) {#setGridlineColor-color-}

<b>@deprecated.</b> Please use the 'gridlineColor' property instead. Gets or sets gridline color.

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

<b>@deprecated.</b> Please use the 'textCrossType' property instead. Gets or sets displaying text type when the text width is larger than cell width.

```javascript
getTextCrossType() : TextCrossType;
```


**Returns**

[TextCrossType](../textcrosstype/)

### setTextCrossType(TextCrossType) {#setTextCrossType-textcrosstype-}

<b>@deprecated.</b> Please use the 'textCrossType' property instead. Gets or sets displaying text type when the text width is larger than cell width.

```javascript
setTextCrossType(value: TextCrossType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextCrossType](../textcrosstype/) | The value to set. |

### getDefaultEditLanguage() {#getDefaultEditLanguage--}

<b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language.

```javascript
getDefaultEditLanguage() : DefaultEditLanguage;
```


**Returns**

[DefaultEditLanguage](../defaulteditlanguage/)

**Remarks**

It may display/render different layouts for text paragraph when different edit languages is set. Default is [Aspose.Cells.DefaultEditLanguage.Auto](../aspose.cells.defaulteditlanguage.auto/).

### setDefaultEditLanguage(DefaultEditLanguage) {#setDefaultEditLanguage-defaulteditlanguage-}

<b>@deprecated.</b> Please use the 'defaultEditLanguage' property instead. Gets or sets default edit language.

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

<b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
getSheetSet() : SheetSet;
```


**Returns**

[SheetSet](../sheetset/)

### setSheetSet(SheetSet) {#setSheetSet-sheetset-}

<b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Visible](../aspose.cells.rendering.sheetset.visible/).

```javascript
setSheetSet(value: SheetSet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../sheetset/) | The value to set. |

### getDrawObjectEventHandler() {#getDrawObjectEventHandler--}

<b>@deprecated.</b> Please use the 'drawObjectEventHandler' property instead. Implements this interface to get DrawObject and Bound when rendering.

```javascript
getDrawObjectEventHandler() : DrawObjectEventHandler;
```


**Returns**

[DrawObjectEventHandler](../drawobjecteventhandler/)

### setDrawObjectEventHandler(DrawObjectEventHandler) {#setDrawObjectEventHandler-drawobjecteventhandler-}

<b>@deprecated.</b> Please use the 'drawObjectEventHandler' property instead. Implements this interface to get DrawObject and Bound when rendering.

```javascript
setDrawObjectEventHandler(value: DrawObjectEventHandler) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [DrawObjectEventHandler](../drawobjecteventhandler/) | The value to set. |

### getPageSavingCallback() {#getPageSavingCallback--}

<b>@deprecated.</b> Please use the 'pageSavingCallback' property instead. Control/Indicate progress of page saving process.

```javascript
getPageSavingCallback() : IPageSavingCallback;
```


**Returns**

[IPageSavingCallback](../ipagesavingcallback/)

### setPageSavingCallback(IPageSavingCallback) {#setPageSavingCallback-ipagesavingcallback-}

<b>@deprecated.</b> Please use the 'pageSavingCallback' property instead. Control/Indicate progress of page saving process.

```javascript
setPageSavingCallback(value: IPageSavingCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IPageSavingCallback](../ipagesavingcallback/) | The value to set. |

### getEmfRenderSetting() {#getEmfRenderSetting--}

<b>@deprecated.</b> Please use the 'emfRenderSetting' property instead. Setting for rendering Emf metafile.

```javascript
getEmfRenderSetting() : EmfRenderSetting;
```


**Returns**

[EmfRenderSetting](../emfrendersetting/)

**Remarks**

EMF metafiles identified as "EMF+ Dual" can contain both EMF+ records and EMF records. Either type of record can be used to render the image, only EMF+ records, or only EMF records. When [Aspose.Cells.EmfRenderSetting.EmfPlusPrefer](../aspose.cells.emfrendersetting.emfplusprefer/) is set, then EMF+ records will be parsed while rendering to page, otherwise only EMF records will be parsed. Default value is [Aspose.Cells.EmfRenderSetting.EmfOnly](../aspose.cells.emfrendersetting.emfonly/).

### setEmfRenderSetting(EmfRenderSetting) {#setEmfRenderSetting-emfrendersetting-}

<b>@deprecated.</b> Please use the 'emfRenderSetting' property instead. Setting for rendering Emf metafile.

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

<b>@deprecated.</b> Please use the 'customRenderSettings' property instead. Gets or sets custom settings during rendering.

```javascript
getCustomRenderSettings() : CustomRenderSettings;
```


**Returns**

[CustomRenderSettings](../customrendersettings/)

### setCustomRenderSettings(CustomRenderSettings) {#setCustomRenderSettings-customrendersettings-}

<b>@deprecated.</b> Please use the 'customRenderSettings' property instead. Gets or sets custom settings during rendering.

```javascript
setCustomRenderSettings(value: CustomRenderSettings) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomRenderSettings](../customrendersettings/) | The value to set. |


