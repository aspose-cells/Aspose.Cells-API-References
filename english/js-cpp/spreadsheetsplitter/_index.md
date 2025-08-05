﻿---
title: SpreadsheetSplitter
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Splits spreadsheet file into multiple parts.
type: docs
url: /js-cpp/spreadsheetsplitter/
---

## SpreadsheetSplitter class

Splits spreadsheet file into multiple parts.

```javascript
class SpreadsheetSplitter;
```


## Methods

| Method | Description |
| --- | --- |
| static [process(string, string)](#process-string-string-)| Splits given template file into multiple parts. |


### process(string, string) {#process-string-string-}

Splits given template file into multiple parts.

```javascript
static process(templateFile: string, resultFile: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| templateFile | string | The template file to be split |
| resultFile | string | The resultant file(name pattern) |

**Remarks**

The output files will be build from the specified resultant file by appending sequence number of the sheet and split part. For example, if the specified output file is Split.xlsx, then the generated files will be Split_0_0.xlsx, Split_0_1.xlsx, ..., Split_1_0.xlsx, ...


