##ScenarioCollection
Represents the list of scenarios.
## ScenarioCollection class
Represents the list of scenarios.
```javascript
class ScenarioCollection;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [activeIndex](#activeIndex--)| number | Gets and sets which scenario is selected. |
| [lastSelected](#lastSelected--)| number | Indicates which scenario was last selected by the user to be run/shown. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Scenario](../scenario/) object by the index. |
| [getActiveIndex()](#getActiveIndex--)| <b>@deprecated.</b> Please use the 'activeIndex' property instead. Gets and sets which scenario is selected. |
| [setActiveIndex(number)](#setActiveIndex-number-)| <b>@deprecated.</b> Please use the 'activeIndex' property instead. Gets and sets which scenario is selected. |
| [getLastSelected()](#getLastSelected--)| <b>@deprecated.</b> Please use the 'lastSelected' property instead. Indicates which scenario was last selected by the user to be run/shown. |
| [setLastSelected(number)](#setLastSelected-number-)| <b>@deprecated.</b> Please use the 'lastSelected' property instead. Indicates which scenario was last selected by the user to be run/shown. |
| [add(string)](#add-string-)| Adds a scenario. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### activeIndex {#activeIndex--}
Gets and sets which scenario is selected.
```javascript
activeIndex : number;
```
### lastSelected {#lastSelected--}
Indicates which scenario was last selected by the user to be run/shown.
```javascript
lastSelected : number;
```
### get(number) {#get-number-}
Gets the [Scenario](../scenario/) object by the index.
```javascript
get(index: number) : Scenario;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The specific index in the list. |
**Returns**
[Scenario](../scenario/)
### getActiveIndex() {#getActiveIndex--}
```javascript
getActiveIndex() : number;
```
### setActiveIndex(number) {#setActiveIndex-number-}
```javascript
setActiveIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getLastSelected() {#getLastSelected--}
```javascript
getLastSelected() : number;
```
### setLastSelected(number) {#setLastSelected-number-}
```javascript
setLastSelected(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### add(string) {#add-string-}
Adds a scenario.
```javascript
add(name: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string | The name of scenario. |
**Returns**
The index in the list of scenarios.
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
