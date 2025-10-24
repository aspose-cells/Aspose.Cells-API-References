##CalculationOptions
Represents options for calculation.
## CalculationOptions class
Represents options for calculation.
```javascript
class CalculationOptions;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [ignoreError](#ignoreError--)| boolean | Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true. |
| [recursive](#recursive--)| boolean | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true. |
| [userSpecifiedRefreshDynamicArrayFormula](#userSpecifiedRefreshDynamicArrayFormula--)| boolean | Readonly. Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas. |
| [refreshDynamicArrayFormula](#refreshDynamicArrayFormula--)| boolean | Indicates whether dynamic array formulas should be refreshed before calculating formulas. |
| [customEngine](#customEngine--)| AbstractCalculationEngine | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [calcStackSize](#calcStackSize--)| number | The stack size for calculating cells recursively. Default value is 200. |
| [precisionStrategy](#precisionStrategy--)| CalculationPrecisionStrategy | Specifies the strategy for processing precision of calculation. |
| [linkedDataSources](#linkedDataSources--)| Workbook[] | Specifies the data sources for external links used in formulas. |
| [characterEncoding](#characterEncoding--)| EncodingType | Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### ignoreError {#ignoreError--}
Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.
```javascript
ignoreError : boolean;
```
### recursive {#recursive--}
Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.
```javascript
recursive : boolean;
```
### userSpecifiedRefreshDynamicArrayFormula {#userSpecifiedRefreshDynamicArrayFormula--}
Readonly. Indicates whether user has explicitly specified the behavior of refreshing dynamic array formulas before calculating specified formulas.
```javascript
userSpecifiedRefreshDynamicArrayFormula : boolean;
```
### refreshDynamicArrayFormula {#refreshDynamicArrayFormula--}
Indicates whether dynamic array formulas should be refreshed before calculating formulas.
```javascript
refreshDynamicArrayFormula : boolean;
```
**Remarks**
If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([UserSpecifiedRefreshDynamicArrayFormula](../userspecifiedrefreshdynamicarrayformula/) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [Workbook.CalculateFormula(CalculationOptions)](../workbook.calculateformula(calculationoptions)/), this property will be taken as true. For other cases, such as [Cell.Calculate(CalculationOptions)](../cell.calculate(calculationoptions)/) or [Worksheet.CalculateFormula(CalculationOptions, bool)](../worksheet.calculateformula(calculationoptions, bool)/), this property will be taken as false.
### customEngine {#customEngine--}
The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.
```javascript
customEngine : AbstractCalculationEngine;
```
### calcStackSize {#calcStackSize--}
The stack size for calculating cells recursively. Default value is 200.
```javascript
calcStackSize : number;
```
**Remarks**
When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.
### precisionStrategy {#precisionStrategy--}
Specifies the strategy for processing precision of calculation.
```javascript
precisionStrategy : CalculationPrecisionStrategy;
```
### linkedDataSources {#linkedDataSources--}
Specifies the data sources for external links used in formulas.
```javascript
linkedDataSources : Workbook[];
```
**Remarks**
Like [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.UpdateLinkedDataSource(Workbook[])](../workbook.updatelinkeddatasource(workbook[])/). The match of those workbooks with external links is determined by [Workbook.FileName](../workbook.filename/) and [ExternalLink.DataSource](../externallink.datasource/). So please make sure [Workbook.FileName](../workbook.filename/) has been specified with the proper value(generally it should be same with corresponding [ExternalLink.DataSource](../externallink.datasource/)) for every workbook so they can be linked as expected.
### characterEncoding {#characterEncoding--}
Specifies the encoding used for encoding/decoding characters when calculating formulas. For functions such as CHAR, CODE, the calculated result depends on the region settings and default charset of the environment. With this property user can specify the proper encoding used for those function to get the expected result.
```javascript
characterEncoding : EncodingType;
```
