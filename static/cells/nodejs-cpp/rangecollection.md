##RangeCollection
Encapsulates a collection of Range..range objects.
## RangeCollection class
Encapsulates a collection of [Range](../range/) objects.
```javascript
class RangeCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Range](../range/) element at the specified index. |
| [add(Range)](#add-range-)| Adds a [Range](../range/) item to the collection. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the [Range](../range/) element at the specified index.
```javascript
get(index: number) : Range;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(Range) {#add-range-}
Adds a [Range](../range/) item to the collection.
```javascript
add(range: Range) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | Range object |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
