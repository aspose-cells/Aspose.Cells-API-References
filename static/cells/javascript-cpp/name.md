##Name
Represents a defined name for a range of cells.
## Name class
Represents a defined name for a range of cells.
```javascript
class Name;
```
### Example
```javascript
const { Workbook, SaveFormat } = AsposeCells;
//Instantiating a Workbook object
var workbook = new Workbook();
//Accessing the first worksheet in the Excel file
var worksheet = workbook.worksheets.get(0);
//Creating a named range
var range = worksheet.cells.createRange("B4", "G14");
//Setting the name of the named range
range.setName("TestRange");
//Saving the modified Excel file in default (that is Excel 2000) format
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [comment](#comment--)| string | Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions. |
| [text](#text--)| string | Gets the name text of the object. |
| [fullText](#fullText--)| string | Readonly. Gets the name  full text of the object with the scope setting. |
| [refersTo](#refersTo--)| string | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [r1C1RefersTo](#r1C1RefersTo--)| string | Gets or sets a R1C1 reference of the [Name](../name/). |
| [isReferred](#isReferred--)| boolean | Readonly. Indicates whether this name is referred by other formulas. |
| [isVisible](#isVisible--)| boolean | Indicates whether the name is visible. |
| [sheetIndex](#sheetIndex--)| number | Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |
## Methods
| Method | Description |
| --- | --- |
| [getRefersTo(boolean, boolean)](#getRefersTo-boolean-boolean-)| Get the reference of this Name. |
| [getRefersTo(boolean, boolean, number, number)](#getRefersTo-boolean-boolean-number-number-)| Get the reference of this Name based on specified cell. |
| [setRefersTo(string, boolean, boolean)](#setRefersTo-string-boolean-boolean-)| Set the reference of this Name. |
| [getRanges()](#getRanges--)| Gets all ranges referred by this name. |
| [getRanges(boolean)](#getRanges-boolean-)| Gets all ranges referred by this name. |
| [getReferredAreas(boolean)](#getReferredAreas-boolean-)| Gets all references referred by this name. |
| [getRange()](#getRange--)| Gets the range if this name refers to a range. |
| [getRange(boolean)](#getRange-boolean-)| Gets the range if this name refers to a range |
| [getRange(number, number, number)](#getRange-number-number-number-)| Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell. |
| [toString()](#toString--)| Returns a string represents the current Range object. |
### comment {#comment--}
Gets and sets the comment of the name. Only applies for Excel 2007 or higher versions.
```javascript
comment : string;
```
### text {#text--}
Gets the name text of the object.
```javascript
text : string;
```
### fullText {#fullText--}
Readonly. Gets the name  full text of the object with the scope setting.
```javascript
fullText : string;
```
### refersTo {#refersTo--}
Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.
```javascript
refersTo : string;
```
### r1C1RefersTo {#r1C1RefersTo--}
Gets or sets a R1C1 reference of the [Name](../name/).
```javascript
r1C1RefersTo : string;
```
### isReferred {#isReferred--}
Readonly. Indicates whether this name is referred by other formulas.
```javascript
isReferred : boolean;
```
### isVisible {#isVisible--}
Indicates whether the name is visible.
```javascript
isVisible : boolean;
```
### sheetIndex {#sheetIndex--}
Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)
```javascript
sheetIndex : number;
```
### getRefersTo(boolean, boolean) {#getRefersTo-boolean-boolean-}
Get the reference of this Name.
```javascript
getRefersTo(isR1C1: boolean, isLocal: boolean) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |
### getRefersTo(boolean, boolean, number, number) {#getRefersTo-boolean-boolean-number-number-}
Get the reference of this Name based on specified cell.
```javascript
getRefersTo(isR1C1: boolean, isLocal: boolean, row: number, column: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |
| row | number | The row index of the cell. |
| column | number | The column index of the cell. |
### setRefersTo(string, boolean, boolean) {#setRefersTo-string-boolean-boolean-}
Set the reference of this Name.
```javascript
setRefersTo(refersTo: string, isR1C1: boolean, isLocal: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| refersTo | string | The reference. |
| isR1C1 | boolean | Whether the reference is R1C1 format. |
| isLocal | boolean | Whether the reference is locale formatted. |
### getRanges() {#getRanges--}
Gets all ranges referred by this name.
```javascript
getRanges() : Range[];
```
**Returns**
All ranges.
### getRanges(boolean) {#getRanges-boolean-}
Gets all ranges referred by this name.
```javascript
getRanges(recalculate: boolean) : Range[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |
**Returns**
All ranges.
### getReferredAreas(boolean) {#getReferredAreas-boolean-}
Gets all references referred by this name.
```javascript
getReferredAreas(recalculate: boolean) : ReferredArea[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |
**Returns**
All ranges.
### getRange() {#getRange--}
Gets the range if this name refers to a range.
```javascript
getRange() : Range;
```
**Returns**
The range.
### getRange(boolean) {#getRange-boolean-}
Gets the range if this name refers to a range
```javascript
getRange(recalculate: boolean) : Range;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |
**Returns**
The range.
### getRange(number, number, number) {#getRange-number-number-number-}
Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell.
```javascript
getRange(sheetIndex: number, row: number, column: number) : Range;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | number | The according sheet index. |
| row | number | The according row index. |
| column | number | The according column index |
**Returns**
The range.
### toString() {#toString--}
Returns a string represents the current Range object.
```javascript
toString() : string;
```
