---
title: SpreadsheetLocker
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Low code api to lock spreadsheet file.
type: docs
url: /javascript-cpp/spreadsheetlocker/
---

## SpreadsheetLocker class

Low code api to lock spreadsheet file.

```javascript
class SpreadsheetLocker;
```


## Methods

| Method | Description |
| --- | --- |
| static [process(string, string, string, string)](#process-string-string-string-string-)| Locks spreadsheet file with specified settings. |


### process(string, string, string, string) {#process-string-string-string-string-}

Locks spreadsheet file with specified settings.

```javascript
static process(templateFile: string, resultFile: string, openPassword: string, writePassword: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | string | The template file to be locked |
| resultFile | string | The resultant file |
| openPassword | string | Password for file encryption |
| writePassword | string | Password for protection of modifying spreadsheet |


