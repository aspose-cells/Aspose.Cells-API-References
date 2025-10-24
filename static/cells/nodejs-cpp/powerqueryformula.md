##PowerQueryFormula
Represents the definition of power query formula.
## PowerQueryFormula class
Represents the definition of power query formula.
```javascript
class PowerQueryFormula;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [groupName](#groupName--)| string | Readonly. Gets the name of group which contains this power query formula. |
| [name](#name--)| string | Gets and sets the name of the power query formula. |
| [description](#description--)| string | Gets and sets the description of the power query formula. |
| [powerQueryFormulaItems](#powerQueryFormulaItems--)| PowerQueryFormulaItemCollection | Readonly. Gets all items of power query formula. |
## Methods
| Method | Description |
| --- | --- |
| [getGroupName()](#getGroupName--)| <b>@deprecated.</b> Please use the 'groupName' property instead. Gets the name of group which contains this power query formula. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the power query formula. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the power query formula. |
| [getDescription()](#getDescription--)| <b>@deprecated.</b> Please use the 'description' property instead. Gets and sets the description of the power query formula. |
| [setDescription(string)](#setDescription-string-)| <b>@deprecated.</b> Please use the 'description' property instead. Gets and sets the description of the power query formula. |
| [getPowerQueryFormulaItems()](#getPowerQueryFormulaItems--)| <b>@deprecated.</b> Please use the 'powerQueryFormulaItems' property instead. Gets all items of power query formula. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getType()](#getType--)| Gets the type of this power query formula. |
| [getFormulaDefinition()](#getFormulaDefinition--)| Gets the definition of the power query formula. |
### groupName {#groupName--}
Readonly. Gets the name of group which contains this power query formula.
```javascript
groupName : string;
```
### name {#name--}
Gets and sets the name of the power query formula.
```javascript
name : string;
```
### description {#description--}
Gets and sets the description of the power query formula.
```javascript
description : string;
```
### powerQueryFormulaItems {#powerQueryFormulaItems--}
Readonly. Gets all items of power query formula.
```javascript
powerQueryFormulaItems : PowerQueryFormulaItemCollection;
```
### getGroupName() {#getGroupName--}
```javascript
getGroupName() : string;
```
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
### getDescription() {#getDescription--}
```javascript
getDescription() : string;
```
### setDescription(string) {#setDescription-string-}
```javascript
setDescription(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getPowerQueryFormulaItems() {#getPowerQueryFormulaItems--}
```javascript
getPowerQueryFormulaItems() : PowerQueryFormulaItemCollection;
```
**Returns**
[PowerQueryFormulaItemCollection](../powerqueryformulaitemcollection/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getType() {#getType--}
Gets the type of this power query formula.
```javascript
getType() : PowerQueryFormulaType;
```
**Returns**
[PowerQueryFormulaType](../powerqueryformulatype/)
### getFormulaDefinition() {#getFormulaDefinition--}
Gets the definition of the power query formula.
```javascript
getFormulaDefinition() : string;
```
