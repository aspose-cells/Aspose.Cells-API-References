---
title: ChartPoint.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Returns a DataLabels object that represents the data label associated with this chart point
type: docs
url: /net/aspose.cells.charts/chartpoint/datalabels/
---
## ChartPoint.DataLabels property

Returns a `DataLabels` object that represents the data label associated with this chart point.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(_originalColor, series.Points[2].DataLabels.Font.Color);
public void ChartPoint_Property_DataLabels()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Charts/ChartAPI/TestHadrienMarker.xlsx");
    Chart chart = workbook.Worksheets[0].Charts[0];
    chart.Calculate();

    Color _originalColor = Color.FromArgb(255,255,0,0);
    Color _newColor = Color.FromArgb(255, 0, 128, 0);
    Series series = chart.NSeries[0];
    series.DataLabels.Font.Color = _newColor;
    Assert.AreEqual(_originalColor, series.Points[0].DataLabels.Font.Color);
    Assert.AreEqual(_originalColor, series.Points[1].DataLabels.Font.Color);
    Assert.AreEqual(_originalColor, series.Points[2].DataLabels.Font.Color);
    Assert.AreEqual(_newColor, series.Points[3].DataLabels.Font.Color);

    series.DataLabels.ApplyFont();
    Assert.AreEqual(_newColor, series.Points[0].DataLabels.Font.Color);
    Assert.AreEqual(_newColor, series.Points[1].DataLabels.Font.Color);
    Assert.AreEqual(_newColor, series.Points[2].DataLabels.Font.Color);
    Assert.AreEqual(_newColor, series.Points[3].DataLabels.Font.Color);
}
```

### See Also

* class [DataLabels](../../datalabels/)
* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


