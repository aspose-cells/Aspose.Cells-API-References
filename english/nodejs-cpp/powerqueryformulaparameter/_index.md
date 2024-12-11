---
title: PowerQueryFormulaParameter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the parameter of power query formula.
type: docs
url: /nodejs-cpp/powerqueryformulaparameter/
---

## PowerQueryFormulaParameter class

Represents the parameter of power query formula.

```javascript
class PowerQueryFormulaParameter extends PowerQueryFormula;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(PowerQueryFormula)](#constructor-powerqueryformula-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of power query formula. |
| [getValue()](#getValue--)| Gets the value of parameter. |
| [setValue(string)](#setValue-string-)| Gets the value of parameter. |
| [getFormulaDefinition()](#getFormulaDefinition--)| Gets the definition of the parameter. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getGroupName()](#getGroupName--)| Gets the name of group which contains this power query formula. |
| [getName()](#getName--)| Gets and sets the name of the power query formula. |
| [setName(string)](#setName-string-)| Gets and sets the name of the power query formula. |
| [getPowerQueryFormulaItems()](#getPowerQueryFormulaItems--)| Gets all items of power query formula. |


### constructor(PowerQueryFormula) {#constructor-powerqueryformula-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: PowerQueryFormula);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | PowerQueryFormula | The parent object. |

### getType() {#getType--}

Gets the type of power query formula.

```javascript
getType() : PowerQueryFormulaType;
```


**Returns**

[PowerQueryFormulaType](../powerqueryformulatype/)

### getValue() {#getValue--}

Gets the value of parameter.

```javascript
getValue() : string;
```


### setValue(string) {#setValue-string-}

Gets the value of parameter.

```javascript
setValue(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getFormulaDefinition() {#getFormulaDefinition--}

Gets the definition of the parameter.

```javascript
getFormulaDefinition() : string;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getGroupName() {#getGroupName--}

Gets the name of group which contains this power query formula.

```javascript
getGroupName() : string;
```


### getName() {#getName--}

Gets and sets the name of the power query formula.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets and sets the name of the power query formula.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getPowerQueryFormulaItems() {#getPowerQueryFormulaItems--}

Gets all items of power query formula.

```javascript
getPowerQueryFormulaItems() : PowerQueryFormulaItemCollection;
```


**Returns**

[PowerQueryFormulaItemCollection](../powerqueryformulaitemcollection/)


