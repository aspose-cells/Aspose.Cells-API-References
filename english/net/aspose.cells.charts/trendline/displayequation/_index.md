---
title: Trendline.DisplayEquation
second_title: Aspose.Cells for .NET API Reference
description: Trendline property. Represents if the equation for the trendline is displayed on the chart in the same data label as the Rsquared value. Setting this property to True automatically turns on data labels
type: docs
url: /net/aspose.cells.charts/trendline/displayequation/
---
## Trendline.DisplayEquation property

Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels.

```csharp
public bool DisplayEquation { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(true, ts0.DisplayEquation);
[Test]
        public void Property_DisplayEquation()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts/ChartAPI/UnvisibleTrendline.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            SeriesCollection sc = chart.NSeries;
            TrendlineCollection tls = sc[0].TrendLines;
            Assert.AreEqual(1, tls.Count);
            Trendline ts0 = tls[0];
            Assert.AreEqual(LineCapType.Round, ts0.CapType);
            Assert.AreEqual(MsoLineStyle.Single, ts0.CompoundType);
            Assert.AreEqual(false, ts0.IsVisible);
            Assert.AreEqual(true, ts0.DisplayEquation);
        }
```

### See Also

* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


