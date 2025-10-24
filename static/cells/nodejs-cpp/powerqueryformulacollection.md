##PowerQueryFormulaCollection
Represents all power query formulas in the mashup data.
## PowerQueryFormulaCollection class
Represents all power query formulas in the mashup data.
```javascript
class PowerQueryFormulaCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [ PowerQueryFormula](../ powerqueryformula/) by the index in the list. |
| [get(string)](#get-string-)| Gets [ PowerQueryFormula](../ powerqueryformula/) by the name of the power query formula. |
| [removeBy(string)](#removeBy-string-)| Remove power query formula by name. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets [ PowerQueryFormula](../ powerqueryformula/) by the index in the list.
```javascript
get(index: number) : PowerQueryFormula;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[PowerQueryFormula](../powerqueryformula/)
### get(string) {#get-string-}
Gets [ PowerQueryFormula](../ powerqueryformula/) by the name of the power query formula.
```javascript
get(name: string) : PowerQueryFormula;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of the item. |
**Returns**
[PowerQueryFormula](../powerqueryformula/)
### removeBy(string) {#removeBy-string-}
Remove power query formula by name.
```javascript
removeBy(name: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of power query formula. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
