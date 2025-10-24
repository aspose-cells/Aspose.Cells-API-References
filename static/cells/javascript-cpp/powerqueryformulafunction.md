##PowerQueryFormulaFunction
Represents the function of power query.
## PowerQueryFormulaFunction class
Represents the function of power query.
```javascript
class PowerQueryFormulaFunction extends PowerQueryFormula;
```
## Constructors
| Name | Description |
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
