---
title: DataLabels.Font
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets the font of the DataLabels
type: docs
url: /net/aspose.cells.charts/datalabels/font/
---
## DataLabels.Font property

Gets the font of the DataLabels;

```csharp
public override Font Font { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Generis Sans Com&amp;quot;, chartResaved.NSeries[0].DataLabels.Font.Name, &amp;quot;Resaved DataLabesl.Font.Name&amp;quot;);
[Test]
        public void Property_Font()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-49161.xlsm&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chart.ValueAxis.TickLabels.Font.Name, &quot;ValueAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chart.CategoryAxis.TickLabels.Font.Name, &quot;CategoryAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chart.CategoryAxis.Title.Font.Name, &quot;ValueAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chart.NSeries[0].DataLabels.Font.Name, &quot;DataLabesl.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chart.Title.Font.Name, &quot;Title.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chart.Legend.Font.Name, &quot;Legend.Font.Name&quot;);

            var newWorkbook = new Workbook();
            newWorkbook.Copy(workbook);
            var chartCopied = newWorkbook.Worksheets[0].Charts[0];
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.ValueAxis.TickLabels.Font.Name, &quot;Copied ValueAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.CategoryAxis.TickLabels.Font.Name, &quot;Copied CategoryAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.CategoryAxis.Title.Font.Name, &quot;Copied ValueAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.NSeries[0].DataLabels.Font.Name, &quot;Copied DataLabesl.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.Title.Font.Name, &quot;Copied Title.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.Legend.Font.Name, &quot;Copied Legend.Font.Name&quot;);

            chartCopied.Calculate();
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.ValueAxis.TickLabels.Font.Name, &quot;Calculated Copied ValueAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.CategoryAxis.TickLabels.Font.Name, &quot;Calculated Copied CategoryAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.CategoryAxis.Title.Font.Name, &quot;Calculated Copied ValueAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.NSeries[0].DataLabels.Font.Name, &quot;Calculated Copied DataLabesl.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.Title.Font.Name, &quot;Calculated Copied Title.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartCopied.Legend.Font.Name, &quot;Calculated Copied Legend.Font.Name&quot;);

            newWorkbook.Save(Constants.destPath + &quot;CELLSNET-49161_Resave.xlsx&quot;, SaveFormat.Xlsx);
            newWorkbook = new Workbook(newWorkbook.FileName);
            var chartResaved = newWorkbook.Worksheets[0].Charts[0];
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartResaved.ValueAxis.TickLabels.Font.Name, &quot;Resaved ValueAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartResaved.CategoryAxis.TickLabels.Font.Name, &quot;Resaved CategoryAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartResaved.CategoryAxis.Title.Font.Name, &quot;Resaved ValueAxis TickLabels.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartResaved.NSeries[0].DataLabels.Font.Name, &quot;Resaved DataLabesl.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartResaved.Title.Font.Name, &quot;Resaved Title.Font.Name&quot;);
            Assert.AreEqual(&quot;Generis Sans Com&quot;, chartResaved.Legend.Font.Name, &quot;Resaved Legend.Font.Name&quot;);
        }
```

### See Also

* class [Font](../../../aspose.cells/font/)
* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


