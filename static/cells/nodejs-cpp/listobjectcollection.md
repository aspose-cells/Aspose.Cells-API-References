##ListObjectCollection
Represents a collection of ListObject..listobject objects in the worksheet.
## ListObjectCollection class
Represents a collection of [ListObject](../listobject/) objects in the worksheet.
```javascript
class ListObjectCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the ListObject by index. |
| [get(string)](#get-string-)| Gets the ListObject by specified name. |
| [add(number, number, number, number, boolean)](#add-number-number-number-number-boolean-)| Adds a ListObject to the worksheet. |
| [add(string, string, boolean)](#add-string-string-boolean-)| Adds a ListObject to the worksheet. |
| [updateColumnName()](#updateColumnName--)| Update all column name of the tables. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the ListObject by index.
```javascript
get(index: number) : ListObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
The ListObject
### get(string) {#get-string-}
Gets the ListObject by specified name.
```javascript
get(tableName: string) : ListObject;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tableName | string | ListObject name. |
**Returns**
The ListObject
### add(number, number, number, number, boolean) {#add-number-number-number-number-boolean-}
Adds a ListObject to the worksheet.
```javascript
add(startRow: number, startColumn: number, endRow: number, endColumn: number, hasHeaders: boolean) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row of the list range. |
| startColumn | number | The start row of the list range. |
| endRow | number | The start row of the list range. |
| endColumn | number | The start row of the list range. |
| hasHeaders | boolean | Whether the range has headers. |
**Returns**
The index of the new ListObject
### add(string, string, boolean) {#add-string-string-boolean-}
Adds a ListObject to the worksheet.
```javascript
add(startCell: string, endCell: string, hasHeaders: boolean) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startCell | string | The start cell of the list range. |
| endCell | string | The end cell of the list range. |
| hasHeaders | boolean | Whether the range has headers. |
**Returns**
The index of the new ListObject
### updateColumnName() {#updateColumnName--}
Update all column name of the tables.
```javascript
updateColumnName() : void;
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
