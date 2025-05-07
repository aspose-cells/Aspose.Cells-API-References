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
// Called: AssertHelper.AreEqual(FillPattern.DarkVertical, aseries.Area.FillFormat.Pattern, "chart.NSeries[0].Area.FillFormat.Pattern");
private void Property_Pattern(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            Series aseries = chart.NSeries[0];
            AssertHelper.AreEqual(FillPattern.DarkVertical, aseries.Area.FillFormat.Pattern, "chart.NSeries[0].Area.FillFormat.Pattern");
        }
```

### See Also

* enum [FillPattern](../../fillpattern/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


