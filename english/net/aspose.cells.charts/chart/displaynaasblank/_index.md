---
title: Chart.DisplayNaAsBlank
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Indicates whether displaying N/A as blank value
type: docs
url: /net/aspose.cells.charts/chart/displaynaasblank/
---
## Chart.DisplayNaAsBlank property

Indicates whether displaying #N/A as blank value.

```csharp
public bool DisplayNaAsBlank { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(chart.DisplayNaAsBlank);
[Test]
        public void Property_DisplayNaAsBlank()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-47551.xlsx");
            Chart chart = workbook.Worksheets[0].Charts[0];
            Assert.IsTrue(chart.DisplayNaAsBlank);
            workbook.Save(Constants.destPath + "CELLSNET-47551.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET-47551.xlsx");
            chart = workbook.Worksheets[0].Charts[0];
            Assert.IsTrue(chart.DisplayNaAsBlank);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


