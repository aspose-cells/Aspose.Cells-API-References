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
// Called: copts.CustomEngine = new MyEngineForReferredArea1(wb);
[Test]
        public void Property_CustomEngine()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells[&quot;A1&quot;].Formula = &quot;=MYFUNC(A2:B4)&quot;;
            cells[&quot;A2&quot;].Formula = &quot;=A1&quot;;
            CalculationOptions copts = new CalculationOptions();
            copts.IgnoreError = false;
            copts.CustomEngine = new MyEngineForReferredArea1(wb);
            wb.CalculateFormula(copts);
            Console.WriteLine(&quot;Finished for no calculation for ReferredArea, A2-&quot; + cells[&quot;A2&quot;].Value);
            copts.CustomEngine = new MyEngineForReferredArea2(copts);
            wb.CalculateFormula(copts);
            Console.WriteLine(&quot;Finished for no recursive calculation for ReferredArea, A2-&quot; + cells[&quot;A2&quot;].Value);
            copts.CustomEngine = new MyEngineForReferredArea2(null);
            wb.CalculateFormula(copts);
            Console.WriteLine(&quot;Recursive calculation for ReferredArea, A2-&quot; + cells[&quot;A2&quot;].Value);
            copts.Recursive = false;
            wb.CalculateFormula(copts);
            Console.WriteLine(&quot;Finished for no recursive calculation for all, A2-&quot; + cells[&quot;A2&quot;].Value);
        }
```

### See Also

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


