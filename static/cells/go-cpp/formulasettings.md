##FormulaSettings Class
'FormulaSettings class. Encapsulates the object that represents formulasettings in Go.'
## FormulaSettings class
Settings of formulas and calculation.
```go
type FormulaSettings struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetCalculateOnOpen](./getcalculateonopen/) | Indicates whether the application is required to perform a full calculation when the workbook is opened. |
|[SetCalculateOnOpen](./setcalculateonopen/) | Indicates whether the application is required to perform a full calculation when the workbook is opened. |
|[GetCalculateOnSave](./getcalculateonsave/) | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. |
|[SetCalculateOnSave](./setcalculateonsave/) | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. |
|[GetForceFullCalculation](./getforcefullcalculation/) | Indicates whether calculates all formulas every time when a calculation is triggered. |
|[SetForceFullCalculation](./setforcefullcalculation/) | Indicates whether calculates all formulas every time when a calculation is triggered. |
|[GetCalculationMode](./getcalculationmode/) | Gets or sets the mode for workbook calculation in ms excel. |
|[SetCalculationMode](./setcalculationmode/) | Gets or sets the mode for workbook calculation in ms excel. |
|[GetCalculationId](./getcalculationid/) | Specifies the version of the calculation engine used to calculate values in the workbook. |
|[SetCalculationId](./setcalculationid/) | Specifies the version of the calculation engine used to calculate values in the workbook. |
|[GetEnableIterativeCalculation](./getenableiterativecalculation/) | Indicates whether enable iterative calculation to resolve circular references. |
|[SetEnableIterativeCalculation](./setenableiterativecalculation/) | Indicates whether enable iterative calculation to resolve circular references. |
|[GetMaxIteration](./getmaxiteration/) | The maximum iterations to resolve a circular reference. |
|[SetMaxIteration](./setmaxiteration/) | The maximum iterations to resolve a circular reference. |
|[GetMaxChange](./getmaxchange/) | The maximum change to resolve a circular reference. |
|[SetMaxChange](./setmaxchange/) | The maximum change to resolve a circular reference. |
|[GetPrecisionAsDisplayed](./getprecisionasdisplayed/) | Whether the precision of calculated result be set as they are displayed while calculating formulas |
|[SetPrecisionAsDisplayed](./setprecisionasdisplayed/) | Whether the precision of calculated result be set as they are displayed while calculating formulas |
|[GetEnableCalculationChain](./getenablecalculationchain/) | Whether enable calculation chain for formulas. Default is false. |
|[SetEnableCalculationChain](./setenablecalculationchain/) | Whether enable calculation chain for formulas. Default is false. |
|[GetPreservePaddingSpaces](./getpreservepaddingspaces/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokenswhile getting and setting formulas.Default value is false. |
|[SetPreservePaddingSpaces](./setpreservepaddingspaces/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokenswhile getting and setting formulas.Default value is false. |
