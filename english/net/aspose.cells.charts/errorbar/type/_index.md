---
title: ErrorBar.Type
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Represents error bar amount type
type: docs
url: /net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Represents error bar amount type.

```csharp
public ErrorBarType Type { get; set; }
```

### Examples

```csharp
[C#]
Workbook wb = new Workbook("chart.xlsx");
Chart chart = wb.Worksheets[0].Charts[0];
Series aseries = chart.NSeries[0];
//Sets custom error bar type
aseries.YErrorBar.Type = ErrorBarType.Custom;
aseries.YErrorBar.PlusValue = "=Sheet1!A1";
aseries.YErrorBar.MinusValue = "=Sheet1!A2";

[Visual Basic]
'Sets custom error bar type
aseries.YErrorBar.Type = ErrorBarType.Custom
aseries.YErrorBar.PlusValue = "=Sheet1!A1"
aseries.YErrorBar.MinusValue = "=Sheet1!A2"
```

### See Also

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


