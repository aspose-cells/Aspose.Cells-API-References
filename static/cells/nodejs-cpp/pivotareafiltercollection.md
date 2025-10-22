##PivotAreaFilterCollection
Represents the list of filters for PivotArea..pivotarea
## PivotAreaFilterCollection class
Represents the list of filters for [PivotArea](../pivotarea/)
```javascript
class PivotAreaFilterCollection;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets filter from the list by the index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### get(number) {#get-number-}
Gets filter from the list by the index.
```javascript
get(index: number) : PivotAreaFilter;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The Index |
**Returns**
[PivotAreaFilter](../pivotareafilter/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
