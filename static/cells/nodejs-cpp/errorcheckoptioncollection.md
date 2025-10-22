##ErrorCheckOptionCollection
Represents all error check option.
## ErrorCheckOptionCollection class
Represents all error check option.
```javascript
class ErrorCheckOptionCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [ErrorCheckOption](../errorcheckoption/) object by the given index. |
| [add()](#add--)| Add an error check option. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets [ErrorCheckOption](../errorcheckoption/) object by the given index.
```javascript
get(index: number) : ErrorCheckOption;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index |
**Returns**
Return [ErrorCheckOption](../errorcheckoption/) object
### add() {#add--}
Add an error check option.
```javascript
add() : number;
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
