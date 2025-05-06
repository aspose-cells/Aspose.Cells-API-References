---
title: SeriesLayoutProperties.Subtotals
second_title: Aspose.Cells for .NET API Reference
description: SeriesLayoutProperties property. Represents the index of a subtotal data point
type: docs
url: /net/aspose.cells.charts/serieslayoutproperties/subtotals/
---
## SeriesLayoutProperties.Subtotals property

Represents the index of a subtotal data point.

```csharp
public int[] Subtotals { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, chart.NSeries[0].LayoutProperties.Subtotals[1]);
[Test]
        public void Property_Subtotals()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava43271.xlsx&quot;);
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells.DeleteRow(5); // this is critical
            Chart chart = sheet.Charts[0];
            Assert.AreEqual(0, chart.NSeries[0].LayoutProperties.Subtotals[0]);
            Assert.AreEqual(3, chart.NSeries[0].LayoutProperties.Subtotals[1]);
            workbook.Save(Constants.destPath + &quot;CellsJava43271.xlsx&quot;);
        }
```

### See Also

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


