---
title: "FormulaParseOptions Class"
linktitle: "FormulaParseOptions"
articleTitle: "FormulaParseOptions"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents options when parsing formula."
type: docs
weight: 2600
url: /php/aspose.cells/formulaparseoptions/
---

## FormulaParseOptions class

Represents options when parsing formula.

## Constructors

| Name | Description |
| --- | --- |
| [FormulaParseOptions](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [LocaleDependent](#localedependent) | boolean | Whether the formula is locale formatted. Default is false. |
| [R1C1Style](#r1c1style) | boolean | Whether the formula is R1C1 reference style. Default is false. |
| [CheckAddIn](#checkaddin) | boolean | Whether check addins in existing external links of current workbook for user defined function without external link. Def |
| [Parse](#parse) | boolean | Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the ce |
| [CustomFunctionDefinition](#customfunctiondefinition) | CustomFunctionDefinition | Definition for parsing custom functions. For some special requirements, such as when calculating custom function in user |

### FormulaParseOptions() {#constructor}

### FormulaParseOptions.LocaleDependent property {#localedependent}

Whether the formula is locale formatted. Default is false.

**Type:** boolean

### FormulaParseOptions.R1C1Style property {#r1c1style}

Whether the formula is R1C1 reference style. Default is false.

**Type:** boolean

### FormulaParseOptions.CheckAddIn property {#checkaddin}

Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).

**Type:** boolean

### FormulaParseOptions.Parse property {#parse}

Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas.

**Type:** boolean

### FormulaParseOptions.CustomFunctionDefinition property {#customfunctiondefinition}

Definition for parsing custom functions. For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by Workbook.updateCustomFunctionDefinition(com.aspose.cells.CustomFunctionDefinition) to get the same result.

**Type:** CustomFunctionDefinition
