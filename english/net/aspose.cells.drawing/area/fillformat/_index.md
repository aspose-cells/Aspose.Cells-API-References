---
title: Area.FillFormat
second_title: Aspose.Cells for .NET API Reference
description: Area property. Represents a FillFormat object that contains fill formatting properties for the specified chart or shape
type: docs
url: /net/aspose.cells.drawing/area/fillformat/
---
## Area.FillFormat property

Represents a `FillFormat` object that contains fill formatting properties for the specified chart or shape.

```csharp
public FillFormat FillFormat { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(FillPattern.DashedHorizontal, p.Area.FillFormat.Pattern, "chart.NSeries[2].Area.FillFormat.Pattern");
private void Area_Property_FillFormat(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet3"];
            Chart chart = sheet.Charts[0];
            //Series aseries = chart.NSeries[2];
            ChartPoint p = chart.NSeries[0].Points[2];
            AssertHelper.AreEqual(FillPattern.DashedHorizontal, p.Area.FillFormat.Pattern, "chart.NSeries[2].Area.FillFormat.Pattern");
        }
```

### See Also

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


