---
title: FormulaSettings.EnableIterativeCalculation
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Indicates whether enable iterative calculation to resolve circular references
type: docs
url: /net/aspose.cells/formulasettings/enableiterativecalculation/
---
## FormulaSettings.EnableIterativeCalculation property

Indicates whether enable iterative calculation to resolve circular references.

```csharp
public bool EnableIterativeCalculation { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
public void FormulaSettings_Property_EnableIterativeCalculation()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
    workbook.Settings.FormulaSettings.MaxIteration = 100;
    workbook.Worksheets[1].Cells[37, 5].Value = 0.06;
    workbook.CalculateFormula();
    Assert.AreEqual(6069.76062, workbook.Worksheets[1].Cells[32, 5].DoubleValue, 0.01, "25683_1");

    workbook = new Workbook(Constants.sourcePath + "example.xlsm");
    workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
    workbook.Settings.FormulaSettings.MaxIteration = 100;
    workbook.Worksheets[1].Cells[37, 5].Value = 0.06;
    workbook.CalculateFormula();
    Assert.AreEqual(6139.36894, workbook.Worksheets[1].Cells[32, 5].DoubleValue, 0.01, "25683_2");
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


