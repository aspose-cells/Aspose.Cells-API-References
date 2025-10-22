##PivotConditionalFormatCollection
Represents all conditional formats of pivot table.
## PivotConditionalFormatCollection class
Represents all conditional formats of pivot table.
```javascript
class PivotConditionalFormatCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the pivot FormatCondition object at the specific index. |
| [add()](#add--)| Adds a pivot FormatCondition to the collection. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the pivot FormatCondition object at the specific index.
```javascript
get(index: number) : PivotConditionalFormat;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
pivot FormatCondition object.
### add() {#add--}
Adds a pivot FormatCondition to the collection.
```javascript
add() : number;
```
**Returns**
pivot FormatCondition object index.
**Remarks**
not supported
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
