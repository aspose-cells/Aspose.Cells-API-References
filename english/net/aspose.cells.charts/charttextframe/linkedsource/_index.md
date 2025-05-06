---
title: ChartTextFrame.LinkedSource
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Gets and sets a reference to the worksheet
type: docs
url: /net/aspose.cells.charts/charttextframe/linkedsource/
---
## ChartTextFrame.LinkedSource property

Gets and sets a reference to the worksheet.

```csharp
public virtual string LinkedSource { get; set; }
```

### Examples

```csharp
// Called: if (series.DataLabels.LinkedSource != null)
[Test]
        public void Property_LinkedSource()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;graphtest-hidden.xlsm&quot;);
            Workbook wbCopy = new Workbook();
            wbCopy.Copy(wb);

            Worksheet ws = wbCopy.Worksheets[1];
            Chart ch = ws.Charts[0];
            ch.Calculate();
            SeriesCollection seriesCollection = ch.NSeries;
            for (int i = 0; i &lt; seriesCollection.Count; i++)
            {
                Series series = seriesCollection[i];

                if (series.DataLabels.LinkedSource != null)
                {
                    Assert.AreEqual(series.Points[0].DataLabels.Text, &quot;+1.0&quot;);
                    Assert.AreEqual(series.Points[1].DataLabels.Text, &quot;+2.0&quot;);
                    Assert.AreEqual(series.Points[2].DataLabels.Text, &quot;+3.0&quot;);
                }
            }
        }
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


