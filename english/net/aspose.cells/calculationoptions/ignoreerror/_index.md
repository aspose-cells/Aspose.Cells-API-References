---
title: CalculationOptions.IgnoreError
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function external links etc. The default value is true
type: docs
url: /net/aspose.cells/calculationoptions/ignoreerror/
---
## CalculationOptions.IgnoreError property

Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.

```csharp
public bool IgnoreError { get; set; }
```

### Examples

```csharp
// Called: new CalculationOptions() { IgnoreError = false }), "Calculate reference to the name");
public void CalculationOptions_Property_IgnoreError()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Name n = wb.Worksheets.Names[0];
    Assert.IsNull(n.GetRange());
    FormulaCaseUtil.AssertInt(0, wb.Worksheets[0].CalculateFormula("=" + n.Text,
        new CalculationOptions() { IgnoreError = false }), "Calculate reference to the name");
}
```

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


