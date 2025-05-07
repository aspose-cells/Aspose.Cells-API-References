---
title: ErrorBar.DisplayType
second_title: Aspose.Cells for .NET API Reference
description: ErrorBar property. Represents the display type of error bar
type: docs
url: /net/aspose.cells.charts/errorbar/displaytype/
---
## ErrorBar.DisplayType property

Represents the display type of error bar.

```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(ErrorBarDisplayType.Plus, errorbar.DisplayType, "chart.NSeries[0].YErrorBar.DisplayType");
private void Property_DisplayType(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0  ];
            Chart chart = sheet.Charts[0];
            ErrorBar errorbar = chart.NSeries[0].YErrorBar;
            AssertHelper.AreEqual(ErrorBarDisplayType.Plus, errorbar.DisplayType, "chart.NSeries[0].YErrorBar.DisplayType");
        }
```

### See Also

* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


