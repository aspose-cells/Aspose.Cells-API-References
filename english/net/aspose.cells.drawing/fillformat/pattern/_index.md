---
title: FillFormat.Pattern
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Represents an areas display pattern
type: docs
url: /net/aspose.cells.drawing/fillformat/pattern/
---
## FillFormat.Pattern property

Represents an area's display pattern.

```csharp
public FillPattern Pattern { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(FillPattern.DottedDiamond, p.Area.FillFormat.Pattern, &amp;quot;chart.NSeries[2].Area.FillFormat.Pattern&amp;quot;);
private void Property_Pattern(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[&quot;Sheet4&quot;];
            Chart chart = sheet.Charts[0];
         //   Series aseries = chart.NSeries[2];
            ChartPoint p = chart.NSeries[0].Points[2];
            AssertHelper.AreEqual(FillPattern.DottedDiamond, p.Area.FillFormat.Pattern, &quot;chart.NSeries[2].Area.FillFormat.Pattern&quot;);
        }
```

### See Also

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


