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

Like [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [`UpdateLinkedDataSource`](../../workbook/updatelinkeddatasource/). The match of those workbooks with external links is determined by [`FileName`](../../workbook/filename/) and [`DataSource`](../../externallink/datasource/). So please make sure [`FileName`](../../workbook/filename/) has been specified with the proper value(generally it should be same with corresponding [`DataSource`](../../externallink/datasource/)) for every workbook so they can be linked as expected.

### See Also

* class [Workbook](../../workbook/)
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


