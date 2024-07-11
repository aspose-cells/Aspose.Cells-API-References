﻿---
title: JsonUtility
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the utility class of processing json.
type: docs
url: /nodejs-cpp/jsonutility/
---

## JsonUtility class

Represents the utility class of processing json.

```javascript
class JsonUtility;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| static [importData(string, Cells, number, number, JsonLayoutOptions)](#importData-string-cells-number-number-jsonlayoutoptions-)| Import the json string. |
| static [exportRangeToJson(Range, JsonSaveOptions)](#exportRangeToJson-range-jsonsaveoptions-)| Exporting the range to json file. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### importData(string, Cells, number, number, JsonLayoutOptions) {#importData-string-cells-number-number-jsonlayoutoptions-}

Import the json string.

```javascript
static importData(json: string, cells: Cells, row: number, column: number, option: JsonLayoutOptions) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| json | string | The json string. |
| cells | [Cells](./cells/) | The Cells. |
| row | number | The row index. |
| column | number | The column index. |
| option | [JsonLayoutOptions](./jsonlayoutoptions/) | The options of import json string. |

**Returns**

number[]

### exportRangeToJson(Range, JsonSaveOptions) {#exportRangeToJson-range-jsonsaveoptions-}

Exporting the range to json file.

```javascript
static exportRangeToJson(range: Range, options: JsonSaveOptions) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](./range/) | The range. |
| options | [JsonSaveOptions](./jsonsaveoptions/) | The options of exporting. |

**Returns**

The json string value.


