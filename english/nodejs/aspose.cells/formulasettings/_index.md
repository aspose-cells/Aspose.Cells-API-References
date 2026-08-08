---
title: "FormulaSettings"
linktitle: "FormulaSettings"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Settings of formulas and calculation."
type: docs
weight: 1630
url: /nodejs/aspose.cells/formulasettings/
---

## FormulaSettings class

Settings of formulas and calculation.

## Methods

| Name | Description |
| --- | --- |
| [getCalculateOnOpen()](#getcalculateonopen) | Indicates whether the application is required to perform a full calculation when the workbook is opened. This property i |
| [getCalculateOnSave()](#getcalculateonsave) | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. This property is |
| [getCalculationId()](#getcalculationid) | Specifies the version of the calculation engine used to calculate values in the workbook. This property is only for savi |
| [getCalculationMode()](#getcalculationmode) | Gets or sets the mode for workbook calculation in ms excel. The value of the property is CalcModeType integer constant.  |
| [getEnableCalculationChain()](#getenablecalculationchain) | Whether enable calculation chain for formulas. Default is false. When there are lots of formulas in the workbook and use |
| [getEnableIterativeCalculation()](#getenableiterativecalculation) | Indicates whether enable iterative calculation to resolve circular references. |
| [getForceFullCalculation()](#getforcefullcalculation) | Indicates whether calculates all formulas every time when a calculation is triggered. This property is only for saving t |
| [getMaxChange()](#getmaxchange) | The maximum change to resolve a circular reference. |
| [getMaxIteration()](#getmaxiteration) | The maximum iterations to resolve a circular reference. |
| [getPrecisionAsDisplayed()](#getprecisionasdisplayed) | Whether the precision of calculated result be set as they are displayed while calculating formulas |
| [getPreservePaddingSpaces()](#getpreservepaddingspaces) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |
| [setCalculateOnOpen()](#setcalculateonopen) | Indicates whether the application is required to perform a full calculation when the workbook is opened. This property i |
| [setCalculateOnSave()](#setcalculateonsave) | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. This property is |
| [setCalculationId()](#setcalculationid) | Specifies the version of the calculation engine used to calculate values in the workbook. This property is only for savi |
| [setCalculationMode()](#setcalculationmode) | Gets or sets the mode for workbook calculation in ms excel. The value of the property is CalcModeType integer constant.  |
| [setEnableCalculationChain()](#setenablecalculationchain) | Whether enable calculation chain for formulas. Default is false. When there are lots of formulas in the workbook and use |
| [setEnableIterativeCalculation()](#setenableiterativecalculation) | Indicates whether enable iterative calculation to resolve circular references. |
| [setForceFullCalculation()](#setforcefullcalculation) | Indicates whether calculates all formulas every time when a calculation is triggered. This property is only for saving t |
| [setMaxChange()](#setmaxchange) | The maximum change to resolve a circular reference. |
| [setMaxIteration()](#setmaxiteration) | The maximum iterations to resolve a circular reference. |
| [setPrecisionAsDisplayed()](#setprecisionasdisplayed) | Whether the precision of calculated result be set as they are displayed while calculating formulas |
| [setPreservePaddingSpaces()](#setpreservepaddingspaces) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |

### getCalculateOnOpen() {#getcalculateonopen}

Indicates whether the application is required to perform a full calculation when the workbook is opened. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### getCalculateOnSave() {#getcalculateonsave}

Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### getCalculationId() {#getcalculationid}

Specifies the version of the calculation engine used to calculate values in the workbook. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.

### getCalculationMode() {#getcalculationmode}

Gets or sets the mode for workbook calculation in ms excel. The value of the property is CalcModeType integer constant. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: Workbook.calculateFormula(), Worksheet.calculateFormula(com.aspose.cells.CalculationOptions, boolean), Cell.calculate(com.aspose.cells.CalculationOptions), ...etc.

### getEnableCalculationChain() {#getenablecalculationchain}

Whether enable calculation chain for formulas. Default is false. When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.

### getEnableIterativeCalculation() {#getenableiterativecalculation}

Indicates whether enable iterative calculation to resolve circular references.

### getForceFullCalculation() {#getforcefullcalculation}

Indicates whether calculates all formulas every time when a calculation is triggered. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### getMaxChange() {#getmaxchange}

The maximum change to resolve a circular reference.

### getMaxIteration() {#getmaxiteration}

The maximum iterations to resolve a circular reference.

### getPrecisionAsDisplayed() {#getprecisionasdisplayed}

Whether the precision of calculated result be set as they are displayed while calculating formulas

### getPreservePaddingSpaces() {#getpreservepaddingspaces}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.

### setCalculateOnOpen() {#setcalculateonopen}

Indicates whether the application is required to perform a full calculation when the workbook is opened. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### setCalculateOnSave() {#setcalculateonsave}

Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### setCalculationId() {#setcalculationid}

Specifies the version of the calculation engine used to calculate values in the workbook. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.

### setCalculationMode() {#setcalculationmode}

Gets or sets the mode for workbook calculation in ms excel. The value of the property is CalcModeType integer constant. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: Workbook.calculateFormula(), Worksheet.calculateFormula(com.aspose.cells.CalculationOptions, boolean), Cell.calculate(com.aspose.cells.CalculationOptions), ...etc.

### setEnableCalculationChain() {#setenablecalculationchain}

Whether enable calculation chain for formulas. Default is false. When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.

### setEnableIterativeCalculation() {#setenableiterativecalculation}

Indicates whether enable iterative calculation to resolve circular references.

### setForceFullCalculation() {#setforcefullcalculation}

Indicates whether calculates all formulas every time when a calculation is triggered. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

### setMaxChange() {#setmaxchange}

The maximum change to resolve a circular reference.

### setMaxIteration() {#setmaxiteration}

The maximum iterations to resolve a circular reference.

### setPrecisionAsDisplayed() {#setprecisionasdisplayed}

Whether the precision of calculated result be set as they are displayed while calculating formulas

### setPreservePaddingSpaces() {#setpreservepaddingspaces}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.
