---
title: ShapeCollection.AddShapeInChart
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Add a shape to chart .All unit is 1/4000 of chart area
type: docs
url: /net/aspose.cells.drawing/shapecollection/addshapeinchart/
---
## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int, byte[]) {#addshapeinchart_1}

Add a shape to chart .All unit is 1/4000 of chart area.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom, byte[] imageData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The drawing type. |
| placement | PlacementType | the placement type. |
| left | Int32 | In unit of 1/4000 chart area width. |
| top | Int32 | In unit of 1/4000 chart area height. |
| right | Int32 | In unit of 1/4000 chart area width. |
| bottom | Int32 | In unit of 1/4000 chart area height. |
| imageData | Byte[] | If the shape is not a picture or ole object,imageData should be null. |

### Examples

```csharp
namespace AsposeCellsExamples.ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ShapeCollectionMethodAddShapeInChartWithMsoDrawingTypePlacementTypeIntDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data and create a chart
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(80);

            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Prepare image data
            byte[] imageData = File.ReadAllBytes("sample.png");

            try
            {
                // Call AddShapeInChart with specific parameters
                Shape shape = chart.Shapes.AddShapeInChart(
                    MsoDrawingType.Rectangle,    // Type
                    PlacementType.Move,          // Placement
                    100,                         // Left position
                    100,                         // Top position
                    200,                         // Right position
                    200,                         // Bottom position
                    imageData                    // Image data
                );

                // Set shape properties
                shape.Name = "ChartRectangle";
                shape.Text = "Shape in Chart";
                shape.Fill.SolidFill.Color = System.Drawing.Color.LightBlue;
                shape.Line.CompoundType = MsoLineStyle.ThickThin;
                shape.Line.Weight = 2; // Medium weight (approximately 2 points)

                Console.WriteLine("Shape added to chart successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding shape to chart: {ex.Message}");
            }

            // Save the result
            workbook.Save("AddShapeInChartDemo.xlsx");
        }
    }
}
```

### See Also

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## AddShapeInChart(MsoDrawingType, PlacementType, int, int, int, int) {#addshapeinchart}

Add a shape to chart .All unit is 1/4000 of chart area.

```csharp
public Shape AddShapeInChart(MsoDrawingType type, PlacementType placement, int left, int top, 
    int right, int bottom)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The drawing type. |
| placement | PlacementType | the placement type. |
| left | Int32 | In unit of 1/4000 chart area width. |
| top | Int32 | In unit of 1/4000 chart area height. |
| right | Int32 | In unit of 1/4000 chart area width. |
| bottom | Int32 | In unit of 1/4000 chart area height. |

### Examples

```csharp
// Called: sheet.Charts[0].Shapes.AddShapeInChart(MsoDrawingType.CheckBox,
public void ShapeCollection_Method_AddShapeInChart()
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

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


