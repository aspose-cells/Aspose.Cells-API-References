---
title: DataLabels.Text
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Gets or sets the text of data label
type: docs
url: /net/aspose.cells.charts/datalabels/text/
---
## DataLabels.Text property

Gets or sets the text of data label.

```csharp
public override string Text { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.Text, "Bubble 1");
[Test]
        public void Property_Text()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet41740.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            Chart chart = worksheet.Charts[0];
            Assert.AreEqual(chart.NSeries[0].Points[0].DataLabels.Text, "Bubble 1");

        }
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


