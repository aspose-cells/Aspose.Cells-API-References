---
title: Area.Formatting
second_title: Aspose.Cells for .NET API Reference
description: Area property. Represents the formatting of the area
type: docs
url: /net/aspose.cells.drawing/area/formatting/
---
## Area.Formatting property

Represents the formatting of the area.

```csharp
public FormattingType Formatting { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(FormattingType.Custom, chartarea.Area.Formatting, "chart.chartarea.Area.Formatting");
private void Property_Formatting(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet3"];
            Chart chart = sheet.Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(FormattingType.Custom, chartarea.Area.Formatting, "chart.chartarea.Area.Formatting");
        }
```

### See Also

* enum [FormattingType](../../../aspose.cells.charts/formattingtype/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


