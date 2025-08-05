﻿---
title: OoxmlSaveOptions
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the options of saving office open xml file.
type: docs
url: /js-cpp/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Represents the options of saving office open xml file.

```javascript
class OoxmlSaveOptions extends SaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options for saving office open xml file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(SaveFormat)](#constructor-saveformat-)| Creates the options for saving office open xml file. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [exportCellName](#exportCellName--)| boolean | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true. |
| [lightCellsDataProvider](#lightCellsDataProvider--)| LightCellsDataProvider | The data provider for saving workbook in light mode. |
| [updateZoom](#updateZoom--)| boolean | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. |
| [enableZip64](#enableZip64--)| boolean | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [embedOoxmlAsOleObject](#embedOoxmlAsOleObject--)| boolean | Indicates whether embedding Ooxml files of OleObject as ole object. |
| [compressionType](#compressionType--)| OoxmlCompressionType | Gets and sets the compression type for ooxml file. |
| [wpsCompatibility](#wpsCompatibility--)| boolean | Indicates whether to make the xls more compatible with WPS. |
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

Creates the options for saving office open xml file.

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

### constructor(SaveFormat) {#constructor-saveformat-}

Creates the options for saving office open xml file.

```javascript
constructor(saveFormat: SaveFormat);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](../saveformat/) | The file format.         /// It should be one of following types: [SaveFormat.Xlsx](../saveformat.xlsx/), [SaveFormat.Xltx](../saveformat.xltx/),         /// [SaveFormat.Xlam](../saveformat.xlam/), [SaveFormat.Xlsm](../saveformat.xlsm/) or [SaveFormat.Xltm](../saveformat.xltm/),         /// otherwise the saved format will be set as [SaveFormat.Xlsx](../saveformat.xlsx/) automatically. |

### exportCellName {#exportCellName--}

Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

```javascript
exportCellName : boolean;
```


### lightCellsDataProvider {#lightCellsDataProvider--}

The data provider for saving workbook in light mode.

```javascript
lightCellsDataProvider : LightCellsDataProvider;
```


### updateZoom {#updateZoom--}

Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled.

```javascript
updateZoom : boolean;
```


**Remarks**

The default value is false for performance.

### enableZip64 {#enableZip64--}

Always use ZIP64 extensions when writing zip archives, even when unnecessary.

```javascript
enableZip64 : boolean;
```


### embedOoxmlAsOleObject {#embedOoxmlAsOleObject--}

Indicates whether embedding Ooxml files of OleObject as ole object.

```javascript
embedOoxmlAsOleObject : boolean;
```


**Remarks**

Only for OleObject.

### compressionType {#compressionType--}

Gets and sets the compression type for ooxml file.

```javascript
compressionType : OoxmlCompressionType;
```


**Remarks**

The default value is OoxmlCompressionType.Level2.

### wpsCompatibility {#wpsCompatibility--}

Indicates whether to make the xls more compatible with WPS.

```javascript
wpsCompatibility : boolean;
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


