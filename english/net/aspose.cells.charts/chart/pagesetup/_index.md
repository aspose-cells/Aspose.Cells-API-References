---
title: Chart.PageSetup
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Represents the page setup description in this chart
type: docs
url: /net/aspose.cells.charts/chart/pagesetup/
---
## Chart.PageSetup property

Represents the page setup description in this chart.

```csharp
public PageSetup PageSetup { get; }
```

### Examples

```csharp
// Called: PageSetup ps = chart.PageSetup;
[Test]
        public void Property_PageSetup()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = &quot;Sheet&quot;;
            int iChartWorksheet = wb.Worksheets.Add(SheetType.Chart);
            ws = wb.Worksheets[iChartWorksheet];
            ChartCollection charts = ws.Charts;
            int chartIndex = charts.Add(ChartType.Column, 10, 10, 20, 20);
            Chart chart = charts[chartIndex];

            PageSetup ps = chart.PageSetup;
            string path = Constants.sourcePath + &quot;caffeine.wmf&quot;;
            FileStream inFile = new System.IO.FileStream(path, System.IO.FileMode.Open, System.IO.FileAccess.Read);
            byte[] binaryData = new byte[inFile.Length];
            long bytesRead = inFile.Read(binaryData, 0, (int)inFile.Length);
            ps.SetHeaderPicture(0, binaryData);
            ps.SetHeader(0, &quot;&amp;G&quot;);
            //ps.SetHeader(0, &quot;BI&quot;);
            ps.SetHeader(1, &quot;Center&quot;);
            wb.Save(Constants.destPath + &quot;CELLSNET42437.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET42437.xlsx&quot;);
            Assert.AreEqual(wb.Worksheets[iChartWorksheet].Charts[0].PageSetup.GetPicture(true, 0) != null, true);
        }
```

### See Also

* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


