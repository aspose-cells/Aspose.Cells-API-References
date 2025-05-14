---
title: ChartCollection.AddFloatingChart
second_title: Aspose.Cells for .NET API Reference
description: ChartCollection method. Adds a chart to the collection
type: docs
url: /net/aspose.cells.charts/chartcollection/addfloatingchart/
---
## ChartCollection.AddFloatingChart method

Adds a chart to the collection.

```csharp
public int AddFloatingChart(ChartType type, int left, int top, int width, int height)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | ChartType | Chart type |
| left | Int32 | The x offset to corner |
| top | Int32 | The y offset to corner |
| width | Int32 | The chart width |
| height | Int32 | The chart height |

### Return Value

[`Chart`](../../chart/) object index.

### Examples

```csharp
// Called: sheet.Charts.AddFloatingChart(ChartType.Column, 0, 0, 1024, 960);
public void ChartCollection_Method_AddFloatingChart()
{
    Workbook workbook = new Workbook();
    int index = workbook.Worksheets.Add(SheetType.Chart);
    Worksheet sheet = workbook.Worksheets[index];
    sheet.Charts.AddFloatingChart(ChartType.Column, 0, 0, 1024, 960);
    sheet.Charts[0].NSeries.Add("{1,2,3}", false);
    sheet.Charts[0].Shapes.AddShapeInChart(MsoDrawingType.CheckBox,
        PlacementType.Move, 400, 400, 1000, 600);
    sheet.Charts[0].Shapes[0].Text = "CheckBox 1";
    int width = sheet.Charts[0].Shapes[0].Width;
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* enum [ChartType](../../charttype/)
* class [ChartCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


