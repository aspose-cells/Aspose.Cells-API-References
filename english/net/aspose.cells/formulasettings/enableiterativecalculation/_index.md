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
// Called: wb.Settings.FormulaSettings.EnableIterativeCalculation = true;
[Test]
        public void Property_EnableIterativeCalculation()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[&quot;A1&quot;].SetFormula(&quot;=B1&quot;, 0);
            cells[&quot;C1&quot;].SetFormula(&quot;=E1+D1&quot;, 0);
            cells[&quot;D1&quot;].SetFormula(&quot;=A1&quot;, 0);
            cells[&quot;E1&quot;].SetFormula(&quot;=A1&quot;, 0);
            cells[&quot;F1&quot;].SetFormula(&quot;=G1&quot;, 0);
            cells[&quot;G1&quot;].SetFormula(&quot;=B1&quot;, 0);
            cells[&quot;B1&quot;].SetFormula(&quot;=C1+D1+F1+1&quot;, 1);
            wb.Settings.FormulaSettings.EnableIterativeCalculation = true;
            wb.Settings.FormulaSettings.MaxIteration = 1;
            CalculationOptions opts = new CalculationOptions();
            wb.CalculateFormula(opts);
            //1,1,0,1,1,0,1
            Assert.AreEqual(1, cells[&quot;A1&quot;].IntValue, &quot;1-A1&quot;);
            Assert.AreEqual(1, cells[&quot;B1&quot;].IntValue, &quot;1-B1&quot;);
            Assert.AreEqual(0, cells[&quot;C1&quot;].IntValue, &quot;1-C1&quot;);
            Assert.AreEqual(1, cells[&quot;D1&quot;].IntValue, &quot;1-D1&quot;);
            Assert.AreEqual(1, cells[&quot;E1&quot;].IntValue, &quot;1-E1&quot;);
            Assert.AreEqual(0, cells[&quot;F1&quot;].IntValue, &quot;1-F1&quot;);
            Assert.AreEqual(1, cells[&quot;G1&quot;].IntValue, &quot;1-G1&quot;);
            wb.CalculateFormula(opts);
            //1,2,2,1,1,1,2
            Assert.AreEqual(1, cells[&quot;A1&quot;].IntValue, &quot;2-A1&quot;);
            Assert.AreEqual(2, cells[&quot;B1&quot;].IntValue, &quot;2-B1&quot;);
            Assert.AreEqual(2, cells[&quot;C1&quot;].IntValue, &quot;2-C1&quot;);
            Assert.AreEqual(1, cells[&quot;D1&quot;].IntValue, &quot;2-D1&quot;);
            Assert.AreEqual(1, cells[&quot;E1&quot;].IntValue, &quot;2-E1&quot;);
            Assert.AreEqual(1, cells[&quot;F1&quot;].IntValue, &quot;2-F1&quot;);
            Assert.AreEqual(2, cells[&quot;G1&quot;].IntValue, &quot;2-G1&quot;);
            wb.CalculateFormula(opts);
            //2,5,2,2,2,2,5
            Assert.AreEqual(2, cells[&quot;A1&quot;].IntValue, &quot;3-A1&quot;);
            Assert.AreEqual(5, cells[&quot;B1&quot;].IntValue, &quot;3-B1&quot;);
            Assert.AreEqual(2, cells[&quot;C1&quot;].IntValue, &quot;3-C1&quot;);
            Assert.AreEqual(2, cells[&quot;D1&quot;].IntValue, &quot;3-D1&quot;);
            Assert.AreEqual(2, cells[&quot;E1&quot;].IntValue, &quot;3-E1&quot;);
            Assert.AreEqual(2, cells[&quot;F1&quot;].IntValue, &quot;3-F1&quot;);
            Assert.AreEqual(5, cells[&quot;G1&quot;].IntValue, &quot;3-G1&quot;);
            //5,7,4,5,5,5,7
            //7,15,10,7,7,7,15
            //15,25,14,15,15,15,25
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


