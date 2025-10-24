##HyperlinkCollection
Encapsulates a collection of Hyperlink..hyperlink objects.
## HyperlinkCollection class
Encapsulates a collection of [Hyperlink](../hyperlink/) objects.
```javascript
class HyperlinkCollection;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
//Instantiating a Workbook object
var workbook = new Workbook();
//Obtaining the reference of the newly added worksheet by passing its sheet index
var worksheet = workbook.worksheets.get(0);
//Get Hyperlinks Collection
var hyperlinks = worksheet.hyperlinks;
//Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "https://www.aspose.com");
//Saving the Excel file
workbook.save("output/HyperlinkCollection.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Hyperlink](../hyperlink/) element at the specified index. |
| [add(number, number, number, number, string)](#add-number-number-number-number-string-)| Adds a hyperlink to a specified cell or a range of cells. |
| [add(string, number, number, string)](#add-string-number-number-string-)| Adds a hyperlink to a specified cell or a range of cells. |
| [add(string, string, string, string, string)](#add-string-string-string-string-string-)| Adds a hyperlink to a specified cell or a range of cells. |
| [removeAt(number)](#removeAt-number-)| Remove the hyperlink  at the specified index in this collection. |
| [clear()](#clear--)| Clears all hyperlinks. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the [Hyperlink](../hyperlink/) element at the specified index.
```javascript
get(index: number) : Hyperlink;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(number, number, number, number, string) {#add-number-number-number-number-string-}
Adds a hyperlink to a specified cell or a range of cells.
```javascript
add(firstRow: number, firstColumn: number, totalRows: number, totalColumns: number, address: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| firstRow | number | First row of the hyperlink range. |
| firstColumn | number | First column of the hyperlink range. |
| totalRows | number | Number of rows in this hyperlink range. |
| totalColumns | number | Number of columns of this hyperlink range. |
| address | string | Address of the hyperlink. |
**Returns**
[Hyperlink](../hyperlink/) object index.
**Example**
```javascript
const { Workbook } = require("aspose.cells.node");
var excel = new Workbook();
var worksheet = excel.worksheets.get(0);
worksheet.hyperlinks.add("A4", 1, 1, "https://www.aspose.com");
worksheet.hyperlinks.add("A5", 1, 1, "c:\\book1.xls");
```
### add(string, number, number, string) {#add-string-number-number-string-}
Adds a hyperlink to a specified cell or a range of cells.
```javascript
add(cellName: string, totalRows: number, totalColumns: number, address: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Cell name. |
| totalRows | number | Number of rows in this hyperlink range. |
| totalColumns | number | Number of columns of this hyperlink range. |
| address | string | Address of the hyperlink. |
**Returns**
[Hyperlink](../hyperlink/) object index.
### add(string, string, string, string, string) {#add-string-string-string-string-string-}
Adds a hyperlink to a specified cell or a range of cells.
```javascript
add(startCellName: string, endCellName: string, address: string, textToDisplay: string, screenTip: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | string | The top-left cell of the range. |
| endCellName | string | The bottom-right cell of the range. |
| address | string | Address of the hyperlink. |
| textToDisplay | string | The text to be displayed for the specified hyperlink. |
| screenTip | string | The screenTip text for the specified hyperlink. |
**Returns**
[Hyperlink](../hyperlink/) object index.
### removeAt(number) {#removeAt-number-}
Remove the hyperlink  at the specified index in this collection.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
### clear() {#clear--}
Clears all hyperlinks.
```javascript
clear() : void;
```
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
