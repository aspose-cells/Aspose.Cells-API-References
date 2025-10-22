##DataSorterKeyCollection
Represents the key list of data sorter.
## DataSorterKeyCollection class
Represents the key list of data sorter.
```javascript
class DataSorterKeyCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets and sets [DataSorterKey](../datasorterkey/) by index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### get(number) {#get-number-}
Gets and sets [DataSorterKey](../datasorterkey/) by index.
```javascript
get(index: number) : DataSorterKey;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[DataSorterKey](../datasorterkey/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
