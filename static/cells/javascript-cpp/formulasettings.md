##FormulaSettings
Settings of formulas and calculation.
## FormulaSettings class
Settings of formulas and calculation.
```javascript
class FormulaSettings;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [calculateOnOpen](#calculateOnOpen--)| boolean | Indicates whether the application is required to perform a full calculation when the workbook is opened. |
| [calculateOnSave](#calculateOnSave--)| boolean | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. |
| [forceFullCalculation](#forceFullCalculation--)| boolean | Indicates whether calculates all formulas every time when a calculation is triggered. |
| [calculationMode](#calculationMode--)| CalcModeType | Gets or sets the mode for workbook calculation in ms excel. |
| [calculationId](#calculationId--)| string | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [enableIterativeCalculation](#enableIterativeCalculation--)| boolean | Indicates whether enable iterative calculation to resolve circular references. |
| [maxIteration](#maxIteration--)| number | The maximum iterations to resolve a circular reference. |
| [maxChange](#maxChange--)| number | The maximum change to resolve a circular reference. |
| [precisionAsDisplayed](#precisionAsDisplayed--)| boolean | Whether the precision of calculated result be set as they are displayed while calculating formulas |
| [enableCalculationChain](#enableCalculationChain--)| boolean | Whether enable calculation chain for formulas. Default is false. |
| [preservePaddingSpaces](#preservePaddingSpaces--)| boolean | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
### calculateOnOpen {#calculateOnOpen--}
Indicates whether the application is required to perform a full calculation when the workbook is opened.
```javascript
calculateOnOpen : boolean;
```
**Remarks**
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.
### calculateOnSave {#calculateOnSave--}
Indicates whether recalculate the workbook before saving the document, when in manual calculation mode.
```javascript
calculateOnSave : boolean;
```
**Remarks**
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.
### forceFullCalculation {#forceFullCalculation--}
Indicates whether calculates all formulas every time when a calculation is triggered.
```javascript
forceFullCalculation : boolean;
```
**Remarks**
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.
### calculationMode {#calculationMode--}
Gets or sets the mode for workbook calculation in ms excel.
```javascript
calculationMode : CalcModeType;
```
**Remarks**
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: [Workbook.CalculateFormula()](../workbook.calculateformula()/), [Worksheet.CalculateFormula(CalculationOptions, bool)](../worksheet.calculateformula(calculationoptions, bool)/), [Cell.Calculate(CalculationOptions)](../cell.calculate(calculationoptions)/), ...etc.
### calculationId {#calculationId--}
Specifies the version of the calculation engine used to calculate values in the workbook.
```javascript
calculationId : string;
```
**Remarks**
This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.
### enableIterativeCalculation {#enableIterativeCalculation--}
Indicates whether enable iterative calculation to resolve circular references.
```javascript
enableIterativeCalculation : boolean;
```
### maxIteration {#maxIteration--}
The maximum iterations to resolve a circular reference.
```javascript
maxIteration : number;
```
### maxChange {#maxChange--}
The maximum change to resolve a circular reference.
```javascript
maxChange : number;
```
### precisionAsDisplayed {#precisionAsDisplayed--}
Whether the precision of calculated result be set as they are displayed while calculating formulas
```javascript
precisionAsDisplayed : boolean;
```
### enableCalculationChain {#enableCalculationChain--}
Whether enable calculation chain for formulas. Default is false.
```javascript
enableCalculationChain : boolean;
```
**Remarks**
When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.
### preservePaddingSpaces {#preservePaddingSpaces--}
Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.
```javascript
preservePaddingSpaces : boolean;
```
**Remarks**
Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.
