---
title: Aspose::Cells::FormulaSettings class
linktitle: FormulaSettings
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::FormulaSettings class. Settings of formulas and calculation in C++.'
type: docs
weight: 7500
url: /cpp/aspose.cells/formulasettings/
---
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
| [GetCalculateOnSave()](./getcalculateonsave/) | Indicates whether to recalculate the workbook before saving the document, when in manual calculation mode. |
| [GetCalculationId()](./getcalculationid/) | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [GetCalculationMode()](./getcalculationmode/) | Gets or sets the mode for workbook calculation in MS Excel. |
| [GetEnableCalculationChain()](./getenablecalculationchain/) | Indicates whether to enable calculation chain for formulas. Default is false. |
| [GetEnableIterativeCalculation()](./getenableiterativecalculation/) | Indicates whether to enable iterative calculation to resolve circular references. |
| [GetForceFullCalculation()](./getforcefullcalculation/) | Indicates whether it calculates all formulas every time when a calculation is triggered. |
| [GetMaxChange()](./getmaxchange/) | The maximum change to resolve a circular reference. |
| [GetMaxIteration()](./getmaxiteration/) | The maximum iterations to resolve a circular reference. |
| [GetPrecisionAsDisplayed()](./getprecisionasdisplayed/) | Indicates whether the precision of calculated result be set as they are displayed while calculating formulas. |
| [GetPreservePaddingSpaces()](./getpreservepaddingspaces/) | Indicates whether to preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const FormulaSettings\& src)](./operator_asm/) | operator= |
| [SetCalculateOnOpen(bool value)](./setcalculateonopen/) | Indicates whether the application is required to perform a full calculation when the workbook is opened. |
| [SetCalculateOnSave(bool value)](./setcalculateonsave/) | Indicates whether to recalculate the workbook before saving the document, when in manual calculation mode. |
| [SetCalculationId(const U16String\& value)](./setcalculationid/) | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [SetCalculationId(const char16_t* value)](./setcalculationid/) | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [SetCalculationMode(CalcModeType value)](./setcalculationmode/) | Gets or sets the mode for workbook calculation in MS Excel. |
| [SetEnableCalculationChain(bool value)](./setenablecalculationchain/) | Indicates whether to enable calculation chain for formulas. Default is false. |
| [SetEnableIterativeCalculation(bool value)](./setenableiterativecalculation/) | Indicates whether to enable iterative calculation to resolve circular references. |
| [SetForceFullCalculation(bool value)](./setforcefullcalculation/) | Indicates whether it calculates all formulas every time when a calculation is triggered. |
| [SetMaxChange(double value)](./setmaxchange/) | The maximum change to resolve a circular reference. |
| [SetMaxIteration(int32_t value)](./setmaxiteration/) | The maximum iterations to resolve a circular reference. |
| [SetPrecisionAsDisplayed(bool value)](./setprecisionasdisplayed/) | Indicates whether the precision of calculated result be set as they are displayed while calculating formulas. |
| [SetPreservePaddingSpaces(bool value)](./setpreservepaddingspaces/) | Indicates whether to preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false. |
| [~FormulaSettings()](./~formulasettings/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
