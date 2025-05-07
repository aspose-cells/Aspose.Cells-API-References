---
title: Class TickLabelItem
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Charts.TickLabelItem class. Represents a tick label in the chart
type: docs
url: /net/aspose.cells.charts/ticklabelitem/
---
## TickLabelItem class

Represents a tick label in the chart.

```csharp
public class TickLabelItem
```

## Properties

| Name | Description |
| --- | --- |
| [Height](../../aspose.cells.charts/ticklabelitem/height/) { get; } | Height of Ticklabel item in ratio of chart height. |
| [Width](../../aspose.cells.charts/ticklabelitem/width/) { get; } | Width of Ticklabel item in ratio of chart width. |
| [X](../../aspose.cells.charts/ticklabelitem/x/) { get; } | X coordinates of Ticklabel item in ratio of chart width. |
| [Y](../../aspose.cells.charts/ticklabelitem/y/) { get; } | Y coordinates of Ticklabel item in ratio of chart height. |

### Examples

```csharp
// Called: TickLabelItem[] items = axis.TickLabels.TickLabelItems;
[Test]
        public void Type_TickLabelItem()
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

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


