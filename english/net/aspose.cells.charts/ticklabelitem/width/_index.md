---
title: TickLabelItem.Width
second_title: Aspose.Cells for .NET API Reference
description: TickLabelItem property. Width of Ticklabel item in ratio of chart width
type: docs
url: /net/aspose.cells.charts/ticklabelitem/width/
---
## TickLabelItem.Width property

Width of Ticklabel item in ratio of chart width.

```csharp
public double Width { get; }
```

### Examples

```csharp
// Called: item.Width + item.X,
[Test]
        public void Property_Width()
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

* class [TickLabelItem](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


