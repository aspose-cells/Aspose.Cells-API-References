---
title: FileFormatUtil
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Provides utility methods for converting file format enums to strings or file extensions and back.
type: docs
url: /nodejs-cpp/fileformatutil/
---

## FileFormatUtil class

Provides utility methods for converting file format enums to strings or file extensions and back.

```javascript
class FileFormatUtil;
```


## Methods

| Method | Description |
| --- | --- |
| static [detectFileFormat(Uint8Array)](#detectFileFormat-uint8array-)| Detects and returns the information about a format of an excel stored in a stream. |
| static [verifyPassword(Uint8Array, string)](#verifyPassword-uint8array-string-)| Detects and returns the information about a format of an excel stored in a stream. |
| static [fileFormatToSaveFormat(FileFormatType)](#fileFormatToSaveFormat-fileformattype-)| Converting file format to save format. |
| static [extensionToSaveFormat(string)](#extensionToSaveFormat-string-)| Converts a file name extension into a SaveFormat value. |
| static [isTemplateFormat(string)](#isTemplateFormat-string-)| Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
| static [loadFormatToExtension(LoadFormat)](#loadFormatToExtension-loadformat-)| Converts a load format enumerated value into a file extension. |
| static [loadFormatToSaveFormat(LoadFormat)](#loadFormatToSaveFormat-loadformat-)| Converts a LoadFormat value to a SaveFormat value if possible. |
| static [saveFormatToExtension(SaveFormat)](#saveFormatToExtension-saveformat-)| Converts a save format enumerated value into a file extension. |
| static [saveFormatToLoadFormat(SaveFormat)](#saveFormatToLoadFormat-saveformat-)| Converts a SaveFormat value to a LoadFormat value if possible. |


### detectFileFormat(Uint8Array) {#detectFileFormat-uint8array-}

Detects and returns the information about a format of an excel stored in a stream.

```javascript
static detectFileFormat(stream: Uint8Array) : FileFormatInfo;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array |  |

**Returns**

A [FileFormatInfo](/nodejs-cpp/fileformatinfo/) object that contains the detected information.

### verifyPassword(Uint8Array, string) {#verifyPassword-uint8array-string-}

Detects and returns the information about a format of an excel stored in a stream.

```javascript
static verifyPassword(stream: Uint8Array, password: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array |  |
| password | string | The password for encrypted ooxml files. |

**Returns**

Returns whether the password is corrected.

### fileFormatToSaveFormat(FileFormatType) {#fileFormatToSaveFormat-fileformattype-}

Converting file format to save format.

```javascript
static fileFormatToSaveFormat(format: FileFormatType) : SaveFormat;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | [FileFormatType](/nodejs-cpp/fileformattype/) | The file format type. |

**Returns**

[SaveFormat](/nodejs-cpp/saveformat/)

### extensionToSaveFormat(string) {#extensionToSaveFormat-string-}

Converts a file name extension into a SaveFormat value.

```javascript
static extensionToSaveFormat(extension: string) : SaveFormat;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extension | string | The file extension. Can be with or without a leading dot. Case-insensitive. |

**Returns**

[SaveFormat](/nodejs-cpp/saveformat/)

**Remarks**

If the extension cannot be recognized, returns [SaveFormat.Unknown](/nodejs-cpp/saveformat.unknown/).

### isTemplateFormat(string) {#isTemplateFormat-string-}

Returns true if the extension is .xlt, .xltX, .xltm,.ots.

```javascript
static isTemplateFormat(extension: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| extension | string |  |

### loadFormatToExtension(LoadFormat) {#loadFormatToExtension-loadformat-}

Converts a load format enumerated value into a file extension.

```javascript
static loadFormatToExtension(loadFormat: LoadFormat) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | [LoadFormat](/nodejs-cpp/loadformat/) | The loaded file format. |

**Returns**

The returned extension is a lower-case string with a leading dot.

**Remarks**

If it can not be converted, returns null.

### loadFormatToSaveFormat(LoadFormat) {#loadFormatToSaveFormat-loadformat-}

Converts a LoadFormat value to a SaveFormat value if possible.

```javascript
static loadFormatToSaveFormat(loadFormat: LoadFormat) : SaveFormat;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | [LoadFormat](/nodejs-cpp/loadformat/) | The load format. |

**Returns**

The save format.

### saveFormatToExtension(SaveFormat) {#saveFormatToExtension-saveformat-}

Converts a save format enumerated value into a file extension.

```javascript
static saveFormatToExtension(format: SaveFormat) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| format | [SaveFormat](/nodejs-cpp/saveformat/) | The save format. |

**Returns**

The returned extension is a lower-case string with a leading dot.

### saveFormatToLoadFormat(SaveFormat) {#saveFormatToLoadFormat-saveformat-}

Converts a SaveFormat value to a LoadFormat value if possible.

```javascript
static saveFormatToLoadFormat(saveFormat: SaveFormat) : LoadFormat;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | [SaveFormat](/nodejs-cpp/saveformat/) | The save format. |

**Returns**

The load format


