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
// Called: Shape shape_title = chart.Shapes.AddShapeInChart(MsoDrawingType.Oval, PlacementType.Move,
[Test]
        public void Method_Int32_()
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
            book.Save(Constants.destPath + "CELLSNET50017_Out.xlsx");
        }
```

### See Also

* class [Shape](../../shape/)
* enum [MsoDrawingType](../../msodrawingtype/)
* enum [PlacementType](../../placementtype/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


