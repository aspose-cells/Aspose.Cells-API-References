---
title: Chart.FilteredNSeries
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets a SeriesCollection collection representing the data series that are filtered in the chart
type: docs
url: /net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

Gets a [`SeriesCollection`](../../seriescollection/) collection representing the data series that are filtered in the chart.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(2, workbookcopied.Worksheets[0].Charts[0].FilteredNSeries.Count);
[Test]
        public void Property_FilteredNSeries()
        {
            //Test for FilteredNSeries is missing in the copied worksheet
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;SeriesFiltered.xlsx&quot;);
            Worksheet sourceWorksheet = workbook.Worksheets[0];
            SeriesCollection filteredSeriesInOriginalWorksheet = sourceWorksheet.Charts[0].FilteredNSeries;
            Assert.AreEqual(2, filteredSeriesInOriginalWorksheet.Count);
            Worksheet CopiedSheet = sourceWorksheet.Workbook.Worksheets.Add(&quot;CopiedSheet&quot;);
            CopiedSheet.Copy(sourceWorksheet);
            SeriesCollection filteredSeriesInCopiedWorksheet = CopiedSheet.Charts[0].FilteredNSeries;
            Assert.AreEqual(2, filteredSeriesInCopiedWorksheet.Count);
            workbook.Save(Constants.destPath + &quot;SeriesFiltered.out.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;SeriesFiltered.out.xlsx&quot;);
            Assert.AreEqual(2, workbook.Worksheets[0].Charts[0].FilteredNSeries.Count);
            Assert.AreEqual(2, workbook.Worksheets[&quot;CopiedSheet&quot;].Charts[0].FilteredNSeries.Count);
            Workbook workbookcopied = new Workbook();
            workbookcopied.Copy(workbook);
            Assert.AreEqual(2, workbookcopied.Worksheets[0].Charts[0].FilteredNSeries.Count);
            Assert.AreEqual(2, workbookcopied.Worksheets[&quot;CopiedSheet&quot;].Charts[0].FilteredNSeries.Count);
            workbook.Save(Constants.destPath + &quot;SeriesFiltered.WorkbookOut.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;SeriesFiltered.WorkbookOut.xlsx&quot;);
            Assert.AreEqual(2, workbook.Worksheets[0].Charts[0].FilteredNSeries.Count);
            Assert.AreEqual(2, workbook.Worksheets[&quot;CopiedSheet&quot;].Charts[0].FilteredNSeries.Count);
        }
```

### See Also

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


