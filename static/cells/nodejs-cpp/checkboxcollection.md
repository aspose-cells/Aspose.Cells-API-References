##CheckBoxCollection
Represents a collection of CheckBox..checkbox objects in a worksheet.
## CheckBoxCollection class
Represents a collection of [CheckBox](../checkbox/) objects in a worksheet.
```javascript
class CheckBoxCollection;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
var excel = new Workbook();
var index = excel.worksheets.get(0).getCheckBoxes().add(15, 15, 20, 100);
var checkBox = excel.worksheets.get(0).getCheckBoxes().get(index);
checkBox.text = "Check Box 1";
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [CheckBox](../checkbox/) element at the specified index. |
| [add(number, number, number, number)](#add-number-number-number-number-)| Adds a checkBox to the collection. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the [CheckBox](../checkbox/) element at the specified index.
```javascript
get(index: number) : CheckBox;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(number, number, number, number) {#add-number-number-number-number-}
Adds a checkBox to the collection.
```javascript
add(upperLeftRow: number, upperLeftColumn: number, height: number, width: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| height | number | Height of checkBox, in unit of pixel. |
| width | number | Width of checkBox, in unit of pixel. |
**Returns**
[CheckBox](../checkbox/) object index.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
