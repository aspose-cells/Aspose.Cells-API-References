---
title: FormulaSettings.CalculationMode
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Gets or sets the mode for workbook calculation in ms excel
type: docs
url: /net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

Gets or sets the mode for workbook calculation in ms excel.

```csharp
public CalcModeType CalculationMode { get; set; }
```

### Remarks

This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: [`CalculateFormula`](../../workbook/calculateformula/), [`CalculateFormula`](../../worksheet/calculateformula/), [`Calculate`](../../cell/calculate/), ...etc.

### Examples

```csharp
// Called: workbook.Settings.FormulaSettings.CalculationMode, "workbook.Settings.CalcMode");
private void Property_CalculationMode(Workbook workbook)
        {
            AssertHelper.AreEqual(CalcModeType.Manual,
                workbook.Settings.FormulaSettings.CalculationMode, "workbook.Settings.CalcMode");
        }
```

### See Also

* enum [CalcModeType](../../calcmodetype/)
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


