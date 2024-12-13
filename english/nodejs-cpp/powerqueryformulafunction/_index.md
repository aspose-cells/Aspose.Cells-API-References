---
title: PowerQueryFormulaFunction
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the function of power query.
type: docs
url: /nodejs-cpp/powerqueryformulafunction/
---

## PowerQueryFormulaFunction class

Represents the function of power query.

```javascript
class PowerQueryFormulaFunction extends PowerQueryFormula;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(PowerQueryFormula)](#constructor-powerqueryformula-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getType()](#getType--)| Gets the type of power query formula. |
| [getF()](#getF--)| Gets and sets the definition of function. |
| [setF(string)](#setF-string-)| Gets and sets the definition of function. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getGroupName()](#getGroupName--)| Gets the name of group which contains this power query formula. |
| [getName()](#getName--)| Gets and sets the name of the power query formula. |
| [setName(string)](#setName-string-)| Gets and sets the name of the power query formula. |
| [getPowerQueryFormulaItems()](#getPowerQueryFormulaItems--)| Gets all items of power query formula. |
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

### getType() {#getType--}

Gets the type of power query formula.

```javascript
getType() : PowerQueryFormulaType;
```


**Returns**

[PowerQueryFormulaType](../powerqueryformulatype/)

### getF() {#getF--}

Gets and sets the definition of function.

```javascript
getF() : string;
```


### setF(string) {#setF-string-}

Gets and sets the definition of function.

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

### getFormulaDefinition() {#getFormulaDefinition--}

Gets the definition of the power query formula.

```javascript
getFormulaDefinition() : string;
```



