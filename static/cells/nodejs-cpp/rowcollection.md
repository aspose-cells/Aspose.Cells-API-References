##RowCollection
Collects the Row..row objects that represent the individual rows in a worksheet.
## RowCollection class
Collects the [Row](../row/) objects that represent the individual rows in a worksheet.
```javascript
class RowCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the number of rows in this collection. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Row](../row/) object by given row index. The Row object of given row index will be instantiated if it does not exist before. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of rows in this collection. |
| [getEnumerator()](#getEnumerator--)| Gets an enumerator that iterates rows through this collection |
| [getEnumerator(boolean, boolean)](#getEnumerator-boolean-boolean-)| Gets an enumerator that iterates rows through this collection |
| [getRowByIndex(number)](#getRowByIndex-number-)| Gets the row object by the position in the list. |
| [clear()](#clear--)| Clear all rows and cells. |
| [removeAt(number)](#removeAt-number-)| Remove the row item at the specified index(position) in this collection. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### count {#count--}
Readonly. Gets the number of rows in this collection.
```javascript
count : number;
```
### get(number) {#get-number-}
Gets a [Row](../row/) object by given row index. The Row object of given row index will be instantiated if it does not exist before.
```javascript
get(rowIndex: number) : Row;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowIndex | number |  |
**Returns**
[Row](../row/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### getEnumerator() {#getEnumerator--}
Gets an enumerator that iterates rows through this collection
```javascript
getEnumerator() : RowEnumerator;
```
**Returns**
The row enumerator which will traverse all existing rows in this collection.
### getEnumerator(boolean, boolean) {#getEnumerator-boolean-boolean-}
Gets an enumerator that iterates rows through this collection
```javascript
getEnumerator(reversed: boolean, sync: boolean) : RowEnumerator;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| reversed | boolean | whether enumerate rows in reversed order |
| sync | boolean | whether the returned enumerator should check the modification of row collection         /// and keep synchronized with it. |
**Returns**
The row enumerator which will traverse all existing rows in this collection.
**Remarks**
If the row collection will be modified(by operations that may cause new Row be instantiated or existing Row be removed) during the traversal with the enumerator, synchronized enumerator should be used instead of normal enumerator so that the traversal can continue from the position just after the one has been traversed by the last MoveNext(). However, together with the advantage that no element be skipped or traversed repeatedly, the disadvantage for synchronized enumerator is that the performance will be degraded a bit when comparing with normal enumerator.
### getRowByIndex(number) {#getRowByIndex-number-}
Gets the row object by the position in the list.
```javascript
getRowByIndex(index: number) : Row;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position. |
**Returns**
The Row object at given position.
### clear() {#clear--}
Clear all rows and cells.
```javascript
clear() : void;
```
### removeAt(number) {#removeAt-number-}
Remove the row item at the specified index(position) in this collection.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | zero-based index(position, not [Row.Index](../row.index/)) of the existing row item in this collection. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
