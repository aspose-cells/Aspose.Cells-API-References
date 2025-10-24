##FormulaParseOptions
Represents options when parsing formula.
## FormulaParseOptions class
Represents options when parsing formula.
```javascript
class FormulaParseOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [localeDependent](#localeDependent--)| boolean | Whether the formula is locale formatted. Default is false. |
| [r1C1Style](#r1C1Style--)| boolean | Whether the formula is R1C1 reference style. Default is false. |
| [checkAddIn](#checkAddIn--)| boolean | Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
| [parse](#parse--)| boolean | Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas. |
| [customFunctionDefinition](#customFunctionDefinition--)| CustomFunctionDefinition | Definition for parsing custom functions. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### localeDependent {#localeDependent--}
Whether the formula is locale formatted. Default is false.
```javascript
localeDependent : boolean;
```
### r1C1Style {#r1C1Style--}
Whether the formula is R1C1 reference style. Default is false.
```javascript
r1C1Style : boolean;
```
### checkAddIn {#checkAddIn--}
Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin).
```javascript
checkAddIn : boolean;
```
### parse {#parse--}
Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas.
```javascript
parse : boolean;
```
### customFunctionDefinition {#customFunctionDefinition--}
Definition for parsing custom functions.
```javascript
customFunctionDefinition : CustomFunctionDefinition;
```
**Remarks**
For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by [Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)](../workbook.updatecustomfunctiondefinition(customfunctiondefinition)/) to get the same result.
