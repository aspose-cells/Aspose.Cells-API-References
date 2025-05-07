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
[Test]
        public void Property_EnableIterativeCalculation()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Formula/calculate/CellsNet40396.xlsm");
            workbook.Settings.FormulaSettings.EnableIterativeCalculation = true;
            workbook.Settings.FormulaSettings.MaxIteration = 100;
            var total = workbook.Worksheets[1].Cells["F28"].DoubleValue;
            double perentage = 13.43;
            workbook.Worksheets[1].Cells["F32"].PutValue(perentage / 100);
            workbook.CalculateFormula();
            Assert.AreEqual("56,027", workbook.Worksheets[1].Cells["F28"].StringValue);
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


