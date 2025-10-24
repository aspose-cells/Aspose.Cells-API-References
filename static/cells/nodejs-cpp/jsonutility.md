##JsonUtility
Represents the utility class of processing json.
## JsonUtility class
Represents the utility class of processing json.
```javascript
class JsonUtility;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| static [importData(string, Cells, number, number, JsonLayoutOptions)](#importData-string-cells-number-number-jsonlayoutoptions-)| Import the json string. |
| static [exportRangeToJson(Range, JsonSaveOptions)](#exportRangeToJson-range-jsonsaveoptions-)| Exporting the range to json file. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
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
| cells | [Cells](../cells/) | The Cells. |
| row | number | The row index. |
| column | number | The column index. |
| option | [JsonLayoutOptions](../jsonlayoutoptions/) | The options of import json string. |
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
| range | [Range](../range/) | The range. |
| options | [JsonSaveOptions](../jsonsaveoptions/) | The options of exporting. |
**Returns**
The json string value.
