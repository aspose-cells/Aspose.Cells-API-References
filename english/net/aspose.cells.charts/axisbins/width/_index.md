---
title: AxisBins.Width
second_title: Aspose.Cells for .NET API Reference
description: AxisBins property. Gets or sets the width of axis bin
type: docs
url: /net/aspose.cells.charts/axisbins/width/
---
## AxisBins.Width property

Gets or sets the width of axis bin

```csharp
public double Width { get; set; }
```

### Examples

```csharp
// Called: chart.CategoryAxis.Bins.Width = 12;
[Test]
        public void Property_Width()
        {
            // CELLSNET49316
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells[&quot;B1&quot;].PutValue(10);
            worksheet.Cells[&quot;C1&quot;].PutValue(20);
            worksheet.Cells[&quot;D1&quot;].PutValue(15);
            worksheet.Cells[&quot;B2&quot;].PutValue(35);
            worksheet.Cells[&quot;C2&quot;].PutValue(32);
            worksheet.Cells[&quot;D2&quot;].PutValue(31);
            worksheet.Cells[&quot;B3&quot;].PutValue(185);
            worksheet.Cells[&quot;C3&quot;].PutValue(202);
            worksheet.Cells[&quot;D3&quot;].PutValue(224);
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Histogram, 7, 1, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add(&quot;B2:D2&quot;, false);
            chart.NSeries.Add(&quot;B3:D3&quot;, false);
            chart.NSeries.Add(&quot;B4:D4&quot;, false);
            chart.NSeries.CategoryData = &quot;B1:D1&quot;;
            chart.CategoryAxis.Bins.Width = 12;
            workbook.Save(Constants.destPath + &quot;CELLSNET49168.xlsx&quot;);

            workbook = new Workbook(workbook.FileName);
            var bins = workbook.Worksheets[0].Charts[0].CategoryAxis.Bins;
            Assert.AreEqual(false, bins.IsByCategory, &quot;By Category&quot;);
            Assert.AreEqual(12, bins.Width, &quot;Bin Width&quot;);
            bins.Count = 3;
            bins.Overflow = 10;
            bins.Underflow = 0.5;
            workbook.Save(Constants.destPath + &quot;CELLSNET49168.xlsx&quot;);
            workbook = new Workbook(workbook.FileName);
            bins = workbook.Worksheets[0].Charts[0].CategoryAxis.Bins;
            Assert.AreEqual(false, bins.IsByCategory, &quot;By Category&quot;);
            ;
            Assert.AreEqual(3, bins.Count, &quot;Bins Count&quot;);
            Assert.AreEqual(10, bins.Overflow, &quot;Bin Overflow&quot;);
            Assert.AreEqual(0.5, bins.Underflow, &quot;Bin Underflow&quot;);
        }
```

### See Also

* class [AxisBins](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


