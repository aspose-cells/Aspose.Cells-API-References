##HorizontalPageBreakCollection
Encapsulates a collection of HorizontalPageBreak..horizontalpagebreak objects.
## HorizontalPageBreakCollection class
Encapsulates a collection of [HorizontalPageBreak](../horizontalpagebreak/) objects.
```javascript
class HorizontalPageBreakCollection;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
var excel = new Workbook();
//Add a pagebreak at G5
excel.worksheets.get(0).horizontalPageBreaks.add("G5");
excel.worksheets.get(0).verticalPageBreaks.add("G5");
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [HorizontalPageBreak](../horizontalpagebreak/) element at the specified index. |
| [get(string)](#get-string-)| Gets the [HorizontalPageBreak](../horizontalpagebreak/) element with the specified cell name. |
| [add(number, number, number)](#add-number-number-number-)| Adds a horizontal page break to the collection. |
| [add(number)](#add-number-)| Adds a horizontal page break to the collection. |
| [add(number, number)](#add-number-number-)| Adds a horizontal page break to the collection. |
| [add(string)](#add-string-)| Adds a horizontal page break to the collection. |
| [removeAt(number)](#removeAt-number-)| Removes the HPageBreak element at a specified name. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the [HorizontalPageBreak](../horizontalpagebreak/) element at the specified index.
```javascript
get(index: number) : HorizontalPageBreak;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### get(string) {#get-string-}
Gets the [HorizontalPageBreak](../horizontalpagebreak/) element with the specified cell name.
```javascript
get(cellName: string) : HorizontalPageBreak;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Cell name. |
**Returns**
The element with the specified cell name.
### add(number, number, number) {#add-number-number-number-}
Adds a horizontal page break to the collection.
```javascript
add(row: number, startColumn: number, endColumn: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Row index, zero based. |
| startColumn | number | Start column index, zero based. |
| endColumn | number | End column index, zero based. |
**Returns**
[HorizontalPageBreak](../horizontalpagebreak/) object index.
**Remarks**
This method is used to add a horizontal pagebreak within a print area.
### add(number) {#add-number-}
Adds a horizontal page break to the collection.
```javascript
add(row: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Cell row index, zero based. |
**Returns**
[HorizontalPageBreak](../horizontalpagebreak/) object index.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### add(number, number) {#add-number-number-}
Adds a horizontal page break to the collection.
```javascript
add(row: number, column: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Cell row index, zero based. |
| column | number | Cell column index, zero based. |
**Returns**
[HorizontalPageBreak](../horizontalpagebreak/) object index.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### add(string) {#add-string-}
Adds a horizontal page break to the collection.
```javascript
add(cellName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Cell name. |
**Returns**
[HorizontalPageBreak](../horizontalpagebreak/) object index.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### removeAt(number) {#removeAt-number-}
Removes the HPageBreak element at a specified name.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | Element index, zero based. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
