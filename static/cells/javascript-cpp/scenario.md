##Scenario
Represents an individual scenario.
## Scenario class
Represents an individual scenario.
```javascript
class Scenario;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [comment](#comment--)| string | Gets and sets the comment of scenario. |
| [name](#name--)| string | Gets and sets the name of scenario. |
| [user](#user--)| string | Readonly. Gets name of user who last changed the scenario. |
| [isHidden](#isHidden--)| boolean | Indicates whether scenario is hidden. |
| [isLocked](#isLocked--)| boolean | Indicates whether scenario is locked for editing when the sheet is protected. |
| [inputCells](#inputCells--)| ScenarioInputCellCollection | Readonly. Gets the input cells of scenario. |
### comment {#comment--}
Gets and sets the comment of scenario.
```javascript
comment : string;
```
### name {#name--}
Gets and sets the name of scenario.
```javascript
name : string;
```
### user {#user--}
Readonly. Gets name of user who last changed the scenario.
```javascript
user : string;
```
### isHidden {#isHidden--}
Indicates whether scenario is hidden.
```javascript
isHidden : boolean;
```
### isLocked {#isLocked--}
Indicates whether scenario is locked for editing when the sheet is protected.
```javascript
isLocked : boolean;
```
### inputCells {#inputCells--}
Readonly. Gets the input cells of scenario.
```javascript
inputCells : ScenarioInputCellCollection;
```
