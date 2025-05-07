---
title: DataLabels.DirectionType
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets and sets the direction of text
type: docs
url: /net/aspose.cells.charts/datalabels/directiontype/
---
## DataLabels.DirectionType property

Gets and sets the direction of text.

```csharp
public override ChartTextDirectionType DirectionType { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].DataLabels.DirectionType, ChartTextDirectionType.Stacked);
[Test]
        public void Property_DirectionType()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet46229.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].DataLabels.DirectionType = ChartTextDirectionType.Stacked;
            workbook.Save(Constants.destPath + "CellsNet46229.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet46229.xlsx");
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].DataLabels.DirectionType, ChartTextDirectionType.Stacked);
        }
```

### See Also

* enum [ChartTextDirectionType](../../charttextdirectiontype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


