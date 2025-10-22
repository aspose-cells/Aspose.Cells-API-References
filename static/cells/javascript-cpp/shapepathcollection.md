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
| [add()](#add--)| Add a creation path. |
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
### add() {#add--}
Add a creation path.
```javascript
add() : number;
```
**Returns**
Returns [ShapePath](../shapepath/) object.
