##PivotAreaCollection
Represents a list of pivot area.
## PivotAreaCollection class
Represents a list of pivot area.
```javascript
class PivotAreaCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [PivotArea](../pivotarea/) object; |
| [add(PivotArea)](#add-pivotarea-)| Adds pivot area. |
| [add(CellArea)](#add-cellarea-)| Adds an area based on pivot table view. |
| [removeAt(number)](#removeAt-number-)| Remove one pivot conditional formatted area setting. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets a [PivotArea](../pivotarea/) object;
```javascript
get(index: number) : PivotArea;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
**Returns**
[PivotArea](../pivotarea/)
### add(PivotArea) {#add-pivotarea-}
Adds pivot area.
```javascript
add(pivotArea: PivotArea) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotArea | [PivotArea](../pivotarea/) | The pivot area. |
### add(CellArea) {#add-cellarea-}
Adds an area based on pivot table view.
```javascript
add(cellArea: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | The area based on pivot table view. |
### removeAt(number) {#removeAt-number-}
Remove one pivot conditional formatted area setting.
```javascript
removeAt(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
