---
title: Chart.CategoryAxis
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts X axis
type: docs
url: /net/aspose.cells.charts/chart/categoryaxis/
---
## Chart.CategoryAxis property

Gets the chart's X axis.

```csharp
public Axis CategoryAxis { get; }
```

### Examples

```csharp
// Called: var fontNameCopied = newWorkbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.Font.Name;
[Test]
        public void Property_CategoryAxis()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-48386.xlsx");
            var fontName = workbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.Font.Name;
            Assert.AreEqual("Generis Sans Com", fontName, "TickLabels.Font.Name");
            var newWorkbook = new Workbook();
            newWorkbook.Copy(workbook);
            var fontNameCopied = newWorkbook.Worksheets[0].Charts[0].CategoryAxis.TickLabels.Font.Name;
            Assert.AreEqual("Generis Sans Com", fontNameCopied, "TickLabels.Font.Name");
        }
```

### See Also

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


