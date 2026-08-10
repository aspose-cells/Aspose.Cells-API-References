---
title: "FormulaParseOptions"
linktitle: "FormulaParseOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents options when parsing formula."
type: docs
weight: 1620
url: /nodejs/aspose.cells/formulaparseoptions/
---

## FormulaParseOptions class

Represents options when parsing formula.

```js
new FormulaParseOptions()
```

## Methods

| Name | Description |
| --- | --- |
| [getCheckAddIn()](#getcheckaddin) | Whether check addins in existing external links of current workbook for user defined function without external link. Def |
| [getCustomFunctionDefinition()](#getcustomfunctiondefinition) | Definition for parsing custom functions. For some special requirements, such as when calculating custom function in user |
| [getLocaleDependent()](#getlocaledependent) | Whether the formula is locale formatted. Default is false. |
| [getParse()](#getparse) | Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the ce |
| [getR1C1Style()](#getr1c1style) | Whether the formula is R1C1 reference style. Default is false. |
| [setCheckAddIn()](#setcheckaddin) | Whether check addins in existing external links of current workbook for user defined function without external link. Def |
| [setCustomFunctionDefinition()](#setcustomfunctiondefinition) | Definition for parsing custom functions. For some special requirements, such as when calculating custom function in user |
| [setLocaleDependent()](#setlocaledependent) | Whether the formula is locale formatted. Default is false. |
| [setParse()](#setparse) | Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the ce |
| [setR1C1Style()](#setr1c1style) | Whether the formula is R1C1 reference style. Default is false. |

### getCheckAddIn() {#getcheckaddin}

Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).

### getCustomFunctionDefinition() {#getcustomfunctiondefinition}

Definition for parsing custom functions. For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by Workbook.updateCustomFunctionDefinition(com.aspose.cells.CustomFunctionDefinition) to get the same result.

### getLocaleDependent() {#getlocaledependent}

Whether the formula is locale formatted. Default is false.

### getParse() {#getparse}

Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas.

### getR1C1Style() {#getr1c1style}

Whether the formula is R1C1 reference style. Default is false.

### setCheckAddIn() {#setcheckaddin}

Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).

### setCustomFunctionDefinition() {#setcustomfunctiondefinition}

Definition for parsing custom functions. For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by Workbook.updateCustomFunctionDefinition(com.aspose.cells.CustomFunctionDefinition) to get the same result.

### setLocaleDependent() {#setlocaledependent}

Whether the formula is locale formatted. Default is false.

### setParse() {#setparse}

Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas.

### setR1C1Style() {#setr1c1style}

Whether the formula is R1C1 reference style. Default is false.
