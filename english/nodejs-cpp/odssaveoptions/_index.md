---
title: OdsSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of saving ods file.
type: docs
url: /nodejs-cpp/odssaveoptions/
---

## OdsSaveOptions class

Represents the options of saving ods file.

```javascript
class OdsSaveOptions extends SaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the options of saving ods file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |
| [constructor(SaveFormat)](#constructor-saveformat-)| Creates the options of saving ods file. |

## Methods

| Method | Description |
| --- | --- |
| [getGeneratorType()](#getGeneratorType--)| Gets and sets the generator of the ods file. |
| [setGeneratorType(OdsGeneratorType)](#setGeneratorType-odsgeneratortype-)| Gets and sets the generator of the ods file. |
| [isStrictSchema11()](#isStrictSchema11--)| Indicates whether the ods file should be saved as ODF format version 1.1. Default is false. |
| [setIsStrictSchema11(boolean)](#setIsStrictSchema11-boolean-)| Indicates whether the ods file should be saved as ODF format version 1.1. Default is false. |
| [getOdfStrictVersion()](#getOdfStrictVersion--)| Gets and sets the ODF version. |
| [setOdfStrictVersion(OpenDocumentFormatVersionType)](#setOdfStrictVersion-opendocumentformatversiontype-)| Gets and sets the ODF version. |
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

Creates the options of saving ods file.

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

Creates the options of saving ods file.

```javascript
constructor(saveFormat: SaveFormat);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](/nodejs-cpp/saveformat/) | The file format.         /// It should be [SaveFormat.Ods](/nodejs-cpp/saveformat.ods/), [SaveFormat.Ods](/nodejs-cpp/saveformat.ods/),         /// [SaveFormat.Ods](/nodejs-cpp/saveformat.ods/) or [SaveFormat.Ods](/nodejs-cpp/saveformat.ods/),         /// otherwise the saved format will be set as [SaveFormat.Ods](/nodejs-cpp/saveformat.ods/) automatically. |

### getGeneratorType() {#getGeneratorType--}

Gets and sets the generator of the ods file.

```javascript
getGeneratorType() : OdsGeneratorType;
```


**Returns**

[OdsGeneratorType](/nodejs-cpp/odsgeneratortype/)

### setGeneratorType(OdsGeneratorType) {#setGeneratorType-odsgeneratortype-}

Gets and sets the generator of the ods file.

```javascript
setGeneratorType(value: OdsGeneratorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OdsGeneratorType](/nodejs-cpp/odsgeneratortype/) | The value to set. |

### isStrictSchema11() {#isStrictSchema11--}

Indicates whether the ods file should be saved as ODF format version 1.1. Default is false.

```javascript
isStrictSchema11() : boolean;
```


**Remarks**

NOTE: This member is now obsolete. Instead, please use OdsSaveOptions.OdfStrictVersion property. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.

### setIsStrictSchema11(boolean) {#setIsStrictSchema11-boolean-}

Indicates whether the ods file should be saved as ODF format version 1.1. Default is false.

```javascript
setIsStrictSchema11(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

NOTE: This member is now obsolete. Instead, please use OdsSaveOptions.OdfStrictVersion property. This method will be removed 12 months later since February 2024. Aspose apologizes for any inconvenience you may have experienced.

### getOdfStrictVersion() {#getOdfStrictVersion--}

Gets and sets the ODF version.

```javascript
getOdfStrictVersion() : OpenDocumentFormatVersionType;
```


**Returns**

[OpenDocumentFormatVersionType](/nodejs-cpp/opendocumentformatversiontype/)

### setOdfStrictVersion(OpenDocumentFormatVersionType) {#setOdfStrictVersion-opendocumentformatversiontype-}

Gets and sets the ODF version.

```javascript
setOdfStrictVersion(value: OpenDocumentFormatVersionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OpenDocumentFormatVersionType](/nodejs-cpp/opendocumentformatversiontype/) | The value to set. |

### getSaveFormat() {#getSaveFormat--}

Gets the save file format.

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](/nodejs-cpp/saveformat/)

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
| value | [IWarningCallback](/nodejs-cpp/iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](/nodejs-cpp/iwarningcallback/)

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


