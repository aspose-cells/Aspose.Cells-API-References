---
title: FormulaParseOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents options when parsing formula.
type: docs
url: /nodejs-cpp/formulaparseoptions/
---

## FormulaParseOptions class

Represents options when parsing formula.

```javascript
class FormulaParseOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [getLocaleDependent()](#getLocaleDependent--)| Whether the formula is locale formatted. Default is false. |
| [setLocaleDependent(boolean)](#setLocaleDependent-boolean-)| Whether the formula is locale formatted. Default is false. |
| [getR1C1Style()](#getR1C1Style--)| Whether the formula is R1C1 reference style. Default is false. |
| [setR1C1Style(boolean)](#setR1C1Style-boolean-)| Whether the formula is R1C1 reference style. Default is false. |
| [getCheckAddIn()](#getCheckAddIn--)| Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
| [setCheckAddIn(boolean)](#setCheckAddIn-boolean-)| Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
| [getParse()](#getParse--)| Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas. |
| [setParse(boolean)](#setParse-boolean-)| Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas. |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--)| Definition for parsing custom functions. |
| [setCustomFunctionDefinition(CustomFunctionDefinition)](#setCustomFunctionDefinition-customfunctiondefinition-)| Definition for parsing custom functions. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### getLocaleDependent() {#getLocaleDependent--}

Whether the formula is locale formatted. Default is false.

```javascript
getLocaleDependent() : boolean;
```


### setLocaleDependent(boolean) {#setLocaleDependent-boolean-}

Whether the formula is locale formatted. Default is false.

```javascript
setLocaleDependent(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getR1C1Style() {#getR1C1Style--}

Whether the formula is R1C1 reference style. Default is false.

```javascript
getR1C1Style() : boolean;
```


### setR1C1Style(boolean) {#setR1C1Style-boolean-}

Whether the formula is R1C1 reference style. Default is false.

```javascript
setR1C1Style(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCheckAddIn() {#getCheckAddIn--}

Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).

```javascript
getCheckAddIn() : boolean;
```


### setCheckAddIn(boolean) {#setCheckAddIn-boolean-}

Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).

```javascript
setCheckAddIn(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getParse() {#getParse--}

Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas.

```javascript
getParse() : boolean;
```


### setParse(boolean) {#setParse-boolean-}

Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas.

```javascript
setParse(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}

Definition for parsing custom functions.

```javascript
getCustomFunctionDefinition() : CustomFunctionDefinition;
```


**Returns**

[CustomFunctionDefinition](../customfunctiondefinition/)

**Remarks**

For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by [Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)](../workbook.updatecustomfunctiondefinition(customfunctiondefinition)/) to get the same result.

### setCustomFunctionDefinition(CustomFunctionDefinition) {#setCustomFunctionDefinition-customfunctiondefinition-}

Definition for parsing custom functions.

```javascript
setCustomFunctionDefinition(value: CustomFunctionDefinition) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CustomFunctionDefinition](../customfunctiondefinition/) | The value to set. |

**Remarks**

For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by [Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)](../workbook.updatecustomfunctiondefinition(customfunctiondefinition)/) to get the same result.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



