---
title: Chart.Shapes
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Returns all drawing shapes in this chart
type: docs
url: /net/aspose.cells.charts/chart/shapes/
---
## Chart.Shapes property

Returns all drawing shapes in this chart.

```csharp
public ShapeCollection Shapes { get; }
```

### Examples

```csharp
// Called: sheet.Charts[0].Shapes.AddShapeInChart(MsoDrawingType.CheckBox,
[Test]
        public void Property_Shapes()
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
            workbook.Save(Constants.destPath + " CELLSNET-40174.xlsx");
        }
```

### See Also

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


