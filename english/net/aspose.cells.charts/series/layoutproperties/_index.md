---
title: Series.LayoutProperties
second_title: Aspose.Cells for .NET API Reference
description: Series property. Represents the properties of layout
type: docs
url: /net/aspose.cells.charts/series/layoutproperties/
---
## Series.LayoutProperties property

Represents the properties of layout.

```csharp
public SeriesLayoutProperties LayoutProperties { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(3, chart.NSeries[0].LayoutProperties.Subtotals[1]);
[Test]
        public void Property_LayoutProperties()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava43271.xlsx");
            Worksheet sheet = workbook.Worksheets[0];
            sheet.Cells.DeleteRow(5); // this is critical
            Chart chart = sheet.Charts[0];
            Assert.AreEqual(0, chart.NSeries[0].LayoutProperties.Subtotals[0]);
            Assert.AreEqual(3, chart.NSeries[0].LayoutProperties.Subtotals[1]);
            workbook.Save(Constants.destPath + "CellsJava43271.xlsx");
        }
```

### See Also

* class [SeriesLayoutProperties](../../serieslayoutproperties/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


