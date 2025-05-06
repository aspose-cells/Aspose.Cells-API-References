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
[Test]
        public void Method_Double_()
        {
            //a test file contains a chart without any shapes (Such as bubbles, squares, and so on)
            Workbook book = new Workbook(Constants.sourcePath + &quot;Column_Stacked+bubble.xlsx&quot;);
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
            for (int i = 0; i &lt; items.Length; i++)
            {
                TickLabelItem item = items[i];

                //Add a Rectangle on CategoryAxis, scale unit
                Shape shape = chart.Shapes.AddShapeInChartByScale(MsoDrawingType.Rectangle, PlacementType.Move,
                    item.X,
                    item.Y,
                    item.Width + item.X,
                    item.Height + item.Y);
                shape.Fill.SolidFill.Transparency = 1;
                Assert.IsTrue(chart.Shapes[i * 2 + 1].X - item.X * chart.ChartObject.Width - chart.ChartObject.X &lt; 1);
                Assert.IsTrue(chart.Shapes[i * 2 + 1].Y - item.Y * chart.ChartObject.Height - chart.ChartObject.Y &lt; 1);
                Assert.IsTrue(chart.Shapes[i * 2 + 1].Width - item.Width * chart.ChartObject.Width &lt; 1);
                Assert.IsTrue(chart.Shapes[i * 2 + 1].Height - item.Height * chart.ChartObject.Height &lt; 1);

                //Add a circle after CategoryAxis, Diameter = AxisHeight, scale unit
                Shape shape2 = chart.Shapes.AddShapeInChartByScale(MsoDrawingType.Oval, PlacementType.Move,
                    item.Width + item.X,
                    item.Y,
                    item.Width + item.X + item.Height * chart.ActualChartSize.Height / chart.ActualChartSize.Width,
                    item.Height + item.Y);
                shape2.Fill.SolidFill.Color = Color.Red;


            }
            //Save result file, chart with shapes (Such as bubbles, squares)
            book.Save(Constants.destPath + &quot;CELLSNET50017_Out.xlsx&quot;);
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

### See Also

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


