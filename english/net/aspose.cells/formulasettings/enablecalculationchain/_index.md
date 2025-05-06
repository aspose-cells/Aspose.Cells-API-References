---
title: FormulaSettings.EnableCalculationChain
second_title: Aspose.Cells for .NET API Reference
description: FormulaSettings property. Whether enable calculation chain for formulas. Default is false
type: docs
url: /net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Whether enable calculation chain for formulas. Default is false.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Remarks

When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.

### Examples

```csharp
// Called: wb.Settings.FormulaSettings.EnableCalculationChain = true;
[Test]
        public void Property_EnableCalculationChain()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            wb.Settings.FormulaSettings.EnableCalculationChain = true;
            cells[&quot;A1&quot;].Formula = &quot;=SUM(B1:B3)&quot;;
            cells[&quot;B1&quot;].Formula = &quot;=C1*2&quot;;
            cells[&quot;C1&quot;].PutValue(1);
            wb.CalculateFormula();
            AssertHelper.AreEqual(2, cells[&quot;A1&quot;].IntValue, &quot;A1&apos;s value&quot;);
            cells[&quot;C1&quot;].PutValue(2);
            wb.CalculateFormula();
            AssertHelper.AreEqual(4, cells[&quot;B1&quot;].IntValue, &quot;B1&apos;s value&quot;);
            AssertHelper.AreEqual(4, cells[&quot;A1&quot;].IntValue, &quot;A1&apos;s value after C1 being changed&quot;);
        }
```

### See Also

* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


