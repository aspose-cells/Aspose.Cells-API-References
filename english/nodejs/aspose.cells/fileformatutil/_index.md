---
title: "FileFormatUtil"
linktitle: "FileFormatUtil"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Provides utility methods for converting file format enums to strings or file extensions and back."
type: docs
weight: 1430
url: /nodejs/aspose.cells/fileformatutil/
---

## FileFormatUtil class

Provides utility methods for converting file format enums to strings or file extensions and back.

## Methods

| Name | Description |
| --- | --- |
| [detectFileFormat(stream)](#detectfileformat) *(static)* | Detects and returns the information about a format of an excel stored in a stream. |
| [detectFileFormat(stream, password)](#detectfileformat-1) *(static)* | Detects and returns the information about a format of an excel stored in a stream. |
| [detectFileFormat(filePath)](#detectfileformat-2) *(static)* | Detects and returns the information about a format of an excel stored in a file. |
| [detectFileFormat(filePath, password)](#detectfileformat-3) *(static)* | Detects and returns the information about a format of an excel stored in a file. |
| [detectFileFormatFromStream(stream, callback)](#detectfileformatfromstream) *(static)* | Detects and returns the information about a format of an excel stored in a stream. |
| [extensionToSaveFormat(extension)](#extensiontosaveformat) *(static)* | Converts a file name extension into a SaveFormat value. If the extension cannot be recognized, returns SaveFormat.UNKNOW |
| [fileFormatToSaveFormat(format)](#fileformattosaveformat) *(static)* | Converting file format to save format. |
| [isTemplateFormat(extension)](#istemplateformat) *(static)* | Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
| [loadFormatToExtension(loadFormat)](#loadformattoextension) *(static)* | Converts a load format enumerated value into a file extension. If it can not be converted, returns null. |
| [loadFormatToSaveFormat(loadFormat)](#loadformattosaveformat) *(static)* | Converts a LoadFormat value to a SaveFormat value if possible. |
| [saveFormatToExtension(format)](#saveformattoextension) *(static)* | Converts a save format enumerated value into a file extension. |
| [saveFormatToLoadFormat(saveFormat)](#saveformattoloadformat) *(static)* | Converts a SaveFormat value to a LoadFormat value if possible. |
| [verifyPassword(stream, password)](#verifypassword) *(static)* | Detects and returns the information about a format of an excel stored in a stream. |

### detectFileFormat(stream) (static) {#detectfileformat}

Detects and returns the information about a format of an excel stored in a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | InputStream | The stream |

**Returns:** FileFormatInfo — `FileFormatInfo` A FileFormatInfo object that contains the detected information.

### detectFileFormat(stream, password) (static) {#detectfileformat-1}

Detects and returns the information about a format of an excel stored in a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | InputStream |  |
| password | String | The password for encrypted ooxml files. |

**Returns:** FileFormatInfo — `FileFormatInfo` A FileFormatInfo object that contains the detected information.

### detectFileFormat(filePath) (static) {#detectfileformat-2}

Detects and returns the information about a format of an excel stored in a file.

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |

**Returns:** FileFormatInfo — `FileFormatInfo` A FileFormatInfo object that contains the detected information.

### detectFileFormat(filePath, password) (static) {#detectfileformat-3}

Detects and returns the information about a format of an excel stored in a file.

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
| password | String | The password for encrypted ooxml files. |

**Returns:** FileFormatInfo — `FileFormatInfo` A FileFormatInfo object that contains the detected information.

### detectFileFormatFromStream(stream, callback) (static) {#detectfileformatfromstream}

Detects and returns the information about a format of an excel stored in a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | ReadableStream | The stream |
| callback | Callback | The callback function |

**Returns:** FileFormatInfo — `FileFormatInfo` A FileFormatInfo object that contains the detected information.

**Example:**

```js
var aspose = aspose || {};
aspose.cells = require("aspose.cells");
var fs = require("fs");
var readStream = fs.createReadStream("Book2.xlsx");
aspose.cells.FileFormatUtil.detectFileFormatFromStream(readStream, function(result, err) {
if (!err) {
console.log("detect result: " + result.getFileFormatType());
}
});
```

### extensionToSaveFormat(extension) (static) {#extensiontosaveformat}

Converts a file name extension into a SaveFormat value. If the extension cannot be recognized, returns SaveFormat.UNKNOWN.

| Parameter | Type | Description |
| --- | --- | --- |
| extension | String | The file extension. Can be with or without a leading dot. Case-insensitive. |

**Returns:** Number — `Number` A SaveFormat value.

### fileFormatToSaveFormat(format) (static) {#fileformattosaveformat}

Converting file format to save format.

| Parameter | Type | Description |
| --- | --- | --- |
| format | Number | FileFormatType |

**Returns:** Number — `Number` A SaveFormat value.

### isTemplateFormat(extension) (static) {#istemplateformat}

Returns true if the extension is .xlt, .xltX, .xltm,.ots.

| Parameter | Type | Description |
| --- | --- | --- |
| extension | String |  |

**Returns:** boolean — `boolean`

### loadFormatToExtension(loadFormat) (static) {#loadformattoextension}

Converts a load format enumerated value into a file extension. If it can not be converted, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | Number | LoadFormat |

**Returns:** String — `String` The returned extension is a lower-case string with a leading dot.

### loadFormatToSaveFormat(loadFormat) (static) {#loadformattosaveformat}

Converts a LoadFormat value to a SaveFormat value if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | Number | LoadFormat |

**Returns:** Number — `Number` A SaveFormat value. The save format.

### saveFormatToExtension(format) (static) {#saveformattoextension}

Converts a save format enumerated value into a file extension.

| Parameter | Type | Description |
| --- | --- | --- |
| format | Number | SaveFormat |

**Returns:** String — `String` The returned extension is a lower-case string with a leading dot.

### saveFormatToLoadFormat(saveFormat) (static) {#saveformattoloadformat}

Converts a SaveFormat value to a LoadFormat value if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | SaveFormat |

**Returns:** Number — `Number` A LoadFormat value. The load format

### verifyPassword(stream, password) (static) {#verifypassword}

Detects and returns the information about a format of an excel stored in a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | InputStream |  |
| password | String | The password for encrypted ooxml files. |

**Returns:** boolean — `boolean` Returns whether the password is corrected.
