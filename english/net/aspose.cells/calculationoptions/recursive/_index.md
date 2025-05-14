---
title: CalculationOptions.Recursive
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true
type: docs
url: /net/aspose.cells/calculationoptions/recursive/
---
## CalculationOptions.Recursive property

Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value is true.

```csharp
public bool Recursive { get; set; }
```

### Examples

```csharp
// Called: copts.Recursive = false;
public void CalculationOptions_Property_Recursive()
{
    Workbook wb = new Workbook();
    Cells cells = wb.Worksheets[0].Cells;
    cells["A1"].Formula = "=MYFUNC(A2:B4)";
    cells["A2"].Formula = "=A1";
    CalculationOptions copts = new CalculationOptions();
    copts.IgnoreError = false;
    copts.CustomEngine = new MyEngineForReferredArea1(wb);
    wb.CalculateFormula(copts);
    Console.WriteLine("Finished for no calculation for ReferredArea, A2-" + cells["A2"].Value);
    copts.CustomEngine = new MyEngineForReferredArea2(copts);
    wb.CalculateFormula(copts);
    Console.WriteLine("Finished for no recursive calculation for ReferredArea, A2-" + cells["A2"].Value);
    copts.CustomEngine = new MyEngineForReferredArea2(null);
    wb.CalculateFormula(copts);
    Console.WriteLine("Recursive calculation for ReferredArea, A2-" + cells["A2"].Value);
    copts.Recursive = false;
    wb.CalculateFormula(copts);
    Console.WriteLine("Finished for no recursive calculation for all, A2-" + cells["A2"].Value);
}
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


