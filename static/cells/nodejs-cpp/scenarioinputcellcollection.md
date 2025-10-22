##ScenarioInputCellCollection
Represents the list of the scenarios input cells.
## ScenarioInputCellCollection class
Represents the list of the scenario's input cells.
```javascript
class ScenarioInputCellCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [ScenarioInputCell](../scenarioinputcell/) by index in the list. |
| [add(number, number, string)](#add-number-number-string-)| Adds an input cell. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets [ScenarioInputCell](../scenarioinputcell/) by index in the list.
```javascript
get(index: number) : ScenarioInputCell;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The specific index in the list |
**Returns**
The [ScenarioInputCell](../scenarioinputcell/) object
### add(number, number, string) {#add-number-number-string-}
Adds an input cell.
```javascript
add(row: number, column: number, value: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index of input cell. |
| column | number | The column index of input cell. |
| value | string | The value of input cell. |
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
