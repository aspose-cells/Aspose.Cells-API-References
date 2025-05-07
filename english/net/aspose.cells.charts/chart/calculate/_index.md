---
title: Chart.Calculate
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Calculates the custom position of plot area axes if the position of them are auto assigned
type: docs
url: /net/aspose.cells.charts/chart/calculate/
---
## Calculate() {#calculate}

Calculates the custom position of plot area, axes if the position of them are auto assigned.

```csharp
public void Calculate()
```

### Examples

```csharp
// Called: chart.Calculate();
[Test]
        public void Method_Calculate()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA43532.xlsm");
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.Calculate();
            SeriesCollection nSeries = chart.NSeries;
            for (int i = 8; i < nSeries.Count; i++)
            {
                Assert.AreEqual(nSeries[7].DisplayName, nSeries[i].DisplayName, "Series DisplayName");
            }
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Calculate(ChartCalculateOptions) {#calculate_1}

Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options.

```csharp
public void Calculate(ChartCalculateOptions calculateOptions)
```

### Examples

```csharp
// Called: chart.Calculate(new ChartCalculateOptions() { UpdateAllPoints = true });
[Test]
        public void Method_ChartCalculateOptions_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Charts/ChartAPI/TimChartORama-source.xlsx");
            Chart chart = workbook.Worksheets["HELLO CHARTS"].Charts[0];
            chart.Calculate(new ChartCalculateOptions() { UpdateAllPoints = true });
            Assert.AreEqual("100", chart.NSeries[0].Points[0].DataLabels.Text);
            Assert.AreEqual("200", chart.NSeries[0].Points[1].DataLabels.Text);
            Assert.AreEqual("300", chart.NSeries[0].Points[2].DataLabels.Text);
            Assert.AreEqual("Custom Data Label 2", chart.NSeries[0].Points[3].DataLabels.Text);

            Assert.AreEqual("400", chart.NSeries[1].Points[0].DataLabels.Text);
            Assert.AreEqual("Custom Data Label 1", chart.NSeries[1].Points[1].DataLabels.Text);
            Assert.AreEqual("800", chart.NSeries[1].Points[2].DataLabels.Text);
            Assert.AreEqual("1000", chart.NSeries[1].Points[3].DataLabels.Text);

            Assert.AreEqual("100", chart.NSeries[2].Points[0].DataLabels.Text);
            Assert.AreEqual("500", chart.NSeries[2].Points[1].DataLabels.Text);
            Assert.AreEqual("900", chart.NSeries[2].Points[2].DataLabels.Text);
            Assert.AreEqual("1200", chart.NSeries[2].Points[3].DataLabels.Text);
        }
```

### See Also

* class [ChartCalculateOptions](../../chartcalculateoptions/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


