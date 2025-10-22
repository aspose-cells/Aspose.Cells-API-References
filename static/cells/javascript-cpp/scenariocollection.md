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
| [add(string)](#add-string-)| Adds a scenario. |
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
