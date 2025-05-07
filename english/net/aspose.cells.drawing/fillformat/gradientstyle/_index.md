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
// Called: AssertHelper.AreEqual(GradientStyleType.DiagonalUp, chartarea.Area.FillFormat.GradientStyle, "chart.ChartArea.Area.FillFormat.GradientStyle");
private void Property_GradientStyle(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet3"];
            Chart chart = sheet.Charts[0];
            ChartArea chartarea = chart.ChartArea;
            AssertHelper.AreEqual(GradientStyleType.DiagonalUp, chartarea.Area.FillFormat.GradientStyle, "chart.ChartArea.Area.FillFormat.GradientStyle");
        }
```

### See Also

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


