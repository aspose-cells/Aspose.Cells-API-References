##FormulaParseOptions
Represents options when parsing formula.
## FormulaParseOptions class
Represents options when parsing formula.
```javascript
class FormulaParseOptions;
```
## Constructors
| Constructor | Description |
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
## Methods
| Method | Description |
| --- | --- |
| [getLocaleDependent()](#getLocaleDependent--)| <b>@deprecated.</b> Please use the 'localeDependent' property instead. Whether the formula is locale formatted. Default is false. |
| [setLocaleDependent(boolean)](#setLocaleDependent-boolean-)| <b>@deprecated.</b> Please use the 'localeDependent' property instead. Whether the formula is locale formatted. Default is false. |
| [getR1C1Style()](#getR1C1Style--)| <b>@deprecated.</b> Please use the 'r1C1Style' property instead. Whether the formula is R1C1 reference style. Default is false. |
| [setR1C1Style(boolean)](#setR1C1Style-boolean-)| <b>@deprecated.</b> Please use the 'r1C1Style' property instead. Whether the formula is R1C1 reference style. Default is false. |
| [getCheckAddIn()](#getCheckAddIn--)| <b>@deprecated.</b> Please use the 'checkAddIn' property instead. Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
| [setCheckAddIn(boolean)](#setCheckAddIn-boolean-)| <b>@deprecated.</b> Please use the 'checkAddIn' property instead. Whether check addins in existing external links of current workbook for user defined function without external link. Default is true(if user defined function matches one addin in existing external links, then take it as the addin). |
| [getParse()](#getParse--)| <b>@deprecated.</b> Please use the 'parse' property instead. Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas. |
| [setParse(boolean)](#setParse-boolean-)| <b>@deprecated.</b> Please use the 'parse' property instead. Whether parse given formula. Default is true. If it is false, then given formula string will be kept as it is for the cell until user call other methods to parse them or parsed formula data is required by other operations such as calculating formulas. |
| [getCustomFunctionDefinition()](#getCustomFunctionDefinition--)| <b>@deprecated.</b> Please use the 'customFunctionDefinition' property instead. Definition for parsing custom functions. |
| [setCustomFunctionDefinition(CustomFunctionDefinition)](#setCustomFunctionDefinition-customfunctiondefinition-)| <b>@deprecated.</b> Please use the 'customFunctionDefinition' property instead. Definition for parsing custom functions. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getLocaleDependent() {#getLocaleDependent--}
```javascript
getLocaleDependent() : boolean;
```
### setLocaleDependent(boolean) {#setLocaleDependent-boolean-}
```javascript
setLocaleDependent(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getR1C1Style() {#getR1C1Style--}
```javascript
getR1C1Style() : boolean;
```
### setR1C1Style(boolean) {#setR1C1Style-boolean-}
```javascript
setR1C1Style(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCheckAddIn() {#getCheckAddIn--}
```javascript
getCheckAddIn() : boolean;
```
### setCheckAddIn(boolean) {#setCheckAddIn-boolean-}
```javascript
setCheckAddIn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getParse() {#getParse--}
```javascript
getParse() : boolean;
```
### setParse(boolean) {#setParse-boolean-}
```javascript
setParse(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getCustomFunctionDefinition() {#getCustomFunctionDefinition--}
```javascript
getCustomFunctionDefinition() : CustomFunctionDefinition;
```
**Returns**
[CustomFunctionDefinition](../customfunctiondefinition/)
**Remarks**
For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by [Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)](../workbook.updatecustomfunctiondefinition(customfunctiondefinition)/) to get the same result.
### setCustomFunctionDefinition(CustomFunctionDefinition) {#setCustomFunctionDefinition-customfunctiondefinition-}
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
