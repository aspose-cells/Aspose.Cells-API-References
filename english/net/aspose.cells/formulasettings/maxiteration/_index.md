---
title: FormulaSettings.MaxIteration
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. The maximum iterations to resolve a circular reference
type: docs
url: /net/aspose.cells/formulasettings/maxiteration/
---
## FormulaSettings.MaxIteration property

The maximum iterations to resolve a circular reference.

```csharp
public int MaxIteration { get; set; }
```

### Examples

```csharp
// Called: workbook.Settings.FormulaSettings.MaxIteration = 10;
public void FormulaSettings_Property_MaxIteration()
{
    Workbook workbook = new Workbook();
    workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
    workbook.Settings.FormulaSettings.MaxIteration = 10;
    Cells cells = workbook.Worksheets[0].Cells;
    Cell cell = cells[2, 0];
    cell.Formula = "=ISERR(A3:A5)";
    workbook.CalculateFormula(false);
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


