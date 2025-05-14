---
title: FormulaSettings.MaxChange
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. The maximum change to resolve a circular reference
type: docs
url: /net/aspose.cells/formulasettings/maxchange/
---
## FormulaSettings.MaxChange property

The maximum change to resolve a circular reference.

```csharp
public double MaxChange { get; set; }
```

### Examples

```csharp
// Called: if (!FormulaCaseUtil.VerifyCalc(wb, wb1, "", wb.Settings.FormulaSettings.MaxChange, int.MaxValue))
public void FormulaSettings_Property_MaxChange()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    wb.RefreshDynamicArrayFormulas(true, new CalculationOptions());
    wb.CalculateFormula();
    Workbook wb1 = new Workbook();
    wb1.Copy(wb);
    wb.CalculateFormula();
    if (!FormulaCaseUtil.VerifyCalc(wb, wb1, "", wb.Settings.FormulaSettings.MaxChange, int.MaxValue))
    {
        Assert.Fail("Circular references should be finished in first calculation without change any more");
    }
}
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


