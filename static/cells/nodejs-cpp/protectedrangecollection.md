##ProtectedRangeCollection
Encapsulates a collection of ProtectedRange..protectedrange objects.
## ProtectedRangeCollection class
Encapsulates a collection of [ProtectedRange](../protectedrange/) objects.
```javascript
class ProtectedRangeCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [ProtectedRange](../protectedrange/) element at the specified index. |
| [add(string, number, number, number, number)](#add-string-number-number-number-number-)| Adds a [ProtectedRange](../protectedrange/) item to the collection. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the [ProtectedRange](../protectedrange/) element at the specified index.
```javascript
get(index: number) : ProtectedRange;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### add(string, number, number, number, number) {#add-string-number-number-number-number-}
Adds a [ProtectedRange](../protectedrange/) item to the collection.
```javascript
add(name: string, startRow: number, startColumn: number, endRow: number, endColumn: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | Range title. This is used as a descriptor, not as a named range definition. |
| startRow | number | Start row index of the range. |
| startColumn | number | Start column index of the range. |
| endRow | number | End row index of the range. |
| endColumn | number | End column index of the range. |
**Returns**
object index.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
