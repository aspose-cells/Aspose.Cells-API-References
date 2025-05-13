---
title: ChartPoint.Area
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets the  area
type: docs
url: /net/aspose.cells.charts/chartpoint/area/
---
## ChartPoint.Area property

Gets the ` area`.

```csharp
public Area Area { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(TextureType.Granite, p.Area.FillFormat.Texture, "chart.NSeries[3].Area.FillFormat.Texture");
private void ChartPoint_Property_Area(Workbook workbook)
        {
            Worksheet sheet = workbook.Worksheets["Sheet2"];
            Chart chart = sheet.Charts[0];
           // Series aseries = chart.NSeries[3];
            ChartPoint p = chart.NSeries[0].Points[3];
            AssertHelper.AreEqual(TextureType.Granite, p.Area.FillFormat.Texture, "chart.NSeries[3].Area.FillFormat.Texture");
        }
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


