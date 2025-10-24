##LegendEntryCollection
Represents a collection of all the LegendEntry..legendentry objects in the specified chart legend.
## LegendEntryCollection class
Represents a collection of all the [LegendEntry](../legendentry/) objects in the specified chart legend.
```javascript
class LegendEntryCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [LegendEntry](../legendentry/) element at the specified index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the [LegendEntry](../legendentry/) element at the specified index.
```javascript
get(index: number) : LegendEntry;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |
**Returns**
The element at the specified index.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
