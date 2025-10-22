##PowerQueryFormulaFunction
Represents the function of power query.
## PowerQueryFormulaFunction class
Represents the function of power query.
```javascript
class PowerQueryFormulaFunction extends PowerQueryFormula;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(PowerQueryFormula)](#constructor-powerqueryformula-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [f](#f--)| string | Gets and sets the definition of function. |
| [groupName](#groupName--)| string | Readonly. Gets the name of group which contains this power query formula. |
| [name](#name--)| string | Gets and sets the name of the power query formula. |
| [description](#description--)| string | Gets and sets the description of the power query formula. |
| [powerQueryFormulaItems](#powerQueryFormulaItems--)| PowerQueryFormulaItemCollection | Readonly. Gets all items of power query formula. |
## Methods
| Method | Description |
| --- | --- |
| [getF()](#getF--)| <b>@deprecated.</b> Please use the 'f' property instead. Gets and sets the definition of function. |
| [setF(string)](#setF-string-)| <b>@deprecated.</b> Please use the 'f' property instead. Gets and sets the definition of function. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getGroupName()](#getGroupName--)| <b>@deprecated.</b> Please use the 'groupName' property instead. Gets the name of group which contains this power query formula. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the power query formula. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the power query formula. |
| [getDescription()](#getDescription--)| <b>@deprecated.</b> Please use the 'description' property instead. Gets and sets the description of the power query formula. |
| [setDescription(string)](#setDescription-string-)| <b>@deprecated.</b> Please use the 'description' property instead. Gets and sets the description of the power query formula. |
| [getPowerQueryFormulaItems()](#getPowerQueryFormulaItems--)| <b>@deprecated.</b> Please use the 'powerQueryFormulaItems' property instead. Gets all items of power query formula. |
| [getType()](#getType--)| Gets the type of power query formula. |
| [getFormulaDefinition()](#getFormulaDefinition--)| Gets the definition of the power query formula. |
### constructor(PowerQueryFormula) {#constructor-powerqueryformula-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: PowerQueryFormula);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PowerQueryFormula | The parent object. |
### f {#f--}
Gets and sets the definition of function.
```javascript
f : string;
```
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
### getF() {#getF--}
```javascript
getF() : string;
```
### setF(string) {#setF-string-}
```javascript
setF(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
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
### getType() {#getType--}
Gets the type of power query formula.
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
