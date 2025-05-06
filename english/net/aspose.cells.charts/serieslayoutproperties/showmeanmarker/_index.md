---
title: SeriesLayoutProperties.ShowMeanMarker
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Indicates whether showing markers denoting the mean
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/showmeanmarker/
---
## SeriesLayoutProperties.ShowMeanMarker property

Indicates whether showing markers denoting the mean.

```csharp
public bool ShowMeanMarker { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(false, layout.ShowMeanMarker, &amp;quot;ShowMeanMarker&amp;quot;);
[Test]
        public void Property_ShowMeanMarker()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts/BoxWhisker/Charts1.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            Series aSeries = chart.NSeries[0];
            var points = aSeries.Points;
            points[9].DataLabels.ShowSeriesName = true;

            ChartCalculateOptions calculateOptions = new ChartCalculateOptions();
            calculateOptions.UpdateAllPoints = true;

            chart.Calculate(calculateOptions);
            AssertHelper.AreEqual(10, points[1].YValue, &quot;ChartPoint Value&quot;);
            AssertHelper.AreEqual(40, points[2].YValue, &quot;ChartPoint Value&quot;);
            AssertHelper.AreEqual(25, points[9].YValue, &quot;Quartile1 Value&quot;);
            AssertHelper.AreEqual(40, points[10].YValue, &quot;Quartile2 Value&quot;);
            AssertHelper.AreEqual(115, points[11].YValue, &quot;Quartile3 Value&quot;);
            AssertHelper.AreEqual(true, (double)points[12].YValue &gt; 65.666 &amp;&amp; (double)points[12].YValue &lt; 65.667, &quot;Mean Value&quot;);

            //  AssertHelper.AreEqual(&quot;Series1, 25&quot;, points[9].DataLabels.Text, &quot;DataLabel(Quartile1) Text&quot;);
            // AssertHelper.AreEqual(&quot;40&quot;, points[10].DataLabels.Text, &quot;DataLabel(Quartile2) Text&quot;);

            SeriesLayoutProperties layout = aSeries.LayoutProperties;
            AssertHelper.AreEqual(true, layout.ShowMeanMarker, &quot;ShowMeanMarker&quot;);
            AssertHelper.AreEqual(false, layout.ShowMeanLine, &quot;ShowMeanLine&quot;);
            AssertHelper.AreEqual(true, layout.ShowOutlierPoints, &quot;ShowOutlierPoints&quot;);
            AssertHelper.AreEqual(true, layout.ShowInnerPoints, &quot;ShowInnerPoints&quot;);
            AssertHelper.AreEqual(QuartileCalculationType.Exclusive, layout.QuartileCalculation, &quot;QuartileCalculationType&quot;);

            aSeries = chart.NSeries[1];
            layout = aSeries.LayoutProperties;
            AssertHelper.AreEqual(false, layout.ShowMeanMarker, &quot;ShowMeanMarker&quot;);
            AssertHelper.AreEqual(true, layout.ShowMeanLine, &quot;ShowMeanLine&quot;);
            AssertHelper.AreEqual(false, layout.ShowOutlierPoints, &quot;ShowOutlierPoints&quot;);
            AssertHelper.AreEqual(false, layout.ShowInnerPoints, &quot;ShowInnerPoints&quot;);
            AssertHelper.AreEqual(QuartileCalculationType.Exclusive, layout.QuartileCalculation, &quot;QuartileCalculationType&quot;);

            aSeries = chart.NSeries[2];
            layout = aSeries.LayoutProperties;
            AssertHelper.AreEqual(QuartileCalculationType.Inclusive, layout.QuartileCalculation, &quot;QuartileCalculationType&quot;);
            string destPath = Constants.destPath + &quot;Charts/BoxWhisker&quot;;
            if (!Directory.Exists(destPath))
                Directory.CreateDirectory(destPath);

            workbook.Save(destPath + &quot;/ChartsReSave.xlsx&quot;);
            workbook = new Workbook(workbook.FileName);
            chart = worksheet.Charts[0];
            aSeries = chart.NSeries[0];
            points = aSeries.Points;
            chart.Calculate(calculateOptions);
            AssertHelper.AreEqual(10, points[1].YValue, &quot;ChartPoint Value&quot;);
            AssertHelper.AreEqual(40, points[2].YValue, &quot;ChartPoint Value&quot;);
            AssertHelper.AreEqual(25, points[9].YValue, &quot;Quartile1 Value&quot;);
            AssertHelper.AreEqual(40, points[10].YValue, &quot;Quartile2 Value&quot;);
            AssertHelper.AreEqual(115, points[11].YValue, &quot;Quartile3 Value&quot;);
            AssertHelper.AreEqual(true, (double)points[12].YValue &gt; 65.666 &amp;&amp; (double)points[12].YValue &lt; 65.667, &quot;Mean Value&quot;);

            //  AssertHelper.AreEqual(&quot;Series1, 25&quot;, points[9].DataLabels.Text, &quot;DataLabel(Quartile1) Text&quot;);
            //AssertHelper.AreEqual(&quot;40&quot;, points[10].DataLabels.Text, &quot;DataLabel(Quartile2) Text&quot;);

            layout = aSeries.LayoutProperties;
            AssertHelper.AreEqual(true, layout.ShowMeanMarker, &quot;ShowMeanMarker&quot;);
            AssertHelper.AreEqual(false, layout.ShowMeanLine, &quot;ShowMeanLine&quot;);
            AssertHelper.AreEqual(true, layout.ShowOutlierPoints, &quot;ShowOutlierPoints&quot;);
            AssertHelper.AreEqual(true, layout.ShowInnerPoints, &quot;ShowInnerPoints&quot;);
            AssertHelper.AreEqual(QuartileCalculationType.Exclusive, layout.QuartileCalculation, &quot;QuartileCalculationType&quot;);

            aSeries = chart.NSeries[1];
            layout = aSeries.LayoutProperties;
            AssertHelper.AreEqual(false, layout.ShowMeanMarker, &quot;ShowMeanMarker&quot;);
            AssertHelper.AreEqual(true, layout.ShowMeanLine, &quot;ShowMeanLine&quot;);
            AssertHelper.AreEqual(false, layout.ShowOutlierPoints, &quot;ShowOutlierPoints&quot;);
            AssertHelper.AreEqual(false, layout.ShowInnerPoints, &quot;ShowInnerPoints&quot;);
            AssertHelper.AreEqual(QuartileCalculationType.Exclusive, layout.QuartileCalculation, &quot;QuartileCalculationType&quot;);

        }
```

### See Also

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


