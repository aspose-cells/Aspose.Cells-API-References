---
title: DataLabels.Position
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents the position of the data label
type: docs
url: /net/aspose.cells.charts/datalabels/position/
---
## DataLabels.Position property

Represents the position of the data label.

```csharp
public LabelPositionType Position { get; set; }
```

### Examples

```csharp
// Called: chart.NSeries[0].DataLabels.Position = LabelPositionType.BestFit;
[Test]
        public void Property_Position()
        {
            Workbook workbook = new Workbook();
            workbook = TestPie.CreateChart(workbook);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].DataLabels.ShowValue = true;
            chart.NSeries[0].DataLabels.Position = LabelPositionType.BestFit;

            checkLabelPositionType_BestFit(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
            checkLabelPositionType_BestFit(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Xlsx);
            checkLabelPositionType_BestFit(workbook);
            workbook = Util.ReSave(workbook, SaveFormat.Excel97To2003);
        }
```

### See Also

* enum [LabelPositionType](../../labelpositiontype/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


