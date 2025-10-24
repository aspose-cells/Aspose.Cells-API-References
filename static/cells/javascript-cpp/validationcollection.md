##ValidationCollection
Represents data validation collection.
## ValidationCollection class
Represents data validation collection.
```javascript
class ValidationCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Validation](../validation/) element at the specified index. |
| [add(CellArea)](#add-cellarea-)| Adds a data validation to the collection. |
| [removeACell(number, number)](#removeACell-number-number-)| Removes all validation setting on the cell. |
| [removeArea(CellArea)](#removeArea-cellarea-)| Removes all validation setting on the range.. |
| [getValidationInCell(number, number)](#getValidationInCell-number-number-)| Gets the validation applied to given cell. |
### get(number) {#get-number-}
Gets the [Validation](../validation/) element at the specified index.
```javascript
get(index: number) : Validation;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(CellArea) {#add-cellarea-}
Adds a data validation to the collection.
```javascript
add(ca: CellArea) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The area contains this validation. |
**Returns**
[Validation](../validation/) object index.
### removeACell(number, number) {#removeACell-number-number-}
Removes all validation setting on the cell.
```javascript
removeACell(row: number, column: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index of the cell. |
| column | number | The column index of the cell. |
### removeArea(CellArea) {#removeArea-cellarea-}
Removes all validation setting on the range..
```javascript
removeArea(ca: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The range which contains the validations setting. |
### getValidationInCell(number, number) {#getValidationInCell-number-number-}
Gets the validation applied to given cell.
```javascript
getValidationInCell(row: number, column: number) : Validation;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
Returns a [Validation](../validation/) object or null if there is no validation for given cell
