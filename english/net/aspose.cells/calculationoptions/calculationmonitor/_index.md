---
title: CalculationOptions.CalculationMonitor
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. The monitor for user to track the progress of formula calculation
type: docs
url: /net/aspose.cells/calculationoptions/calculationmonitor/
---
## CalculationOptions.CalculationMonitor property

The monitor for user to track the progress of formula calculation.

```csharp
public AbstractCalculationMonitor CalculationMonitor { get; set; }
```

### Examples

```csharp
// Called: wb.CalculateFormula(new CalculationOptions() { CalculationMonitor = new CalcMonitor50512() });
[Test]
        public void Property_CalculationMonitor()
        {
            Workbook wb = new Workbook();
            wb.Settings.FormulaSettings.EnableCalculationChain = true;
            Cells cells = wb.Worksheets[0].Cells;
            cells[0, 0].PutValue(1);
            cells[0, 1].PutValue(2);
            cells[0, 2].PutValue(4);
            cells[1, 0].Formula = &quot;=SUM(testname)&quot;;
            cells[1, 1].Formula = &quot;=SUM(B1:C1)&quot;;
            cells[1, 2].Formula = &quot;=A2&quot;;
            wb.CalculateFormula();
            Assert.AreEqual(&quot;#NAME?&quot;, cells[1, 0].Value, &quot;A2-First calc without defined name&quot;);
            Assert.AreEqual(6, cells[1, 1].Value, &quot;B2-First calc without defined name&quot;);
            CheckDependentsInCalculation(&quot;Without defined name-&quot;, cells[0, 0], true, null);
            CheckDependentsInCalculation(&quot;Without defined name-&quot;, cells[0, 1], true, new string[] { &quot;Sheet1!B2&quot; });
            Aspose.Cells.Range r = cells.CreateRange(&quot;A1:B1&quot;);
            r.Name = &quot;testname&quot;;
            wb.CalculateFormula(new CalculationOptions() { CalculationMonitor = new CalcMonitor50512() });
            Assert.AreEqual(3, cells[1, 0].Value, &quot;A2-Recalc with defined name&quot;);
            Assert.AreEqual(3, cells[1, 2].Value, &quot;C2-Recalc with defined name&quot;);
            CheckDependentsInCalculation(&quot;With defined name-&quot;, cells[0, 0], true, new string[] { &quot;Sheet1!A2&quot;, &quot;Sheet1!C2&quot; });
            CheckDependentsInCalculation(&quot;With defined name-&quot;, cells[0, 1], true, new string[] { &quot;Sheet1!A2&quot;, &quot;Sheet1!B2&quot;, &quot;Sheet1!C2&quot; });
            cells[0, 1].PutValue(8);
            wb.CalculateFormula();
            Assert.AreEqual(9, cells[1, 0].Value, &quot;A2-Recalc with B1 changed&quot;);
            Assert.AreEqual(12, cells[1, 1].Value, &quot;B2-Recalc with B1 changed&quot;);
            Assert.AreEqual(9, cells[1, 2].Value, &quot;C2-Recalc with B1 changed&quot;);
            Name n = wb.Worksheets.Names[&quot;testname&quot;];
            n.RefersTo = &quot;Sheet1!$B$1:$C$1&quot;;
            wb.CalculateFormula(new CalculationOptions() { CalculationMonitor = new CalcMonitor50512() });
            Assert.AreEqual(12, cells[1, 0].Value, &quot;Recalc with defined name changed&quot;);
            CheckDependentsInCalculation(&quot;With updated name-&quot;, cells[0, 0], true, null);
            CheckDependentsInCalculation(&quot;With updated name-&quot;, cells[0, 1], true, new string[] { &quot;Sheet1!A2&quot;, &quot;Sheet1!B2&quot;, &quot;Sheet1!C2&quot; });
            CheckDependentsInCalculation(&quot;With updated name-&quot;, cells[0, 2], true, new string[] { &quot;Sheet1!A2&quot;, &quot;Sheet1!B2&quot;, &quot;Sheet1!C2&quot; });
        }
```

### See Also

* class [AbstractCalculationMonitor](../../abstractcalculationmonitor/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


