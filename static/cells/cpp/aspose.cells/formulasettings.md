##Aspose::Cells::FormulaSettings class
'Aspose::Cells::FormulaSettings class. Settings of formulas and calculation in C++.'
## FormulaSettings class
[Settings](../../aspose.cells.settings/) of formulas and calculation.
```cpp
class FormulaSettings
```
## Methods
| Method | Description |
| --- | --- |
| [FormulaSettings(FormulaSettings_Impl* impl)](./formulasettings/) | Constructs from an implementation object. |
| [FormulaSettings(const FormulaSettings\& src)](./formulasettings/) | Copy constructor. |
| [GetCalculateOnOpen()](./getcalculateonopen/) | Indicates whether the application is required to perform a full calculation when the workbook is opened. |
| [GetCalculateOnSave()](./getcalculateonsave/) | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. |
| [GetCalculationId()](./getcalculationid/) | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [GetCalculationMode()](./getcalculationmode/) | Gets or sets the mode for workbook calculation in ms excel. |
| [GetEnableCalculationChain()](./getenablecalculationchain/) | Whether enable calculation chain for formulas. Default is false. |
| [GetEnableIterativeCalculation()](./getenableiterativecalculation/) | Indicates whether enable iterative calculation to resolve circular references. |
| [GetForceFullCalculation()](./getforcefullcalculation/) | Indicates whether calculates all formulas every time when a calculation is triggered. |
| [GetMaxChange()](./getmaxchange/) | The maximum change to resolve a circular reference. |
| [GetMaxIteration()](./getmaxiteration/) | The maximum iterations to resolve a circular reference. |
| [GetPrecisionAsDisplayed()](./getprecisionasdisplayed/) | Whether the precision of calculated result be set as they are displayed while calculating formulas. |
| [GetPreservePaddingSpaces()](./getpreservepaddingspaces/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FormulaSettings\& src)](./operator_asm/) | operator= |
| [SetCalculateOnOpen(bool value)](./setcalculateonopen/) | Indicates whether the application is required to perform a full calculation when the workbook is opened. |
| [SetCalculateOnSave(bool value)](./setcalculateonsave/) | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. |
| [SetCalculationId(const U16String\& value)](./setcalculationid/) | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [SetCalculationId(const char16_t* value)](./setcalculationid/) | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [SetCalculationMode(CalcModeType value)](./setcalculationmode/) | Gets or sets the mode for workbook calculation in ms excel. |
| [SetEnableCalculationChain(bool value)](./setenablecalculationchain/) | Whether enable calculation chain for formulas. Default is false. |
| [SetEnableIterativeCalculation(bool value)](./setenableiterativecalculation/) | Indicates whether enable iterative calculation to resolve circular references. |
| [SetForceFullCalculation(bool value)](./setforcefullcalculation/) | Indicates whether calculates all formulas every time when a calculation is triggered. |
| [SetMaxChange(double value)](./setmaxchange/) | The maximum change to resolve a circular reference. |
| [SetMaxIteration(int32_t value)](./setmaxiteration/) | The maximum iterations to resolve a circular reference. |
| [SetPrecisionAsDisplayed(bool value)](./setprecisionasdisplayed/) | Whether the precision of calculated result be set as they are displayed while calculating formulas. |
| [SetPreservePaddingSpaces(bool value)](./setpreservepaddingspaces/) | Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [~FormulaSettings()](./~formulasettings/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
