##VerticalPageBreakCollection
Encapsulates a collection of VerticalPageBreak..verticalpagebreak objects.
## VerticalPageBreakCollection class
Encapsulates a collection of [VerticalPageBreak](../verticalpagebreak/) objects.
```javascript
class VerticalPageBreakCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [VerticalPageBreak](../verticalpagebreak/) element at the specified index. |
| [get(string)](#get-string-)| Gets the [VerticalPageBreak](../verticalpagebreak/) element with the specified cell name. |
| [add(number, number, number)](#add-number-number-number-)| Adds a vertical page break to the collection. |
| [add(number)](#add-number-)| Adds a vertical page break to the collection. |
| [add(number, number)](#add-number-number-)| Adds a vertical page break to the collection. |
| [add(string)](#add-string-)| Adds a vertical page break to the collection. |
| [removeAt(number)](#removeAt-number-)| Removes the VPageBreak element at a specified name. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the [VerticalPageBreak](../verticalpagebreak/) element at the specified index.
```javascript
get(index: number) : VerticalPageBreak;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### get(string) {#get-string-}
Gets the [VerticalPageBreak](../verticalpagebreak/) element with the specified cell name.
```javascript
get(cellName: string) : VerticalPageBreak;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Cell name. |
**Returns**
The element with the specified cell name.
### add(number, number, number) {#add-number-number-number-}
Adds a vertical page break to the collection.
```javascript
add(startRow: number, endRow: number, column: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | Start row index, zero based. |
| endRow | number | End row index, zero based. |
| column | number | Column index, zero based. |
**Returns**
[VerticalPageBreak](../verticalpagebreak/) object index.
**Remarks**
This method is used to add a vertical pagebreak within a print area.
### add(number) {#add-number-}
Adds a vertical page break to the collection.
```javascript
add(column: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| column | number | Cell column index, zero based. |
**Returns**
[VerticalPageBreak](../verticalpagebreak/) object index.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### add(number, number) {#add-number-number-}
Adds a vertical page break to the collection.
```javascript
add(row: number, column: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | Cell row index, zero based. |
| column | number | Cell column index, zero based. |
**Returns**
[VerticalPageBreak](../verticalpagebreak/) object index.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### add(string) {#add-string-}
Adds a vertical page break to the collection.
```javascript
add(cellName: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | Cell name. |
**Returns**
[VerticalPageBreak](../verticalpagebreak/) object index.
**Remarks**
Page break is added in the top left of the cell. Please set a horizontal page break and a vertical page break concurrently.
### removeAt(number) {#removeAt-number-}
Removes the VPageBreak element at a specified name.
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
