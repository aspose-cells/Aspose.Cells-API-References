---
title: ChartPoint.YValue
second_title: Aspose.Cells for .NET API Reference
description: ChartPoint property. Gets or sets the Y value of the chart point
type: docs
url: /net/aspose.cells.charts/chartpoint/yvalue/
---
## ChartPoint.YValue property

Gets or sets the Y value of the chart point.

```csharp
public object YValue { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(40, points[10].YValue, "Quartile2 Value");
public void ChartPoint_Property_YValue()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "Charts/BoxWhisker/Charts1.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    Chart chart = worksheet.Charts[0];
    Series aSeries = chart.NSeries[0];
    var points = aSeries.Points;
    points[9].DataLabels.ShowSeriesName = true;

    ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
    calculateOptions.UpdateAllPoints = true;

    chart.Calculate(calculateOptions);
    AssertHelper.AreEqual(10, points[1].YValue, "ChartPoint Value");
    AssertHelper.AreEqual(40, points[2].YValue, "ChartPoint Value");
    AssertHelper.AreEqual(25, points[9].YValue, "Quartile1 Value");
    AssertHelper.AreEqual(40, points[10].YValue, "Quartile2 Value");
    AssertHelper.AreEqual(115, points[11].YValue, "Quartile3 Value");
    AssertHelper.AreEqual(true, (double)points[12].YValue > 65.666 && (double)points[12].YValue < 65.667, "Mean Value");

    //  AssertHelper.AreEqual("Series1, 25", points[9].DataLabels.Text, "DataLabel(Quartile1) Text");
    // AssertHelper.AreEqual("40", points[10].DataLabels.Text, "DataLabel(Quartile2) Text");

    SeriesLayoutProperties layout = aSeries.LayoutProperties;
    AssertHelper.AreEqual(true, layout.ShowMeanMarker, "ShowMeanMarker");
    AssertHelper.AreEqual(false, layout.ShowMeanLine, "ShowMeanLine");
    AssertHelper.AreEqual(true, layout.ShowOutlierPoints, "ShowOutlierPoints");
    AssertHelper.AreEqual(true, layout.ShowInnerPoints, "ShowInnerPoints");
    AssertHelper.AreEqual(QuartileCalculationType.Exclusive, layout.QuartileCalculation, "QuartileCalculationType");

    aSeries = chart.NSeries[1];
    layout = aSeries.LayoutProperties;
    AssertHelper.AreEqual(false, layout.ShowMeanMarker, "ShowMeanMarker");
    AssertHelper.AreEqual(true, layout.ShowMeanLine, "ShowMeanLine");
    AssertHelper.AreEqual(false, layout.ShowOutlierPoints, "ShowOutlierPoints");
    AssertHelper.AreEqual(false, layout.ShowInnerPoints, "ShowInnerPoints");
    AssertHelper.AreEqual(QuartileCalculationType.Exclusive, layout.QuartileCalculation, "QuartileCalculationType");

    aSeries = chart.NSeries[2];
    layout = aSeries.LayoutProperties;
    AssertHelper.AreEqual(QuartileCalculationType.Inclusive, layout.QuartileCalculation, "QuartileCalculationType");
    string destPath = Constants.destPath + "Charts/BoxWhisker";
    if (!Directory.Exists(destPath))
        Directory.CreateDirectory(destPath);

    workbook.Save(destPath + "/ChartsReSave.xlsx");
    workbook = new Workbook(workbook.FileName);
    chart = worksheet.Charts[0];
    aSeries = chart.NSeries[0];
    points = aSeries.Points;
    chart.Calculate(calculateOptions);
    AssertHelper.AreEqual(10, points[1].YValue, "ChartPoint Value");
    AssertHelper.AreEqual(40, points[2].YValue, "ChartPoint Value");
    AssertHelper.AreEqual(25, points[9].YValue, "Quartile1 Value");
    AssertHelper.AreEqual(40, points[10].YValue, "Quartile2 Value");
    AssertHelper.AreEqual(115, points[11].YValue, "Quartile3 Value");
    AssertHelper.AreEqual(true, (double)points[12].YValue > 65.666 && (double)points[12].YValue < 65.667, "Mean Value");

    //  AssertHelper.AreEqual("Series1, 25", points[9].DataLabels.Text, "DataLabel(Quartile1) Text");
    //AssertHelper.AreEqual("40", points[10].DataLabels.Text, "DataLabel(Quartile2) Text");

    layout = aSeries.LayoutProperties;
    AssertHelper.AreEqual(true, layout.ShowMeanMarker, "ShowMeanMarker");
    AssertHelper.AreEqual(false, layout.ShowMeanLine, "ShowMeanLine");
    AssertHelper.AreEqual(true, layout.ShowOutlierPoints, "ShowOutlierPoints");
    AssertHelper.AreEqual(true, layout.ShowInnerPoints, "ShowInnerPoints");
    AssertHelper.AreEqual(QuartileCalculationType.Exclusive, layout.QuartileCalculation, "QuartileCalculationType");

    aSeries = chart.NSeries[1];
    layout = aSeries.LayoutProperties;
    AssertHelper.AreEqual(false, layout.ShowMeanMarker, "ShowMeanMarker");
    AssertHelper.AreEqual(true, layout.ShowMeanLine, "ShowMeanLine");
    AssertHelper.AreEqual(false, layout.ShowOutlierPoints, "ShowOutlierPoints");
    AssertHelper.AreEqual(false, layout.ShowInnerPoints, "ShowInnerPoints");
    AssertHelper.AreEqual(QuartileCalculationType.Exclusive, layout.QuartileCalculation, "QuartileCalculationType");

}
```

### See Also

* class [ChartPoint](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


