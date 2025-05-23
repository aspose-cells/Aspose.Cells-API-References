---
title: ShapeCollection.AddShapeInChartByScale
second_title: Aspose.Cells for .NET API Reference
description: ShapeCollection method. Add a shape to chart. All unit is percent scale of chart area
type: docs
url: /net/aspose.cells.drawing/shapecollection/addshapeinchartbyscale/
---
## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double) {#addshapeinchartbyscale}

Add a shape to chart. All unit is percent scale of chart area.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The drawing type. |
| placement | PlacementType | the placement type. |
| left | Double | Unit is percent scale of chart area width. |
| top | Double | Unit is percent scale of chart area height. |
| right | Double | Unit is percent scale of chart area width. |
| bottom | Double | Unit is percent scale of chart area height. |

### Examples

```csharp
// Called: Shape shape = chart.Shapes.AddShapeInChartByScale(MsoDrawingType.Rectangle, PlacementType.Move,
public void ShapeCollection_Method_AddShapeInChartByScale()
{
    //a test file contains a chart without any shapes (Such as bubbles, squares, and so on)
    Workbook book = new Workbook(Constants.sourcePath + "Column_Stacked+bubble.xlsx");
    Chart chart = book.Worksheets[1].Charts[0];
    //First, calculate data
    chart.Calculate();

    //1, Title
    Title title = chart.Title;
    //double title_x = title.X * chart.ChartObject.Width / 4000;
    //double title_y = title.Y * chart.ChartObject.Height / 4000;
    //double title_width = title.Width * chart.ChartObject.Width / 4000;
    double title_height = title.Height * chart.ChartObject.Height / 4000; //pixel
    //Add a circle after Title, Diameter = TitleHeight, 1/4000 unit
    Shape shape_title = chart.Shapes.AddShapeInChart(MsoDrawingType.Oval, PlacementType.Move,
        title.X + title.Width,
        title.Y,
        title.X + title.Width + (int)(title_height / chart.ChartObject.Width * 4000),
        title.Y + title.Height);
    shape_title.Fill.SolidFill.Color = Color.Green;
    Assert.AreEqual(chart.Shapes.Count, 1);

    //2, CategoryAxis
    Axis axis = chart.CategoryAxis;
    TickLabelItem[] items = axis.TickLabels.TickLabelItems;
    for (int i = 0; i < items.Length; i++)
    {
        TickLabelItem item = items[i];

        //Add a Rectangle on CategoryAxis, scale unit
        Shape shape = chart.Shapes.AddShapeInChartByScale(MsoDrawingType.Rectangle, PlacementType.Move,
            item.X,
            item.Y,
            item.Width + item.X,
            item.Height + item.Y);
        shape.Fill.SolidFill.Transparency = 1;
        Assert.IsTrue(chart.Shapes[i * 2 + 1].X - item.X * chart.ChartObject.Width - chart.ChartObject.X < 1);
        Assert.IsTrue(chart.Shapes[i * 2 + 1].Y - item.Y * chart.ChartObject.Height - chart.ChartObject.Y < 1);
        Assert.IsTrue(chart.Shapes[i * 2 + 1].Width - item.Width * chart.ChartObject.Width < 1);
        Assert.IsTrue(chart.Shapes[i * 2 + 1].Height - item.Height * chart.ChartObject.Height < 1);

        //Add a circle after CategoryAxis, Diameter = AxisHeight, scale unit
        Shape shape2 = chart.Shapes.AddShapeInChartByScale(MsoDrawingType.Oval, PlacementType.Move,
            item.Width + item.X,
            item.Y,
            item.Width + item.X + item.Height * chart.ActualChartSize.Height / chart.ActualChartSize.Width,
            item.Height + item.Y);
        shape2.Fill.SolidFill.Color = Color.Red;


    }
    //Save result file, chart with shapes (Such as bubbles, squares)
    book.Save(Constants.destPath + "example.xlsx");
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

## AddShapeInChartByScale(MsoDrawingType, PlacementType, double, double, double, double, byte[]) {#addshapeinchartbyscale_1}

Add a shape to chart .All unit is 1/4000 of chart area.

```csharp
public Shape AddShapeInChartByScale(MsoDrawingType type, PlacementType placement, double left, 
    double top, double right, double bottom, byte[] imageData)
```

| Parameter | Type | Description |
| --- | --- | --- |
| type | MsoDrawingType | The drawing type. |
| placement | PlacementType | the placement type. |
| left | Double | Unit is percent scale of chart area width. |
| top | Double | Unit is percent scale of chart area height. |
| right | Double | Unit is percent scale of chart area width. |
| bottom | Double | Unit is percent scale of chart area height. |
| imageData | Byte[] | If the shape is not a picture or ole object,imageData should be null. |

### Examples

```csharp
namespace AsposeCellsExamples.ShapeCollectionMethodAddShapeInChartByScaleWithMsoDrawingTypePlacementTypeDouDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;
    using System.IO;

    public class ShapeCollectionMethodAddShapeInChartByScaleWithMsoDrawingTypePlacementTypeDouDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data for chart
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Add a chart
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Prepare image data
            byte[] imageData = File.ReadAllBytes("example.png");

            try
            {
                // Call AddShapeInChartByScale method
                Shape shape = chart.Shapes.AddShapeInChartByScale(
                    MsoDrawingType.Rectangle,    // Type
                    PlacementType.Move,           // Placement
                    0.1,                          // Left (10% of chart width)
                    0.1,                         // Top (10% of chart height)
                    0.3,                          // Right (30% of chart width)
                    0.3,                         // Bottom (30% of chart height)
                    imageData);                   // Image data

                // Set shape properties
                shape.Name = "ChartRectangle";
                shape.Text = "Sample Shape in Chart";
                shape.Fill.Transparency = 0.5;

                Console.WriteLine("Shape added successfully to chart");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error adding shape to chart: {ex.Message}");
            }

            workbook.Save("AddShapeInChartByScaleDemo.xlsx");
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


