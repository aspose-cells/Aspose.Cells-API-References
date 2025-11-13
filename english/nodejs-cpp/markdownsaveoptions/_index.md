---
title: MarkdownSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the save options for markdown.
type: docs
url: /nodejs-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Represents the save options for markdown.

```javascript
class MarkdownSaveOptions extends SaveOptions;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving markdown document |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [encoding](#encoding--)| EncodingType | Gets and sets the default encoding. |
| [formatStrategy](#formatStrategy--)| CellValueFormatStrategy | Gets and sets the format strategy when exporting the cell value as string. |
| [lightCellsDataProvider](#lightCellsDataProvider--)| LightCellsDataProvider | The Data provider to provide cells data for saving workbook in light mode. |
| [lineSeparator](#lineSeparator--)| string | Gets and sets the line separator. |
| [tableHeaderType](#tableHeaderType--)| MarkdownTableHeaderType | Gets and sets how set the header of the table. |
| [sheetSet](#sheetSet--)| SheetSet | Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Active](../aspose.cells.rendering.sheetset.active/). |
| [imageOptions](#imageOptions--)| ImageOrPrintOptions | Readonly. Get the ImageOrPrintOptions object before exporting |
| [exportImagesAsBase64](#exportImagesAsBase64--)| boolean | Specifies whether images are saved in Base64 format to Markdown. The default value is true. |
| [calculateFormula](#calculateFormula--)| boolean | Indicates whether to calculate formulas before saving markdown file. |
| [exportHyperlinkAsReference](#exportHyperlinkAsReference--)| boolean | Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false. |
| [alignColumnPadding](#alignColumnPadding--)| string | Indicates whether column alignment is enabled for generated Markdown tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default). |
| [splitTablesByBlankRow](#splitTablesByBlankRow--)| boolean | Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown. The default value is false. |
| [officeMathOutputType](#officeMathOutputType--)| HtmlOfficeMathOutputType | Indicates how export OfficeMath objects to Markdown, Default value is Image. |
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

## Methods

| Method | Description |
| --- | --- |
| [getEncoding()](#getEncoding--)| <b>@deprecated.</b> Please use the 'encoding' property instead. Gets and sets the default encoding. |
| [setEncoding(EncodingType)](#setEncoding-encodingtype-)| <b>@deprecated.</b> Please use the 'encoding' property instead. Gets and sets the default encoding. |
| [getFormatStrategy()](#getFormatStrategy--)| <b>@deprecated.</b> Please use the 'formatStrategy' property instead. Gets and sets the format strategy when exporting the cell value as string. |
| [setFormatStrategy(CellValueFormatStrategy)](#setFormatStrategy-cellvalueformatstrategy-)| <b>@deprecated.</b> Please use the 'formatStrategy' property instead. Gets and sets the format strategy when exporting the cell value as string. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--)| <b>@deprecated.</b> Please use the 'lightCellsDataProvider' property instead. The Data provider to provide cells data for saving workbook in light mode. |
| [setLightCellsDataProvider(LightCellsDataProvider)](#setLightCellsDataProvider-lightcellsdataprovider-)| <b>@deprecated.</b> Please use the 'lightCellsDataProvider' property instead. The Data provider to provide cells data for saving workbook in light mode. |
| [getLineSeparator()](#getLineSeparator--)| <b>@deprecated.</b> Please use the 'lineSeparator' property instead. Gets and sets the line separator. |
| [setLineSeparator(string)](#setLineSeparator-string-)| <b>@deprecated.</b> Please use the 'lineSeparator' property instead. Gets and sets the line separator. |
| [getTableHeaderType()](#getTableHeaderType--)| <b>@deprecated.</b> Please use the 'tableHeaderType' property instead. Gets and sets how set the header of the table. |
| [setTableHeaderType(MarkdownTableHeaderType)](#setTableHeaderType-markdowntableheadertype-)| <b>@deprecated.</b> Please use the 'tableHeaderType' property instead. Gets and sets how set the header of the table. |
| [getSheetSet()](#getSheetSet--)| <b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Active](../aspose.cells.rendering.sheetset.active/). |
| [setSheetSet(SheetSet)](#setSheetSet-sheetset-)| <b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Active](../aspose.cells.rendering.sheetset.active/). |
| [getImageOptions()](#getImageOptions--)| <b>@deprecated.</b> Please use the 'imageOptions' property instead. Get the ImageOrPrintOptions object before exporting |
| [getExportImagesAsBase64()](#getExportImagesAsBase64--)| <b>@deprecated.</b> Please use the 'exportImagesAsBase64' property instead. Specifies whether images are saved in Base64 format to Markdown. The default value is true. |
| [setExportImagesAsBase64(boolean)](#setExportImagesAsBase64-boolean-)| <b>@deprecated.</b> Please use the 'exportImagesAsBase64' property instead. Specifies whether images are saved in Base64 format to Markdown. The default value is true. |
| [getCalculateFormula()](#getCalculateFormula--)| <b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving markdown file. |
| [setCalculateFormula(boolean)](#setCalculateFormula-boolean-)| <b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving markdown file. |
| [getExportHyperlinkAsReference()](#getExportHyperlinkAsReference--)| <b>@deprecated.</b> Please use the 'exportHyperlinkAsReference' property instead. Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false. |
| [setExportHyperlinkAsReference(boolean)](#setExportHyperlinkAsReference-boolean-)| <b>@deprecated.</b> Please use the 'exportHyperlinkAsReference' property instead. Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false. |
| [getAlignColumnPadding()](#getAlignColumnPadding--)| <b>@deprecated.</b> Please use the 'alignColumnPadding' property instead. Indicates whether column alignment is enabled for generated Markdown tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default). |
| [setAlignColumnPadding(string)](#setAlignColumnPadding-string-)| <b>@deprecated.</b> Please use the 'alignColumnPadding' property instead. Indicates whether column alignment is enabled for generated Markdown tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default). |
| [getSplitTablesByBlankRow()](#getSplitTablesByBlankRow--)| <b>@deprecated.</b> Please use the 'splitTablesByBlankRow' property instead. Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown. The default value is false. |
| [setSplitTablesByBlankRow(boolean)](#setSplitTablesByBlankRow-boolean-)| <b>@deprecated.</b> Please use the 'splitTablesByBlankRow' property instead. Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown. The default value is false. |
| [getOfficeMathOutputType()](#getOfficeMathOutputType--)| <b>@deprecated.</b> Please use the 'officeMathOutputType' property instead. Indicates how export OfficeMath objects to Markdown, Default value is Image. |
| [setOfficeMathOutputType(HtmlOfficeMathOutputType)](#setOfficeMathOutputType-htmlofficemathoutputtype-)| <b>@deprecated.</b> Please use the 'officeMathOutputType' property instead. Indicates how export OfficeMath objects to Markdown, Default value is Image. |
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


### constructor() {#constructor--}

Creates options for saving markdown document

```javascript
constructor();
```


### constructor(SaveOptions) {#constructor-saveoptions-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: SaveOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | SaveOptions | The parent object. |

### encoding {#encoding--}

Gets and sets the default encoding.

```javascript
encoding : EncodingType;
```


### formatStrategy {#formatStrategy--}

Gets and sets the format strategy when exporting the cell value as string.

```javascript
formatStrategy : CellValueFormatStrategy;
```


### lightCellsDataProvider {#lightCellsDataProvider--}

The Data provider to provide cells data for saving workbook in light mode.

```javascript
lightCellsDataProvider : LightCellsDataProvider;
```


### lineSeparator {#lineSeparator--}

Gets and sets the line separator.

```javascript
lineSeparator : string;
```


### tableHeaderType {#tableHeaderType--}

Gets and sets how set the header of the table.

```javascript
tableHeaderType : MarkdownTableHeaderType;
```


### sheetSet {#sheetSet--}

Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Active](../aspose.cells.rendering.sheetset.active/).

```javascript
sheetSet : SheetSet;
```


**Remarks**

The set is ignored when it is used in [SheetRender](../sheetrender/)

### imageOptions {#imageOptions--}

Readonly. Get the ImageOrPrintOptions object before exporting

```javascript
imageOptions : ImageOrPrintOptions;
```


### exportImagesAsBase64 {#exportImagesAsBase64--}

Specifies whether images are saved in Base64 format to Markdown. The default value is true.

```javascript
exportImagesAsBase64 : boolean;
```


**Remarks**

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### calculateFormula {#calculateFormula--}

Indicates whether to calculate formulas before saving markdown file.

```javascript
calculateFormula : boolean;
```


**Remarks**

The default value is false.

### exportHyperlinkAsReference {#exportHyperlinkAsReference--}

Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false.

```javascript
exportHyperlinkAsReference : boolean;
```


### alignColumnPadding {#alignColumnPadding--}

Indicates whether column alignment is enabled for generated Markdown tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default).

```javascript
alignColumnPadding : string;
```


### splitTablesByBlankRow {#splitTablesByBlankRow--}

Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown. The default value is false.

```javascript
splitTablesByBlankRow : boolean;
```


### officeMathOutputType {#officeMathOutputType--}

Indicates how export OfficeMath objects to Markdown, Default value is Image.

```javascript
officeMathOutputType : HtmlOfficeMathOutputType;
```


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

### getEncoding() {#getEncoding--}

<b>@deprecated.</b> Please use the 'encoding' property instead. Gets and sets the default encoding.

```javascript
getEncoding() : EncodingType;
```


**Returns**

[EncodingType](../encodingtype/)

### setEncoding(EncodingType) {#setEncoding-encodingtype-}

<b>@deprecated.</b> Please use the 'encoding' property instead. Gets and sets the default encoding.

```javascript
setEncoding(value: EncodingType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [EncodingType](../encodingtype/) | The value to set. |

### getFormatStrategy() {#getFormatStrategy--}

<b>@deprecated.</b> Please use the 'formatStrategy' property instead. Gets and sets the format strategy when exporting the cell value as string.

```javascript
getFormatStrategy() : CellValueFormatStrategy;
```


**Returns**

[CellValueFormatStrategy](../cellvalueformatstrategy/)

### setFormatStrategy(CellValueFormatStrategy) {#setFormatStrategy-cellvalueformatstrategy-}

<b>@deprecated.</b> Please use the 'formatStrategy' property instead. Gets and sets the format strategy when exporting the cell value as string.

```javascript
setFormatStrategy(value: CellValueFormatStrategy) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellValueFormatStrategy](../cellvalueformatstrategy/) | The value to set. |

### getLightCellsDataProvider() {#getLightCellsDataProvider--}

<b>@deprecated.</b> Please use the 'lightCellsDataProvider' property instead. The Data provider to provide cells data for saving workbook in light mode.

```javascript
getLightCellsDataProvider() : LightCellsDataProvider;
```


**Returns**

[LightCellsDataProvider](../lightcellsdataprovider/)

### setLightCellsDataProvider(LightCellsDataProvider) {#setLightCellsDataProvider-lightcellsdataprovider-}

<b>@deprecated.</b> Please use the 'lightCellsDataProvider' property instead. The Data provider to provide cells data for saving workbook in light mode.

```javascript
setLightCellsDataProvider(value: LightCellsDataProvider) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../lightcellsdataprovider/) | The value to set. |

### getLineSeparator() {#getLineSeparator--}

<b>@deprecated.</b> Please use the 'lineSeparator' property instead. Gets and sets the line separator.

```javascript
getLineSeparator() : string;
```


### setLineSeparator(string) {#setLineSeparator-string-}

<b>@deprecated.</b> Please use the 'lineSeparator' property instead. Gets and sets the line separator.

```javascript
setLineSeparator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTableHeaderType() {#getTableHeaderType--}

<b>@deprecated.</b> Please use the 'tableHeaderType' property instead. Gets and sets how set the header of the table.

```javascript
getTableHeaderType() : MarkdownTableHeaderType;
```


**Returns**

[MarkdownTableHeaderType](../markdowntableheadertype/)

### setTableHeaderType(MarkdownTableHeaderType) {#setTableHeaderType-markdowntableheadertype-}

<b>@deprecated.</b> Please use the 'tableHeaderType' property instead. Gets and sets how set the header of the table.

```javascript
setTableHeaderType(value: MarkdownTableHeaderType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MarkdownTableHeaderType](../markdowntableheadertype/) | The value to set. |

### getSheetSet() {#getSheetSet--}

<b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Active](../aspose.cells.rendering.sheetset.active/).

```javascript
getSheetSet() : SheetSet;
```


**Returns**

[SheetSet](../sheetset/)

**Remarks**

The set is ignored when it is used in [SheetRender](../sheetrender/)

### setSheetSet(SheetSet) {#setSheetSet-sheetset-}

<b>@deprecated.</b> Please use the 'sheetSet' property instead. Gets or sets the sheets to render. Default is all visible sheets in the workbook: [Aspose.Cells.Rendering.SheetSet.Active](../aspose.cells.rendering.sheetset.active/).

```javascript
setSheetSet(value: SheetSet) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SheetSet](../sheetset/) | The value to set. |

**Remarks**

The set is ignored when it is used in [SheetRender](../sheetrender/)

### getImageOptions() {#getImageOptions--}

<b>@deprecated.</b> Please use the 'imageOptions' property instead. Get the ImageOrPrintOptions object before exporting

```javascript
getImageOptions() : ImageOrPrintOptions;
```


**Returns**

[ImageOrPrintOptions](../imageorprintoptions/)

### getExportImagesAsBase64() {#getExportImagesAsBase64--}

<b>@deprecated.</b> Please use the 'exportImagesAsBase64' property instead. Specifies whether images are saved in Base64 format to Markdown. The default value is true.

```javascript
getExportImagesAsBase64() : boolean;
```


**Remarks**

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### setExportImagesAsBase64(boolean) {#setExportImagesAsBase64-boolean-}

<b>@deprecated.</b> Please use the 'exportImagesAsBase64' property instead. Specifies whether images are saved in Base64 format to Markdown. The default value is true.

```javascript
setExportImagesAsBase64(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When this property is set to true image data is exported directly on the img elements and separate files are not created.

### getCalculateFormula() {#getCalculateFormula--}

<b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving markdown file.

```javascript
getCalculateFormula() : boolean;
```


**Remarks**

The default value is false.

### setCalculateFormula(boolean) {#setCalculateFormula-boolean-}

<b>@deprecated.</b> Please use the 'calculateFormula' property instead. Indicates whether to calculate formulas before saving markdown file.

```javascript
setCalculateFormula(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getExportHyperlinkAsReference() {#getExportHyperlinkAsReference--}

<b>@deprecated.</b> Please use the 'exportHyperlinkAsReference' property instead. Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false.

```javascript
getExportHyperlinkAsReference() : boolean;
```


### setExportHyperlinkAsReference(boolean) {#setExportHyperlinkAsReference-boolean-}

<b>@deprecated.</b> Please use the 'exportHyperlinkAsReference' property instead. Indicates whether to export hyperlink using reference definitions instead of inline format. The default value is false.

```javascript
setExportHyperlinkAsReference(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAlignColumnPadding() {#getAlignColumnPadding--}

<b>@deprecated.</b> Please use the 'alignColumnPadding' property instead. Indicates whether column alignment is enabled for generated Markdown tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default).

```javascript
getAlignColumnPadding() : string;
```


### setAlignColumnPadding(string) {#setAlignColumnPadding-string-}

<b>@deprecated.</b> Please use the 'alignColumnPadding' property instead. Indicates whether column alignment is enabled for generated Markdown tables. When enabled, columns are aligned by padding cell content with the specified character(typically ' ' for spaces). Set to '\0' to disable column alignment (default).

```javascript
setAlignColumnPadding(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSplitTablesByBlankRow() {#getSplitTablesByBlankRow--}

<b>@deprecated.</b> Please use the 'splitTablesByBlankRow' property instead. Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown. The default value is false.

```javascript
getSplitTablesByBlankRow() : boolean;
```


### setSplitTablesByBlankRow(boolean) {#setSplitTablesByBlankRow-boolean-}

<b>@deprecated.</b> Please use the 'splitTablesByBlankRow' property instead. Indicates whether blank rows in the worksheet should be treated as table separators when exporting to Markdown. The default value is false.

```javascript
setSplitTablesByBlankRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getOfficeMathOutputType() {#getOfficeMathOutputType--}

<b>@deprecated.</b> Please use the 'officeMathOutputType' property instead. Indicates how export OfficeMath objects to Markdown, Default value is Image.

```javascript
getOfficeMathOutputType() : HtmlOfficeMathOutputType;
```


**Returns**

[HtmlOfficeMathOutputType](../htmlofficemathoutputtype/)

### setOfficeMathOutputType(HtmlOfficeMathOutputType) {#setOfficeMathOutputType-htmlofficemathoutputtype-}

<b>@deprecated.</b> Please use the 'officeMathOutputType' property instead. Indicates how export OfficeMath objects to Markdown, Default value is Image.

```javascript
setOfficeMathOutputType(value: HtmlOfficeMathOutputType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [HtmlOfficeMathOutputType](../htmlofficemathoutputtype/) | The value to set. |

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


