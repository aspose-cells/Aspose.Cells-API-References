##SmartTagCollection
Represents all smart tags in the cell.
## SmartTagCollection class
Represents all smart tags in the cell.
```javascript
class SmartTagCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [row](#row--)| number | Readonly. Gets the row of the cell smart tags. |
| [column](#column--)| number | Readonly. Gets the column of the cell smart tags. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [SmartTag](../smarttag/) object at the specific index |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets the row of the cell smart tags. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets the column of the cell smart tags. |
| [add(string, string)](#add-string-string-)| Adds a smart tag. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### row {#row--}
Readonly. Gets the row of the cell smart tags.
```javascript
row : number;
```
### column {#column--}
Readonly. Gets the column of the cell smart tags.
```javascript
column : number;
```
### get(number) {#get-number-}
Gets a [SmartTag](../smarttag/) object at the specific index
```javascript
get(index: number) : SmartTag;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
returns a [SmartTag](../smarttag/) object.
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### add(string, string) {#add-string-string-}
Adds a smart tag.
```javascript
add(uri: string, name: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uri | string | Specifies the namespace URI of the smart tag |
| name | string | Specifies the name of the smart tag. |
**Returns**
The index of smart tag in the list.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
