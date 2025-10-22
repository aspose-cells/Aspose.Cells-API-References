##PivotFieldCollection
Represents a collection of all the PivotField objects in the PivotTables specific PivotFields type.
## PivotFieldCollection class
Represents a collection of all the PivotField objects in the PivotTable's specific PivotFields type.
```javascript
class PivotFieldCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| PivotFieldType | Readonly. Gets the PivotFields type. |
| [count](#count--)| number | Readonly. Gets the count of the pivotFields. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the PivotField Object at the specific index. |
| [get(string)](#get-string-)| Gets the PivotField Object of the specific name. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the PivotFields type. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the count of the pivotFields. |
| [getEnumerator()](#getEnumerator--)| Gets an enumerator over the elements in this collection in proper sequence. |
| [addByBaseIndex(number)](#addByBaseIndex-number-)| Adds a PivotField Object to the specific type PivotFields. |
| [add(PivotField)](#add-pivotfield-)| Adds a PivotField Object to the specific type PivotFields. |
| [clear()](#clear--)| clear all fields of PivotFieldCollection |
| [move(number, number)](#move-number-number-)| Moves the PivotField from current position to destination position |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### type {#type--}
Readonly. Gets the PivotFields type.
```javascript
type : PivotFieldType;
```
### count {#count--}
Readonly. Gets the count of the pivotFields.
```javascript
count : number;
```
### get(number) {#get-number-}
Gets the PivotField Object at the specific index.
```javascript
get(index: number) : PivotField;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
[PivotField](../pivotfield/)
### get(string) {#get-string-}
Gets the PivotField Object of the specific name.
```javascript
get(name: string) : PivotField;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |
**Returns**
[PivotField](../pivotfield/)
### getType() {#getType--}
```javascript
getType() : PivotFieldType;
```
**Returns**
[PivotFieldType](../pivotfieldtype/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### getEnumerator() {#getEnumerator--}
Gets an enumerator over the elements in this collection in proper sequence.
```javascript
getEnumerator() : PivotFieldEnumerator;
```
**Returns**
enumerator
### addByBaseIndex(number) {#addByBaseIndex-number-}
Adds a PivotField Object to the specific type PivotFields.
```javascript
addByBaseIndex(baseFieldIndex: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| baseFieldIndex | number | field index in the base PivotFields. |
**Returns**
the index of  the PivotField Object in this PivotFields.
### add(PivotField) {#add-pivotfield-}
Adds a PivotField Object to the specific type PivotFields.
```javascript
add(pivotField: PivotField) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotField | [PivotField](../pivotfield/) | a PivotField Object. |
**Returns**
the index of  the PivotField Object in this PivotFields.
### clear() {#clear--}
clear all fields of PivotFieldCollection
```javascript
clear() : void;
```
### move(number, number) {#move-number-number-}
Moves the PivotField from current position to destination position
```javascript
move(currPos: number, destPos: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| currPos | number | Current position of PivotField based on zero |
| destPos | number | Destination position of PivotField based on zero |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
