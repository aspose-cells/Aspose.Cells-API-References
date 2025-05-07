---
title: Series.DataLabels
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the DataLabels object for the specified ASeries
type: docs
url: /net/aspose.cells.charts/series/datalabels/
---
## Series.DataLabels property

Represents the DataLabels object for the specified ASeries.

```csharp
public DataLabels DataLabels { get; }
```

### Examples

```csharp
// Called: chart.NSeries[0].DataLabels.IsTextWrapped = false;
[Test]
        public void Property_DataLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "FlexAnalysisReport+-+Unwrapped.xlsx");
            DataLabels labels = workbook.Worksheets[0].Charts[0].NSeries[0].DataLabels;
            Assert.AreEqual(labels.IsTextWrapped, false);
            workbook = new Workbook(Constants.sourcePath + "CellsNet42911.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].DataLabels.IsTextWrapped = false;
            chart.NSeries[1].DataLabels.IsTextWrapped = false;
            chart.NSeries[2].DataLabels.IsTextWrapped = false;
            Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.IsTextWrapped, false);
            workbook.Save(Constants.destPath + "CellsNet42911.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet42911.xlsx");
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.IsTextWrapped, false);
            Assert.AreEqual(chart.NSeries[1].DataLabels.IsTextWrapped, false);
            Assert.AreEqual(chart.NSeries[2].DataLabels.IsTextWrapped, false);
        }
```

### See Also

* class [DataLabels](../../datalabels/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


