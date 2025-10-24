##PowerQueryFormulaParameter
Represents the parameter of power query formula.
## PowerQueryFormulaParameter class
Represents the parameter of power query formula.
```javascript
class PowerQueryFormulaParameter extends PowerQueryFormula;
```
## Constructors
| Constructor | Description |
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
| [getValue()](#getValue--)| <b>@deprecated.</b> Please use the 'value' property instead. Gets the value of parameter. |
| [setValue(string)](#setValue-string-)| <b>@deprecated.</b> Please use the 'value' property instead. Gets the value of parameter. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getGroupName()](#getGroupName--)| <b>@deprecated.</b> Please use the 'groupName' property instead. Gets the name of group which contains this power query formula. |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the power query formula. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the power query formula. |
| [getDescription()](#getDescription--)| <b>@deprecated.</b> Please use the 'description' property instead. Gets and sets the description of the power query formula. |
| [setDescription(string)](#setDescription-string-)| <b>@deprecated.</b> Please use the 'description' property instead. Gets and sets the description of the power query formula. |
| [getPowerQueryFormulaItems()](#getPowerQueryFormulaItems--)| <b>@deprecated.</b> Please use the 'powerQueryFormulaItems' property instead. Gets all items of power query formula. |
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
### getValue() {#getValue--}
```javascript
getValue() : string;
```
### setValue(string) {#setValue-string-}
```javascript
setValue(value: string) : void;
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
Gets the definition of the parameter.
```javascript
getFormulaDefinition() : string;
```
