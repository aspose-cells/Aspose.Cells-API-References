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
// Called: if (!FormulaCaseUtil.VerifyCalc(wb, wb1, &amp;quot;&amp;quot;, wb.Settings.FormulaSettings.MaxChange, int.MaxValue))
[Test]
        public void Property_MaxChange()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;Formula/J45780.xlsx&quot;);
            wb.RefreshDynamicArrayFormulas(true, new CalculationOptions());
            wb.CalculateFormula();
            Workbook wb1 = new Workbook();
            wb1.Copy(wb);
            wb.CalculateFormula();
            if (!FormulaCaseUtil.VerifyCalc(wb, wb1, &quot;&quot;, wb.Settings.FormulaSettings.MaxChange, int.MaxValue))
            {
                Assert.Fail(&quot;Circular references should be finished in first calculation without change any more&quot;);
            }
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


