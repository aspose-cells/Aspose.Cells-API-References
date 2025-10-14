---
title: MarkdownSaveOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the save options for markdown.
type: docs
url: /javascript-cpp/markdownsaveoptions/
---

## MarkdownSaveOptions class

Represents the save options for markdown.

```javascript
class MarkdownSaveOptions extends SaveOptions;
```


## Constructors

| Name | Description |
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


