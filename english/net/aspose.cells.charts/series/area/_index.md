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
// Called: aseries.Area.FillFormat.Texture = TextureType.Stationery;
public void Series_Property_Area()
{
    Workbook workbook = new Workbook();
    workbook = TestColumn.CreateChart(workbook);
    Chart chart = workbook.Worksheets[0].Charts[0];
    Series aseries = chart.NSeries[0];
    aseries.Area.FillFormat.Texture = TextureType.Stationery;

    checkTextureType_Stationery(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
    checkTextureType_Stationery(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
    checkTextureType_Stationery(workbook);
    workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
}
```

### See Also

* class [Area](../../../aspose.cells.drawing/area/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


