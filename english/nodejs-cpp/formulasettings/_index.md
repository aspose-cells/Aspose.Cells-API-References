---
title: FormulaSettings
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Settings of formulas and calculation.
type: docs
url: /nodejs-cpp/formulasettings/
---

## FormulaSettings class

Settings of formulas and calculation.

```javascript
class FormulaSettings;
```


## Methods

| Method | Description |
| --- | --- |
| [getCalculateOnOpen()](#getCalculateOnOpen--)| Indicates whether the application is required to perform a full calculation when the workbook is opened. |
| [setCalculateOnOpen(boolean)](#setCalculateOnOpen-boolean-)| Indicates whether the application is required to perform a full calculation when the workbook is opened. |
| [getCalculateOnSave()](#getCalculateOnSave--)| Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. |
| [setCalculateOnSave(boolean)](#setCalculateOnSave-boolean-)| Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. |
| [getForceFullCalculation()](#getForceFullCalculation--)| Indicates whether calculates all formulas every time when a calculation is triggered. |
| [setForceFullCalculation(boolean)](#setForceFullCalculation-boolean-)| Indicates whether calculates all formulas every time when a calculation is triggered. |
| [getCalculationMode()](#getCalculationMode--)| Gets or sets the mode for workbook calculation in ms excel. |
| [setCalculationMode(CalcModeType)](#setCalculationMode-calcmodetype-)| Gets or sets the mode for workbook calculation in ms excel. |
| [getCalculationId()](#getCalculationId--)| Specifies the version of the calculation engine used to calculate values in the workbook. |
| [setCalculationId(string)](#setCalculationId-string-)| Specifies the version of the calculation engine used to calculate values in the workbook. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--)| Indicates whether enable iterative calculation to resolve circular references. |
| [setEnableIterativeCalculation(boolean)](#setEnableIterativeCalculation-boolean-)| Indicates whether enable iterative calculation to resolve circular references. |
| [getMaxIteration()](#getMaxIteration--)| The maximum iterations to resolve a circular reference. |
| [setMaxIteration(number)](#setMaxIteration-number-)| The maximum iterations to resolve a circular reference. |
| [getMaxChange()](#getMaxChange--)| The maximum change to resolve a circular reference. |
| [setMaxChange(number)](#setMaxChange-number-)| The maximum change to resolve a circular reference. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--)| Whether the precision of calculated result be set as they are displayed while calculating formulas |
| [setPrecisionAsDisplayed(boolean)](#setPrecisionAsDisplayed-boolean-)| Whether the precision of calculated result be set as they are displayed while calculating formulas |
| [getEnableCalculationChain()](#getEnableCalculationChain--)| Whether enable calculation chain for formulas. Default is false. |
| [setEnableCalculationChain(boolean)](#setEnableCalculationChain-boolean-)| Whether enable calculation chain for formulas. Default is false. |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--)| Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [setPreservePaddingSpaces(boolean)](#setPreservePaddingSpaces-boolean-)| Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |


### getCalculateOnOpen() {#getCalculateOnOpen--}

Indicates whether the application is required to perform a full calculation when the workbook is opened.

```javascript
getCalculateOnOpen() : boolean;
```


**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### setCalculateOnOpen(boolean) {#setCalculateOnOpen-boolean-}

Indicates whether the application is required to perform a full calculation when the workbook is opened.

```javascript
setCalculateOnOpen(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### getCalculateOnSave() {#getCalculateOnSave--}

Indicates whether recalculate the workbook before saving the document, when in manual calculation mode.

```javascript
getCalculateOnSave() : boolean;
```


**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### setCalculateOnSave(boolean) {#setCalculateOnSave-boolean-}

Indicates whether recalculate the workbook before saving the document, when in manual calculation mode.

```javascript
setCalculateOnSave(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### getForceFullCalculation() {#getForceFullCalculation--}

Indicates whether calculates all formulas every time when a calculation is triggered.

```javascript
getForceFullCalculation() : boolean;
```


**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### setForceFullCalculation(boolean) {#setForceFullCalculation-boolean-}

Indicates whether calculates all formulas every time when a calculation is triggered.

```javascript
setForceFullCalculation(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### getCalculationMode() {#getCalculationMode--}

Gets or sets the mode for workbook calculation in ms excel.

```javascript
getCalculationMode() : CalcModeType;
```


**Returns**

[CalcModeType](./calcmodetype/)

**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: [Workbook.CalculateFormula()](./workbook.calculateformula()/), [Workbook.CalculateFormula()](./workbook.calculateformula()/), [Cell.Calculate(CalculationOptions)](./cell.calculate(calculationoptions)/), ...etc.

### setCalculationMode(CalcModeType) {#setCalculationMode-calcmodetype-}

Gets or sets the mode for workbook calculation in ms excel.

```javascript
setCalculationMode(value: CalcModeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CalcModeType](./calcmodetype/) | The value to set. |

**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: [Workbook.CalculateFormula()](./workbook.calculateformula()/), [Workbook.CalculateFormula()](./workbook.calculateformula()/), [Cell.Calculate(CalculationOptions)](./cell.calculate(calculationoptions)/), ...etc.

### getCalculationId() {#getCalculationId--}

Specifies the version of the calculation engine used to calculate values in the workbook.

```javascript
getCalculationId() : string;
```


**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.

### setCalculationId(string) {#setCalculationId-string-}

Specifies the version of the calculation engine used to calculate values in the workbook.

```javascript
setCalculationId(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.

### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}

Indicates whether enable iterative calculation to resolve circular references.

```javascript
getEnableIterativeCalculation() : boolean;
```


### setEnableIterativeCalculation(boolean) {#setEnableIterativeCalculation-boolean-}

Indicates whether enable iterative calculation to resolve circular references.

```javascript
setEnableIterativeCalculation(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMaxIteration() {#getMaxIteration--}

The maximum iterations to resolve a circular reference.

```javascript
getMaxIteration() : number;
```


### setMaxIteration(number) {#setMaxIteration-number-}

The maximum iterations to resolve a circular reference.

```javascript
setMaxIteration(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getMaxChange() {#getMaxChange--}

The maximum change to resolve a circular reference.

```javascript
getMaxChange() : number;
```


### setMaxChange(number) {#setMaxChange-number-}

The maximum change to resolve a circular reference.

```javascript
setMaxChange(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}

Whether the precision of calculated result be set as they are displayed while calculating formulas

```javascript
getPrecisionAsDisplayed() : boolean;
```


### setPrecisionAsDisplayed(boolean) {#setPrecisionAsDisplayed-boolean-}

Whether the precision of calculated result be set as they are displayed while calculating formulas

```javascript
setPrecisionAsDisplayed(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getEnableCalculationChain() {#getEnableCalculationChain--}

Whether enable calculation chain for formulas. Default is false.

```javascript
getEnableCalculationChain() : boolean;
```


**Remarks**

When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.

### setEnableCalculationChain(boolean) {#setEnableCalculationChain-boolean-}

Whether enable calculation chain for formulas. Default is false.

```javascript
setEnableCalculationChain(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.

### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

```javascript
getPreservePaddingSpaces() : boolean;
```


**Remarks**

Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.

### setPreservePaddingSpaces(boolean) {#setPreservePaddingSpaces-boolean-}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.

```javascript
setPreservePaddingSpaces(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.


