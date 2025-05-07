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
// Called: workbook.Settings.FormulaSettings.MaxIteration = 100;
[Test]
        public void Property_MaxIteration()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Formula/calculate/CellsNet25683_1.xlsm");
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            workbook.Worksheets[1].Cells[37, 5].Value = 0.06;
            workbook.CalculateFormula();
            Assert.AreEqual(6069.76062, workbook.Worksheets[1].Cells[32, 5].DoubleValue, 0.01, "25683_1");

            workbook = new Workbook(Constants.sourcePath + "Formula/calculate/CellsNet25683_2.xlsm");
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


