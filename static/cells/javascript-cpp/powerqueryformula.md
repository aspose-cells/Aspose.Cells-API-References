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
