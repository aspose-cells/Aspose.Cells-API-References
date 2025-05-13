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
// Called: AssertHelper.AreEqual(FillPattern.DottedGrid, p.Area.FillFormat.Pattern, "chart.NSeries[1].Area.FillFormat.Pattern");
private void FillFormat_Property_Pattern(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet4"];
            Chart chart = sheet.Charts[0];
           // Series aseries = chart.NSeries[1];
            ChartPoint p = chart.NSeries[0].Points[1];
            AssertHelper.AreEqual(FillPattern.DottedGrid, p.Area.FillFormat.Pattern, "chart.NSeries[1].Area.FillFormat.Pattern");
        }
```

### See Also

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


