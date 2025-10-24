##SparklineCollection
Encapsulates a collection of Sparkline..sparkline objects.
## SparklineCollection class
Encapsulates a collection of [Sparkline](../sparkline/) objects.
```javascript
class SparklineCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Sparkline](../sparkline/) element at the specified index. |
| [add(string, number, number)](#add-string-number-number-)| Add a sparkline. |
| [remove(VObject)](#remove-vobject-)| Removes the sparkline |
### get(number) {#get-number-}
Gets the [Sparkline](../sparkline/) element at the specified index.
```javascript
get(index: number) : Sparkline;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(string, number, number) {#add-string-number-number-}
Add a sparkline.
```javascript
add(dataRange: string, row: number, column: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | string | Specifies the new data range of the sparkline. |
| row | number | The row index of the location. |
| column | number | The column index of the location. |
### remove(VObject) {#remove-vobject-}
Removes the sparkline
```javascript
remove(o: VObject) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| o | VObject |  |
