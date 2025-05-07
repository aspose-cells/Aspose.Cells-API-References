---
title: Series.Area
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the background area of Series object
type: docs
url: /net/aspose.cells.charts/series/area/
---
## Series.Area property

Represents the background area of Series object.

```csharp
public Area Area { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(TextureType.Sand, aseries.Area.FillFormat.Texture, "chart.NSeries[0].Area.FillFormat.Texture");
private void Property_Area(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets[0];
            Chart chart = sheet.Charts[0];
            Series aseries = chart.NSeries[0];
            AssertHelper.AreEqual(TextureType.Sand, aseries.Area.FillFormat.Texture, "chart.NSeries[0].Area.FillFormat.Texture");
        }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


