---
title: Aspose::Cells::FormulaSettings::GetCalculationMode method
linktitle: GetCalculationMode
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::FormulaSettings::GetCalculationMode method. Gets or sets the mode for workbook calculation in MS Excel in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells/formulasettings/getcalculationmode/
---
## FormulaSettings::GetCalculationMode method


Gets or sets the mode for workbook calculation in MS Excel.

```cpp
CalcModeType Aspose::Cells::FormulaSettings::GetCalculationMode()
```

## Remarks


This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: [Workbook.CalculateFormula()](../../workbook/calculateformula/), Worksheet.CalculateFormula(CalculationOptions, bool), Cell.Calculate(CalculationOptions), ...etc. 
## See Also

* Enum [CalcModeType](../../calcmodetype/)
* Class [FormulaSettings](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
