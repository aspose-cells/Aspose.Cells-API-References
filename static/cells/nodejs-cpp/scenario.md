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
## Methods
| Method | Description |
| --- | --- |
| [getComment()](#getComment--)| <b>@deprecated.</b> Please use the 'comment' property instead. Gets and sets the comment of scenario. |
| [setComment(string)](#setComment-string-)| <b>@deprecated.</b> Please use the 'comment' property instead. Gets and sets the comment of scenario. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of scenario. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of scenario. |
| [getUser()](#getUser--)| <b>@deprecated.</b> Please use the 'user' property instead. Gets name of user who last changed the scenario. |
| [isHidden()](#isHidden--)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether scenario is hidden. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| <b>@deprecated.</b> Please use the 'isHidden' property instead. Indicates whether scenario is hidden. |
| [isLocked()](#isLocked--)| <b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether scenario is locked for editing when the sheet is protected. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| <b>@deprecated.</b> Please use the 'isLocked' property instead. Indicates whether scenario is locked for editing when the sheet is protected. |
| [getInputCells()](#getInputCells--)| <b>@deprecated.</b> Please use the 'inputCells' property instead. Gets the input cells of scenario. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getComment() {#getComment--}
```javascript
getComment() : string;
```
### setComment(string) {#setComment-string-}
```javascript
setComment(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getName() {#getName--}
```javascript
getName() : string;
```
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getUser() {#getUser--}
```javascript
getUser() : string;
```
### isHidden() {#isHidden--}
```javascript
isHidden() : boolean;
```
### setIsHidden(boolean) {#setIsHidden-boolean-}
```javascript
setIsHidden(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isLocked() {#isLocked--}
```javascript
isLocked() : boolean;
```
### setIsLocked(boolean) {#setIsLocked-boolean-}
```javascript
setIsLocked(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getInputCells() {#getInputCells--}
```javascript
getInputCells() : ScenarioInputCellCollection;
```
**Returns**
[ScenarioInputCellCollection](../scenarioinputcellcollection/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
