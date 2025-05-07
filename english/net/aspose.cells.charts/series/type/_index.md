---
title: Series.Type
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets or sets a data series type
type: docs
url: /net/aspose.cells.charts/series/type/
---
## Series.Type property

Gets or sets a data series' type.

```csharp
public ChartType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(ChartType.Line, chart.NSeries[0].Type);
[Test]
        public void Property_Type()
        {

            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSJAVA42786.ods");
            Chart chart = workbook.Worksheets[1].Charts[0];
            Assert.AreEqual(ChartType.Line, chart.NSeries[0].Type);
            Assert.AreEqual("=Tabellen!$A$21:$A$34", chart.NSeries.CategoryData);
            Assert.AreEqual("=Tabellen!$C$21:$C$34", chart.NSeries[0].Values);
            Assert.AreEqual("=Tabellen!$C$20", chart.NSeries[0].Name);
            workbook.Save(Constants.destPath + "CELLSJAVA42789.xlsx");


        }
```

### See Also

* enum [ChartType](../../charttype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


