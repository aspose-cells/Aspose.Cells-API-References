---
title: DataLabels.IsTextWrapped
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets a value indicating whether the text is wrapped
type: docs
url: /net/aspose.cells.charts/datalabels/istextwrapped/
---
## DataLabels.IsTextWrapped property

Gets or sets a value indicating whether the text is wrapped.

```csharp
public override bool IsTextWrapped { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[1].DataLabels.IsTextWrapped, false);
[Test]
        public void Property_IsTextWrapped()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;FlexAnalysisReport+-+Unwrapped.xlsx&quot;);
            DataLabels labels = workbook.Worksheets[0].Charts[0].NSeries[0].DataLabels;
            Assert.AreEqual(labels.IsTextWrapped, false);
            workbook = new Workbook(Constants.sourcePath + &quot;CellsNet42911.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.NSeries[0].DataLabels.IsTextWrapped = false;
            chart.NSeries[1].DataLabels.IsTextWrapped = false;
            chart.NSeries[2].DataLabels.IsTextWrapped = false;
            Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.IsTextWrapped, false);
            workbook.Save(Constants.destPath + &quot;CellsNet42911.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet42911.xlsx&quot;);
            chart = workbook.Worksheets[0].Charts[0];
            Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.IsTextWrapped, false);
            Assert.AreEqual(chart.NSeries[1].DataLabels.IsTextWrapped, false);
            Assert.AreEqual(chart.NSeries[2].DataLabels.IsTextWrapped, false);
        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


