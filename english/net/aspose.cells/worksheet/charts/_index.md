---
title: Worksheet.Charts
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets a Chart collection
type: docs
url: /net/aspose.cells/worksheet/charts/
---
## Worksheet.Charts property

Gets a [`Chart`](../../../aspose.cells.charts/chart/) collection

```csharp
public ChartCollection Charts { get; }
```

### Examples

```csharp
// Called: Chart chart = sheet.Charts[0];
private void Worksheet_Property_Charts(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            Series aseries = chart.NSeries[0];
            AssertHelper.AreEqual(FillPattern.Gray75, aseries.Area.FillFormat.Pattern, "chart.NSeries[0].Area.FillFormat.Pattern");
        }
```

### See Also

* class [ChartCollection](../../../aspose.cells.charts/chartcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


