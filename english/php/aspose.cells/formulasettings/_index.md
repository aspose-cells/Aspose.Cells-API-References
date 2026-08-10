---
title: "FormulaSettings Class"
linktitle: "FormulaSettings"
articleTitle: "FormulaSettings"
second_title: "Aspose.Cells for PHP via Java"
description: "Settings of formulas and calculation."
type: docs
weight: 2610
url: /php/aspose.cells/formulasettings/
---

## FormulaSettings class

Settings of formulas and calculation.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CalculateOnOpen](#calculateonopen) | boolean | Indicates whether the application is required to perform a full calculation when the workbook is opened. This property i |
| [CalculateOnSave](#calculateonsave) | boolean | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. This property is |
| [ForceFullCalculation](#forcefullcalculation) | boolean | Indicates whether calculates all formulas every time when a calculation is triggered. This property is only for saving t |
| [CalculationMode](#calculationmode) | Number | Gets or sets the mode for workbook calculation in ms excel. The value of the property is CalcModeType integer constant.  |
| [CalculationId](#calculationid) | String | Specifies the version of the calculation engine used to calculate values in the workbook. This property is only for savi |
| [EnableIterativeCalculation](#enableiterativecalculation) | boolean | Indicates whether enable iterative calculation to resolve circular references. |
| [MaxIteration](#maxiteration) | Number | The maximum iterations to resolve a circular reference. |
| [MaxChange](#maxchange) | Number | The maximum change to resolve a circular reference. |
| [PrecisionAsDisplayed](#precisionasdisplayed) | boolean | Whether the precision of calculated result be set as they are displayed while calculating formulas |
| [EnableCalculationChain](#enablecalculationchain) | boolean | Whether enable calculation chain for formulas. Default is false. When there are lots of formulas in the workbook and use |
| [PreservePaddingSpaces](#preservepaddingspaces) | boolean | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting |

### FormulaSettings.CalculateOnOpen property {#calculateonopen}

Indicates whether the application is required to perform a full calculation when the workbook is opened. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

**Type:** boolean

### FormulaSettings.CalculateOnSave property {#calculateonsave}

Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

**Type:** boolean

### FormulaSettings.ForceFullCalculation property {#forcefullcalculation}

Indicates whether calculates all formulas every time when a calculation is triggered. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

**Type:** boolean

### FormulaSettings.CalculationMode property {#calculationmode}

Gets or sets the mode for workbook calculation in ms excel. The value of the property is CalcModeType integer constant. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: Workbook.calculateFormula() , Worksheet.calculateFormula(com.aspose.cells.CalculationOptions, boolean) , Cell.calculate(com.aspose.cells.CalculationOptions) , ...etc.

**Type:** Number

### FormulaSettings.CalculationId property {#calculationid}

Specifies the version of the calculation engine used to calculate values in the workbook. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.

**Type:** String

### FormulaSettings.EnableIterativeCalculation property {#enableiterativecalculation}

Indicates whether enable iterative calculation to resolve circular references.

**Type:** boolean

### FormulaSettings.MaxIteration property {#maxiteration}

The maximum iterations to resolve a circular reference.

**Type:** Number

### FormulaSettings.MaxChange property {#maxchange}

The maximum change to resolve a circular reference.

**Type:** Number

### FormulaSettings.PrecisionAsDisplayed property {#precisionasdisplayed}

Whether the precision of calculated result be set as they are displayed while calculating formulas

**Type:** boolean

### FormulaSettings.EnableCalculationChain property {#enablecalculationchain}

Whether enable calculation chain for formulas. Default is false. When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.

**Type:** boolean

### FormulaSettings.PreservePaddingSpaces property {#preservepaddingspaces}

Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.

**Type:** boolean
