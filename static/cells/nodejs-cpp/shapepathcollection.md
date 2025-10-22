##ShapePathCollection
Represents path collection information in NotPrimitive autoshape
## ShapePathCollection class
Represents path collection information in NotPrimitive autoshape
```javascript
class ShapePathCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of paths |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a creation path. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the count of paths |
| [add()](#add--)| Add a creation path. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### count {#count--}
Readonly. Gets the count of paths
```javascript
count : number;
```
### get(number) {#get-number-}
Gets a creation path.
```javascript
get(index: number) : ShapePath;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
Returns [ShapePath](../shapepath/) object.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### add() {#add--}
Add a creation path.
```javascript
add() : number;
```
**Returns**
Returns [ShapePath](../shapepath/) object.
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
