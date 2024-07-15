---
title: OoxmlSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of saving office open xml file.
type: docs
url: /nodejs-cpp/ooxmlsaveoptions/
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

## Methods

| Method | Description |
| --- | --- |
| [getExportCellName()](#getExportCellName--)| Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true. |
| [setExportCellName(boolean)](#setExportCellName-boolean-)| Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true. |
| [getLightCellsDataProvider()](#getLightCellsDataProvider--)| The data provider for saving workbook in light mode. |
| [setLightCellsDataProvider(LightCellsDataProvider)](#setLightCellsDataProvider-lightcellsdataprovider-)| The data provider for saving workbook in light mode. |
| [getUpdateZoom()](#getUpdateZoom--)| Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. |
| [setUpdateZoom(boolean)](#setUpdateZoom-boolean-)| Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. |
| [getEnableZip64()](#getEnableZip64--)| Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [setEnableZip64(boolean)](#setEnableZip64-boolean-)| Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [getEmbedOoxmlAsOleObject()](#getEmbedOoxmlAsOleObject--)| Indicates whether embedding Ooxml files of OleObject as ole object. |
| [setEmbedOoxmlAsOleObject(boolean)](#setEmbedOoxmlAsOleObject-boolean-)| Indicates whether embedding Ooxml files of OleObject as ole object. |
| [getCompressionType()](#getCompressionType--)| Gets and sets the compression type for ooxml file. |
| [setCompressionType(OoxmlCompressionType)](#setCompressionType-ooxmlcompressiontype-)| Gets and sets the compression type for ooxml file. |
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
| saveFormat | [SaveFormat](../saveformat/) | The file format.         /// It should be one of following types: [SaveFormat.Xlsx](../saveformat.xlsx/), [SaveFormat.Xlsx](../saveformat.xlsx/),         /// [SaveFormat.Xlsx](../saveformat.xlsx/), [SaveFormat.Xlsx](../saveformat.xlsx/) or [SaveFormat.Xlsx](../saveformat.xlsx/),         /// otherwise the saved format will be set as [SaveFormat.Xlsx](../saveformat.xlsx/) automatically. |

### getExportCellName() {#getExportCellName--}

Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

```javascript
getExportCellName() : boolean;
```


### setExportCellName(boolean) {#setExportCellName-boolean-}

Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

```javascript
setExportCellName(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getLightCellsDataProvider() {#getLightCellsDataProvider--}

The data provider for saving workbook in light mode.

```javascript
getLightCellsDataProvider() : LightCellsDataProvider;
```


**Returns**

[LightCellsDataProvider](../lightcellsdataprovider/)

### setLightCellsDataProvider(LightCellsDataProvider) {#setLightCellsDataProvider-lightcellsdataprovider-}

The data provider for saving workbook in light mode.

```javascript
setLightCellsDataProvider(value: LightCellsDataProvider) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LightCellsDataProvider](../lightcellsdataprovider/) | The value to set. |

### getUpdateZoom() {#getUpdateZoom--}

Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled.

```javascript
getUpdateZoom() : boolean;
```


**Remarks**

The default value is false for performance.

### setUpdateZoom(boolean) {#setUpdateZoom-boolean-}

Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled.

```javascript
setUpdateZoom(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false for performance.

### getEnableZip64() {#getEnableZip64--}

Always use ZIP64 extensions when writing zip archives, even when unnecessary.

```javascript
getEnableZip64() : boolean;
```


### setEnableZip64(boolean) {#setEnableZip64-boolean-}

Always use ZIP64 extensions when writing zip archives, even when unnecessary.

```javascript
setEnableZip64(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEmbedOoxmlAsOleObject() {#getEmbedOoxmlAsOleObject--}

Indicates whether embedding Ooxml files of OleObject as ole object.

```javascript
getEmbedOoxmlAsOleObject() : boolean;
```


**Remarks**

Only for OleObject.

### setEmbedOoxmlAsOleObject(boolean) {#setEmbedOoxmlAsOleObject-boolean-}

Indicates whether embedding Ooxml files of OleObject as ole object.

```javascript
setEmbedOoxmlAsOleObject(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for OleObject.

### getCompressionType() {#getCompressionType--}

Gets and sets the compression type for ooxml file.

```javascript
getCompressionType() : OoxmlCompressionType;
```


**Returns**

[OoxmlCompressionType](../ooxmlcompressiontype/)

**Remarks**

The default value is OoxmlCompressionType.Level2.

### setCompressionType(OoxmlCompressionType) {#setCompressionType-ooxmlcompressiontype-}

Gets and sets the compression type for ooxml file.

```javascript
setCompressionType(value: OoxmlCompressionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OoxmlCompressionType](../ooxmlcompressiontype/) | The value to set. |

**Remarks**

The default value is OoxmlCompressionType.Level2.

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


