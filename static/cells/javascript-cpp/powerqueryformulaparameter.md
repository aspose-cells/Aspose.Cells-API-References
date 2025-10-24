##PowerQueryFormulaParameter
Represents the parameter of power query formula.
## PowerQueryFormulaParameter class
Represents the parameter of power query formula.
```javascript
class PowerQueryFormulaParameter extends PowerQueryFormula;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(PowerQueryFormula)](#constructor-powerqueryformula-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [value](#value--)| string | Gets the value of parameter. |
| [groupName](#groupName--)| string | Readonly. Gets the name of group which contains this power query formula. |
| [name](#name--)| string | Gets and sets the name of the power query formula. |
| [description](#description--)| string | Gets and sets the description of the power query formula. |
| [powerQueryFormulaItems](#powerQueryFormulaItems--)| PowerQueryFormulaItemCollection | Readonly. Gets all items of power query formula. |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of power query formula. |
| [getFormulaDefinition()](#getFormulaDefinition--)| Gets the definition of the parameter. |
### constructor(PowerQueryFormula) {#constructor-powerqueryformula-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: PowerQueryFormula);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PowerQueryFormula | The parent object. |
### value {#value--}
Gets the value of parameter.
```javascript
value : string;
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
Gets the definition of the parameter.
```javascript
getFormulaDefinition() : string;
```
