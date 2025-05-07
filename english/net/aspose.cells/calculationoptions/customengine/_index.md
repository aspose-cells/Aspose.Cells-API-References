---
title: CalculationOptions.CustomEngine
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. The custom formula calculation engine to extend the default calculation engine of Aspose.Cells
type: docs
url: /net/aspose.cells/calculationoptions/customengine/
---
## CalculationOptions.CustomEngine property

The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.

```csharp
public AbstractCalculationEngine CustomEngine { get; set; }
```

### Examples

```csharp
// Called: new CalculationOptions() { CustomEngine = new IgnoreCustomFunction() });
[Test]
        public void Property_CustomEngine()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            string fml = "=IGNORECALC()";
            cells[0, 0].SetDynamicArrayFormula(fml, new FormulaParseOptions(),
                new object[][] { new object[] { "val0-0", "val0-1"},
                    new object[] { "val1-0", "val1-1" }, new object[] { "val2-0", "val2-1"}, },
                true, false,
                new CalculationOptions() { CustomEngine = new IgnoreCustomFunction() });
            string[] vals = new string[] { "val0-0", "val0-1", "val1-0", "val1-1", "val2-0", "val2-1", };
            CellArea expected = CellArea.CreateCellArea(0, 0, 2, 1);
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, "IgnoreCustomFunction.Init");
            DynamicFormulaTest.CheckResult(vals, cells, expected, "IgnoreCustomFunction.Init");
            wb.RefreshDynamicArrayFormulas(true,
                new CalculationOptions() { CustomEngine = new IgnoreCustomFunction() });
            DynamicFormulaTest.CheckArrayFormula(fml, cells, expected, "IgnoreCustomFunction.Refresh");
            DynamicFormulaTest.CheckResult(vals, cells, expected, "IgnoreCustomFunction.Refresh");
        }
```

### See Also

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


