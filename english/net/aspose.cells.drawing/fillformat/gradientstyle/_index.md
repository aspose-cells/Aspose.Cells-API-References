---
title: FillFormat.GradientStyle
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Returns the gradient style for the specified fill
type: docs
url: /net/aspose.cells.drawing/fillformat/gradientstyle/
---
## FillFormat.GradientStyle property

Returns the gradient style for the specified fill.

```csharp
public GradientStyleType GradientStyle { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(GradientStyleType.Vertical, chartarea.Area.FillFormat.GradientStyle, "chart.ChartArea.Area.FillFormat.GradientStyle");
private void FillFormat_Property_GradientStyle(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet2"];
            Chart chart = sheet.Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(GradientStyleType.Vertical, chartarea.Area.FillFormat.GradientStyle, "chart.ChartArea.Area.FillFormat.GradientStyle");
        }
```

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


