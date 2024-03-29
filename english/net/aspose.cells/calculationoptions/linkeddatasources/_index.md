---
title: CalculationOptions.LinkedDataSources
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Specifies the data sources for external links used in formulas
type: docs
url: /net/aspose.cells/calculationoptions/linkeddatasources/
---
## CalculationOptions.LinkedDataSources property

Specifies the data sources for external links used in formulas.

```csharp
public Workbook[] LinkedDataSources { get; set; }
```

### Remarks

Like [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/).

### See Also

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


