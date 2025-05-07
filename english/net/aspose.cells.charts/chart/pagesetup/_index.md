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
// Called: Assert.IsTrue(chart.PageSetup.IsAutomaticPaperSize);
[Test]
        public void Property_PageSetup()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47459.xlsb");
            workbook.Save(Constants.destPath + "CellsNet47459.xlsx");
            workbook = new Workbook(Constants.destPath + "CellsNet47459.xlsx");
            workbook.Save(Constants.destPath + "CellsNet47459.xlsb");
            workbook = new Workbook(Constants.destPath + "CellsNet47459.xlsb");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.IsTrue(chart.PageSetup.IsAutomaticPaperSize);
        }
```

### See Also

* class [PageSetup](../../../aspose.cells/pagesetup/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


