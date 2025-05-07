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
// Called: Assert.AreEqual(2, workbook.Worksheets[0].Charts[0].FilteredNSeries.Count);
[Test]
        public void Property_FilteredNSeries()
        {
            //Test for FilteredNSeries is missing in the copied worksheet
            Workbook workbook = new Workbook(Constants.sourcePath + "SeriesFiltered.xlsx");
            Worksheet sourceWorksheet = workbook.Worksheets[0];
            SeriesCollection filteredSeriesInOriginalWorksheet = sourceWorksheet.Charts[0].FilteredNSeries;
            Assert.AreEqual(2, filteredSeriesInOriginalWorksheet.Count);
            Worksheet CopiedSheet = sourceWorksheet.Workbook.Worksheets.Add("CopiedSheet");
            CopiedSheet.Copy(sourceWorksheet);
            SeriesCollection filteredSeriesInCopiedWorksheet = CopiedSheet.Charts[0].FilteredNSeries;
            Assert.AreEqual(2, filteredSeriesInCopiedWorksheet.Count);
            workbook.Save(Constants.destPath + "SeriesFiltered.out.xlsx");
            workbook = new Workbook(Constants.destPath + "SeriesFiltered.out.xlsx");
            Assert.AreEqual(2, workbook.Worksheets[0].Charts[0].FilteredNSeries.Count);
            Assert.AreEqual(2, workbook.Worksheets["CopiedSheet"].Charts[0].FilteredNSeries.Count);
            Workbook workbookcopied = new Workbook();
            workbookcopied.Copy(workbook);
            Assert.AreEqual(2, workbookcopied.Worksheets[0].Charts[0].FilteredNSeries.Count);
            Assert.AreEqual(2, workbookcopied.Worksheets["CopiedSheet"].Charts[0].FilteredNSeries.Count);
            workbook.Save(Constants.destPath + "SeriesFiltered.WorkbookOut.xlsx");
            workbook = new Workbook(Constants.destPath + "SeriesFiltered.WorkbookOut.xlsx");
            Assert.AreEqual(2, workbook.Worksheets[0].Charts[0].FilteredNSeries.Count);
            Assert.AreEqual(2, workbook.Worksheets["CopiedSheet"].Charts[0].FilteredNSeries.Count);
        }
```

### See Also

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


