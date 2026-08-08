---
title: "JsonUtility"
linktitle: "JsonUtility"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the utility class of processing json."
type: docs
weight: 1970
url: /nodejs/aspose.cells/jsonutility/
---

## JsonUtility class

Represents the utility class of processing json.

```js
new JsonUtility()
```

## Methods

| Name | Description |
| --- | --- |
| [exportRangeToJson(range, options)](#exportrangetojson) *(static)* | Exporting the range to json file. NOTE: This member is now obsolete. Instead, please use ExportRangeToJson(Range range,  |
| [exportRangeToJson(range, options)](#exportrangetojson-1) *(static)* | Exporting the range to json file. |
| [importData(json, cells, row, column, option)](#importdata) *(static)* | Import the json string. |

### exportRangeToJson(range, options) (static) {#exportrangetojson}

Exporting the range to json file. NOTE: This member is now obsolete. Instead, please use ExportRangeToJson(Range range, JsonSaveOptions options) method. This property will be removed 6 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |
| options | ExportRangeToJsonOptions | The options of exporting. |

**Returns:** String — `String` The json string value.

### exportRangeToJson(range, options) (static) {#exportrangetojson-1}

Exporting the range to json file.

| Parameter | Type | Description |
| --- | --- | --- |
| range | Range | The range. |
| options | JsonSaveOptions | The options of exporting. |

**Returns:** String — `String` The json string value.

### importData(json, cells, row, column, option) (static) {#importdata}

Import the json string.

| Parameter | Type | Description |
| --- | --- | --- |
| json | String | The json string. |
| cells | Cells | The Cells. |
| row | Number | The row index. |
| column | Number | The column index. |
| option | JsonLayoutOptions | The options of import json string. |

**Returns:** Array of Number — `Array of Number`
