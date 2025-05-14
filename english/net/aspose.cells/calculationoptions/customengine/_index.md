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
// Called: copts.CustomEngine = cffh;
public void CalculationOptions_Property_CustomEngine()
{
    Workbook wb = new Workbook();
    Cell cell = wb.Worksheets[0].Cells[0, 0];
    cell.Formula = "=HYPERLINK(\"http://localhost:9090\",\"Target\")";
    CustomEngineForHyperlink cffh = new CustomEngineForHyperlink(true);
    CalculationOptions copts = new CalculationOptions();
    copts.CustomEngine = cffh;
    wb.CalculateFormula(copts);
    if (!cffh.Invoked)
    {
        Assert.Fail("HYPERLINK in custom engine should be called");
    }
    cffh = new CustomEngineForHyperlink(false);
    copts = new CalculationOptions();
    copts.CustomEngine = cffh;
    wb.CalculateFormula(copts);
    if (cffh.Invoked)
    {
        Assert.Fail("HYPERLINK in custom engine should not be called");
    }
}
```

### See Also

* class [AbstractCalculationEngine](../../abstractcalculationengine/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


