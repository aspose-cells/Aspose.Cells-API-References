---
title: Marker.Area
second_title: Aspose.Cells for .NET API Reference
description: Marker property. Gets the area
type: docs
url: /net/aspose.cells.charts/marker/area/
---
## Marker.Area property

Gets the `area`.

```csharp
public Area Area { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].Marker.Area.ForegroundColor.ToArgb() & 0xFFFFFF, 0xFF0000);
public void Marker_Property_Area()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.NSeries[0].Marker.Area.ForegroundColor = Color.Red;
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual(chart.NSeries[0].Marker.Area.ForegroundColor.ToArgb() & 0xFFFFFF, 0xFF0000);
}
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


