---
title: DataLabels.Text
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets the text of data label
type: docs
url: /net/aspose.cells.charts/datalabels/text/
---
## DataLabels.Text property

Gets or sets the text of data label.

```csharp
public override string Text { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(series.Points[0].DataLabels.Text, "+1.0");
public void DataLabels_Property_Text()
{
    Workbook wb = new Workbook(Constants.sourcePath + "graphtest-hidden.xlsm");
    Workbook wbCopy = new Workbook();
    wbCopy.Copy(wb);

    Worksheet ws = wbCopy.Worksheets[1];
    Chart ch = ws.Charts[0];
    ch.Calculate();
    SeriesCollection seriesCollection = ch.NSeries;
    for (int i = 0; i < seriesCollection.Count; i++)
    {
        Series series = seriesCollection[i];

        if (series.DataLabels.LinkedSource != null)
        {
            Assert.AreEqual(series.Points[0].DataLabels.Text, "+1.0");
            Assert.AreEqual(series.Points[1].DataLabels.Text, "+2.0");
            Assert.AreEqual(series.Points[2].DataLabels.Text, "+3.0");
        }
    }
}
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


