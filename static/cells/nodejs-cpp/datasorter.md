##DataSorter
Summary description for DataSorter.
## DataSorter class
Summary description for DataSorter.
```javascript
class DataSorter;
```
### Example
```javascript
const { Workbook, CellArea, SortOrder } = require("aspose.cells.node");
//Instantiate a new Workbook object.
var workbook = new Workbook("input/DataSorter.xls");
//Get the workbook datasorter object.
var sorter = workbook.dataSorter;
//Set the first order for datasorter object.
sorter.order1 = SortOrder.Descending;
//Define the first key.
sorter.key1 = 0;
//Create a cells area (range).
var ca = new CellArea();
//Specify the start row index.
ca.startRow = 0;
//Specify the start column index.
ca.startColumn = 0;
//Specify the last row index.
ca.endRow = 12;
//Specify the last column index.
ca.endColumn = 1;
//Sort data in the specified data range (A1:B14)
sorter.sort(workbook.worksheets.get(0).cells, ca);
//Save the excel file.
workbook.save("output/DataSorter.xls");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [keys](#keys--)| DataSorterKeyCollection | Readonly. Gets the key list of data sorter. |
| [hasHeaders](#hasHeaders--)| boolean | Represents whether the range has headers. |
| [key1](#key1--)| number | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order1](#order1--)| SortOrder | Represents sort order of the first key. |
| [key2](#key2--)| number | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order2](#order2--)| SortOrder | Represents sort order of the second key. |
| [key3](#key3--)| number | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [order3](#order3--)| SortOrder | Represents sort order of the third key. |
| [sortLeftToRight](#sortLeftToRight--)| boolean | True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
| [caseSensitive](#caseSensitive--)| boolean | Gets and sets whether case sensitive when comparing string. |
| [sortAsNumber](#sortAsNumber--)| boolean | Indicates whether sorting anything that looks like a number. |
## Methods
| Method | Description |
| --- | --- |
| [getKeys()](#getKeys--)| <b>@deprecated.</b> Please use the 'keys' property instead. Gets the key list of data sorter. |
| [getHasHeaders()](#getHasHeaders--)| <b>@deprecated.</b> Please use the 'hasHeaders' property instead. Represents whether the range has headers. |
| [setHasHeaders(boolean)](#setHasHeaders-boolean-)| <b>@deprecated.</b> Please use the 'hasHeaders' property instead. Represents whether the range has headers. |
| [getKey1()](#getKey1--)| <b>@deprecated.</b> Please use the 'key1' property instead. Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey1(number)](#setKey1-number-)| <b>@deprecated.</b> Please use the 'key1' property instead. Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getOrder1()](#getOrder1--)| <b>@deprecated.</b> Please use the 'order1' property instead. Represents sort order of the first key. |
| [setOrder1(SortOrder)](#setOrder1-sortorder-)| <b>@deprecated.</b> Please use the 'order1' property instead. Represents sort order of the first key. |
| [getKey2()](#getKey2--)| <b>@deprecated.</b> Please use the 'key2' property instead. Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey2(number)](#setKey2-number-)| <b>@deprecated.</b> Please use the 'key2' property instead. Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getOrder2()](#getOrder2--)| <b>@deprecated.</b> Please use the 'order2' property instead. Represents sort order of the second key. |
| [setOrder2(SortOrder)](#setOrder2-sortorder-)| <b>@deprecated.</b> Please use the 'order2' property instead. Represents sort order of the second key. |
| [getKey3()](#getKey3--)| <b>@deprecated.</b> Please use the 'key3' property instead. Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey3(number)](#setKey3-number-)| <b>@deprecated.</b> Please use the 'key3' property instead. Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getOrder3()](#getOrder3--)| <b>@deprecated.</b> Please use the 'order3' property instead. Represents sort order of the third key. |
| [setOrder3(SortOrder)](#setOrder3-sortorder-)| <b>@deprecated.</b> Please use the 'order3' property instead. Represents sort order of the third key. |
| [getSortLeftToRight()](#getSortLeftToRight--)| <b>@deprecated.</b> Please use the 'sortLeftToRight' property instead. True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
| [setSortLeftToRight(boolean)](#setSortLeftToRight-boolean-)| <b>@deprecated.</b> Please use the 'sortLeftToRight' property instead. True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
| [getCaseSensitive()](#getCaseSensitive--)| <b>@deprecated.</b> Please use the 'caseSensitive' property instead. Gets and sets whether case sensitive when comparing string. |
| [setCaseSensitive(boolean)](#setCaseSensitive-boolean-)| <b>@deprecated.</b> Please use the 'caseSensitive' property instead. Gets and sets whether case sensitive when comparing string. |
| [getSortAsNumber()](#getSortAsNumber--)| <b>@deprecated.</b> Please use the 'sortAsNumber' property instead. Indicates whether sorting anything that looks like a number. |
| [setSortAsNumber(boolean)](#setSortAsNumber-boolean-)| <b>@deprecated.</b> Please use the 'sortAsNumber' property instead. Indicates whether sorting anything that looks like a number. |
| [clear()](#clear--)| Clear all settings. |
| [addKey(number, SortOrder)](#addKey-number-sortorder-)| Adds sorted column index and sort order. |
| [addKey(number, SortOrder, string)](#addKey-number-sortorder-string-)| Adds sorted column index and sort order with custom sort list. |
| [addKey(number, SortOnType, SortOrder, Object)](#addKey-number-sortontype-sortorder-object-)| Adds sorted column index and sort order with custom sort list. |
| [addKey(number, SortOrder, string[])](#addKey-number-sortorder-stringarray-)| Adds sorted column index and sort order with custom sort list. |
| [addColorKey(number, SortOnType, SortOrder, Color)](#addColorKey-number-sortontype-sortorder-color-)| Adds color sort key. |
| [sort(Cells, number, number, number, number)](#sort-cells-number-number-number-number-)| Sorts the data of the area. |
| [sort(Cells, CellArea)](#sort-cells-cellarea-)| Sort the data of the area. |
| [sort()](#sort--)| Sort the data in the range. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### keys {#keys--}
Readonly. Gets the key list of data sorter.
```javascript
keys : DataSorterKeyCollection;
```
### hasHeaders {#hasHeaders--}
Represents whether the range has headers.
```javascript
hasHeaders : boolean;
```
### key1 {#key1--}
Represents first sorted column index(absolute position, column A is 0, B is 1, ...).
```javascript
key1 : number;
```
### order1 {#order1--}
Represents sort order of the first key.
```javascript
order1 : SortOrder;
```
### key2 {#key2--}
Represents second sorted column index(absolute position, column A is 0, B is 1, ...).
```javascript
key2 : number;
```
### order2 {#order2--}
Represents sort order of the second key.
```javascript
order2 : SortOrder;
```
### key3 {#key3--}
Represents third sorted column index(absolute position, column A is 0, B is 1, ...).
```javascript
key3 : number;
```
### order3 {#order3--}
Represents sort order of the third key.
```javascript
order3 : SortOrder;
```
### sortLeftToRight {#sortLeftToRight--}
True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.
```javascript
sortLeftToRight : boolean;
```
### caseSensitive {#caseSensitive--}
Gets and sets whether case sensitive when comparing string.
```javascript
caseSensitive : boolean;
```
### sortAsNumber {#sortAsNumber--}
Indicates whether sorting anything that looks like a number.
```javascript
sortAsNumber : boolean;
```
### getKeys() {#getKeys--}
```javascript
getKeys() : DataSorterKeyCollection;
```
**Returns**
[DataSorterKeyCollection](../datasorterkeycollection/)
### getHasHeaders() {#getHasHeaders--}
```javascript
getHasHeaders() : boolean;
```
### setHasHeaders(boolean) {#setHasHeaders-boolean-}
```javascript
setHasHeaders(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getKey1() {#getKey1--}
```javascript
getKey1() : number;
```
### setKey1(number) {#setKey1-number-}
```javascript
setKey1(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getOrder1() {#getOrder1--}
```javascript
getOrder1() : SortOrder;
```
**Returns**
[SortOrder](../sortorder/)
### setOrder1(SortOrder) {#setOrder1-sortorder-}
```javascript
setOrder1(value: SortOrder) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SortOrder](../sortorder/) | The value to set. |
### getKey2() {#getKey2--}
```javascript
getKey2() : number;
```
### setKey2(number) {#setKey2-number-}
```javascript
setKey2(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getOrder2() {#getOrder2--}
```javascript
getOrder2() : SortOrder;
```
**Returns**
[SortOrder](../sortorder/)
### setOrder2(SortOrder) {#setOrder2-sortorder-}
```javascript
setOrder2(value: SortOrder) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SortOrder](../sortorder/) | The value to set. |
### getKey3() {#getKey3--}
```javascript
getKey3() : number;
```
### setKey3(number) {#setKey3-number-}
```javascript
setKey3(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getOrder3() {#getOrder3--}
```javascript
getOrder3() : SortOrder;
```
**Returns**
[SortOrder](../sortorder/)
### setOrder3(SortOrder) {#setOrder3-sortorder-}
```javascript
setOrder3(value: SortOrder) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SortOrder](../sortorder/) | The value to set. |
### getSortLeftToRight() {#getSortLeftToRight--}
```javascript
getSortLeftToRight() : boolean;
```
### setSortLeftToRight(boolean) {#setSortLeftToRight-boolean-}
```javascript
setSortLeftToRight(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCaseSensitive() {#getCaseSensitive--}
```javascript
getCaseSensitive() : boolean;
```
### setCaseSensitive(boolean) {#setCaseSensitive-boolean-}
```javascript
setCaseSensitive(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getSortAsNumber() {#getSortAsNumber--}
```javascript
getSortAsNumber() : boolean;
```
### setSortAsNumber(boolean) {#setSortAsNumber-boolean-}
```javascript
setSortAsNumber(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### clear() {#clear--}
Clear all settings.
```javascript
clear() : void;
```
### addKey(number, SortOrder) {#addKey-number-sortorder-}
Adds sorted column index and sort order.
```javascript
addKey(key: number, order: SortOrder) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order |
### addKey(number, SortOrder, string) {#addKey-number-sortorder-string-}
Adds sorted column index and sort order with custom sort list.
```javascript
addKey(key: number, order: SortOrder, customList: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | string | The custom sort list. |
### addKey(number, SortOnType, SortOrder, Object) {#addKey-number-sortontype-sortorder-object-}
Adds sorted column index and sort order with custom sort list.
```javascript
addKey(key: number, type: SortOnType, order: SortOrder, customList: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | [SortOnType](../sortontype/) | The sorted value type. |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | Object | The custom sort list. |
**Remarks**
If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.
### addKey(number, SortOrder, string[]) {#addKey-number-sortorder-stringarray-}
Adds sorted column index and sort order with custom sort list.
```javascript
addKey(key: number, order: SortOrder, customList: string[]) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | string[] | The custom sort list. |
### addColorKey(number, SortOnType, SortOrder, Color) {#addColorKey-number-sortontype-sortorder-color-}
Adds color sort key.
```javascript
addColorKey(key: number, type: SortOnType, order: SortOrder, color: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | [SortOnType](../sortontype/) | The sorted color value type. |
| order | [SortOrder](../sortorder/) | The sort order. |
| color | [Color](../color/) | The custom sort color. |
### sort(Cells, number, number, number, number) {#sort-cells-number-number-number-number-}
Sorts the data of the area.
```javascript
sort(cells: Cells, startRow: number, startColumn: number, endRow: number, endColumn: number) : number[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cells | [Cells](../cells/) | The cells contains the data area. |
| startRow | number | The start row of the area. |
| startColumn | number | The start column of the area. |
| endRow | number | The end row of the area. |
| endColumn | number | The end column of the area. |
**Returns**
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
### sort(Cells, CellArea) {#sort-cells-cellarea-}
Sort the data of the area.
```javascript
sort(cells: Cells, area: CellArea) : number[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cells | [Cells](../cells/) | The cells contains the data area. |
| area | [CellArea](../cellarea/) | The area needed to sort |
**Returns**
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
### sort() {#sort--}
Sort the data in the range.
```javascript
sort() : number[];
```
**Returns**
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
