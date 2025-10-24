##ExportRangeToJsonOptions
Indicates the options that exporting range to json.
## ExportRangeToJsonOptions class
Indicates the options that exporting range to json.
```javascript
class ExportRangeToJsonOptions;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [hasHeaderRow](#hasHeaderRow--)| boolean | Indicates whether the range contains header row. |
| [exportAsString](#exportAsString--)| boolean | Exports the string value of the cells to json. |
| [exportEmptyCells](#exportEmptyCells--)| boolean | Indicates whether exporting empty cells as null. |
| [indent](#indent--)| string | Indicates the indent. |
## Methods
| Method | Description |
| --- | --- |
| [getHasHeaderRow()](#getHasHeaderRow--)| <b>@deprecated.</b> Please use the 'hasHeaderRow' property instead. Indicates whether the range contains header row. |
| [setHasHeaderRow(boolean)](#setHasHeaderRow-boolean-)| <b>@deprecated.</b> Please use the 'hasHeaderRow' property instead. Indicates whether the range contains header row. |
| [getExportAsString()](#getExportAsString--)| <b>@deprecated.</b> Please use the 'exportAsString' property instead. Exports the string value of the cells to json. |
| [setExportAsString(boolean)](#setExportAsString-boolean-)| <b>@deprecated.</b> Please use the 'exportAsString' property instead. Exports the string value of the cells to json. |
| [getExportEmptyCells()](#getExportEmptyCells--)| <b>@deprecated.</b> Please use the 'exportEmptyCells' property instead. Indicates whether exporting empty cells as null. |
| [setExportEmptyCells(boolean)](#setExportEmptyCells-boolean-)| <b>@deprecated.</b> Please use the 'exportEmptyCells' property instead. Indicates whether exporting empty cells as null. |
| [getIndent()](#getIndent--)| <b>@deprecated.</b> Please use the 'indent' property instead. Indicates the indent. |
| [setIndent(string)](#setIndent-string-)| <b>@deprecated.</b> Please use the 'indent' property instead. Indicates the indent. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### hasHeaderRow {#hasHeaderRow--}
Indicates whether the range contains header row.
```javascript
hasHeaderRow : boolean;
```
### exportAsString {#exportAsString--}
Exports the string value of the cells to json.
```javascript
exportAsString : boolean;
```
### exportEmptyCells {#exportEmptyCells--}
Indicates whether exporting empty cells as null.
```javascript
exportEmptyCells : boolean;
```
### indent {#indent--}
Indicates the indent.
```javascript
indent : string;
```
**Remarks**
If the indent is null or empty, the exported json is not formatted.
### getHasHeaderRow() {#getHasHeaderRow--}
```javascript
getHasHeaderRow() : boolean;
```
### setHasHeaderRow(boolean) {#setHasHeaderRow-boolean-}
```javascript
setHasHeaderRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getExportAsString() {#getExportAsString--}
```javascript
getExportAsString() : boolean;
```
### setExportAsString(boolean) {#setExportAsString-boolean-}
```javascript
setExportAsString(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getExportEmptyCells() {#getExportEmptyCells--}
```javascript
getExportEmptyCells() : boolean;
```
### setExportEmptyCells(boolean) {#setExportEmptyCells-boolean-}
```javascript
setExportEmptyCells(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getIndent() {#getIndent--}
```javascript
getIndent() : string;
```
**Remarks**
If the indent is null or empty, the exported json is not formatted.
### setIndent(string) {#setIndent-string-}
```javascript
setIndent(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If the indent is null or empty, the exported json is not formatted.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
