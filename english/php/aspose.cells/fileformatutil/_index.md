---
title: "FileFormatUtil Class"
linktitle: "FileFormatUtil"
articleTitle: "FileFormatUtil"
second_title: "Aspose.Cells for PHP via Java"
description: "Provides utility methods for converting file format enums to strings or file extensions and back."
type: docs
weight: 2260
url: /php/aspose.cells/fileformatutil/
---

## FileFormatUtil class

Provides utility methods for converting file format enums to strings or file extensions and back.

## Methods

| Name | Description |
| --- | --- |
| [detectFileFormat](#detectfileformat) | Detects and returns the information about a format of an excel stored in a stream. |
| [verifyPassword](#verifypassword) | Detects and returns the information about a format of an excel stored in a stream. |
| [fileFormatToSaveFormat](#fileformattosaveformat) | Converting file format to save format. |
| [extensionToSaveFormat](#extensiontosaveformat) | Converts a file name extension into a SaveFormat value.

If the extension cannot be recognized, returns SaveFormat.UNKNO |
| [isTemplateFormat](#istemplateformat) | Returns true if the extension is .xlt, .xltX, .xltm,.ots. |
| [loadFormatToExtension](#loadformattoextension) | Converts a load format enumerated value into a file extension.

If it can not be converted, returns null. |
| [loadFormatToSaveFormat](#loadformattosaveformat) | Converts a LoadFormat value to a SaveFormat value if possible. |
| [saveFormatToExtension](#saveformattoextension) | Converts a save format enumerated value into a file extension. |
| [saveFormatToLoadFormat](#saveformattoloadformat) | Converts a SaveFormat value to a LoadFormat value if possible. |

### detectFileFormat(stream) (1 of 4) {#detectfileformat}

Detects and returns the information about a format of an excel stored in a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | InputStream | The stream |

**Returns:** A FileFormatInfo object that contains the detected information.

---

### detectFileFormat(stream, password) (2 of 4) {#detectfileformat-1}

Detects and returns the information about a format of an excel stored in a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | InputStream |  |
| password | String | The password for encrypted ooxml files. |

**Returns:** A FileFormatInfo object that contains the detected information.

---

### detectFileFormat(filePath) (3 of 4) {#detectfileformat-2}

Detects and returns the information about a format of an excel stored in a file.

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |

**Returns:** A FileFormatInfo object that contains the detected information.

---

### detectFileFormat(filePath, password) (4 of 4) {#detectfileformat-3}

Detects and returns the information about a format of an excel stored in a file.

| Parameter | Type | Description |
| --- | --- | --- |
| filePath | String | The file path. |
| password | String | The password for encrypted ooxml files. |

**Returns:** A FileFormatInfo object that contains the detected information.

### verifyPassword(stream, password) {#verifypassword}

Detects and returns the information about a format of an excel stored in a stream.

| Parameter | Type | Description |
| --- | --- | --- |
| stream | InputStream |  |
| password | String | The password for encrypted ooxml files. |

**Returns:** Returns whether the password is corrected.

### fileFormatToSaveFormat(format) {#fileformattosaveformat}

Converting file format to save format.

| Parameter | Type | Description |
| --- | --- | --- |
| format | Number | A FileFormatType value. The file format type. |

**Returns:** A SaveFormat value.

### extensionToSaveFormat(extension) {#extensiontosaveformat}

Converts a file name extension into a SaveFormat value.

If the extension cannot be recognized, returns SaveFormat.UNKNOWN .

| Parameter | Type | Description |
| --- | --- | --- |
| extension | String | The file extension. Can be with or without a leading dot. Case-insensitive. |

**Returns:** A SaveFormat value.

### isTemplateFormat(extension) {#istemplateformat}

Returns true if the extension is .xlt, .xltX, .xltm,.ots.

| Parameter | Type | Description |
| --- | --- | --- |
| extension | String |  |

### loadFormatToExtension(loadFormat) {#loadformattoextension}

Converts a load format enumerated value into a file extension.

If it can not be converted, returns null.

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | Number | A LoadFormat value. The loaded file format. |

**Returns:** The returned extension is a lower-case string with a leading dot.

### loadFormatToSaveFormat(loadFormat) {#loadformattosaveformat}

Converts a LoadFormat value to a SaveFormat value if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| loadFormat | Number | A LoadFormat value. The load format. |

**Returns:** A SaveFormat value. The save format.

### saveFormatToExtension(format) {#saveformattoextension}

Converts a save format enumerated value into a file extension.

| Parameter | Type | Description |
| --- | --- | --- |
| format | Number | A SaveFormat value. The save format. |

**Returns:** The returned extension is a lower-case string with a leading dot.

### saveFormatToLoadFormat(saveFormat) {#saveformattoloadformat}

Converts a SaveFormat value to a LoadFormat value if possible.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | A SaveFormat value. The save format. |

**Returns:** A LoadFormat value. The load format
