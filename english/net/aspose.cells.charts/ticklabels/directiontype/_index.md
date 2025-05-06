---
title: TickLabels.DirectionType
second_title: Aspose.Cells for .NET API Reference
description: TickLabels property. Gets and sets the direction of text
type: docs
url: /net/aspose.cells.charts/ticklabels/directiontype/
---
## TickLabels.DirectionType property

Gets and sets the direction of text.

```csharp
public ChartTextDirectionType DirectionType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.CategoryAxis.TickLabels.DirectionType, ChartTextDirectionType.Horizontal);
[Test]
        public void Property_DirectionType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46229.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Horizontal;
            workbook.Save(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.CategoryAxis.TickLabels.DirectionType, ChartTextDirectionType.Horizontal);
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Stacked;
            workbook.Save(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.CategoryAxis.TickLabels.DirectionType, ChartTextDirectionType.Stacked);
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Vertical;
            workbook.Save(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.CategoryAxis.TickLabels.DirectionType, ChartTextDirectionType.Vertical);
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Rotate90;
            workbook.Save(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.CategoryAxis.TickLabels.DirectionType, ChartTextDirectionType.Rotate90);
            chart.CategoryAxis.TickLabels.DirectionType = ChartTextDirectionType.Rotate270;
            workbook.Save(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet46229.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.CategoryAxis.TickLabels.DirectionType, ChartTextDirectionType.Rotate270);
        }
```

### See Also

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [TickLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


