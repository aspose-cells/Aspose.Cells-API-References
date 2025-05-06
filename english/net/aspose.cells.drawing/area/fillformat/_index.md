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
// Called: AssertHelper.AreEqual(FillPattern.ZigZag, p.Area.FillFormat.Pattern, &amp;quot;chart.NSeries[6].Area.FillFormat.Pattern&amp;quot;);
private void Property_FillFormat(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet3&quot;];
            Chart chart = sheet.Charts[0];
            //Series aseries = chart.NSeries[6];
            ChartPoint p = chart.NSeries[0].Points[6];
            AssertHelper.AreEqual(FillPattern.ZigZag, p.Area.FillFormat.Pattern, &quot;chart.NSeries[6].Area.FillFormat.Pattern&quot;);
        }
```

### See Also

* class [FillFormat](../../fillformat/)
* class [Area](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


