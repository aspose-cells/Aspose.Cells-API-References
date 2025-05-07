---
title: Chart.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the worksheet which contains this chart
type: docs
url: /net/aspose.cells.charts/chart/worksheet/
---
## Chart.Worksheet property

Gets the worksheet which contains this chart.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.Worksheet.Index, 0);//CELLSJAVA-41019
[Test]
        public void Property_Worksheet()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET43013.xls");
            Chart chart = workbook.Worksheets[0].Charts[6];
            Assert.AreEqual(chart.Worksheet.Index, 0);//CELLSJAVA-41019
            Assert.AreEqual(chart.NSeries[3].Area.FillFormat.FillType, FillType.Pattern);
            Assert.AreEqual(chart.NSeries[3].Area.FillFormat.PatternFill.Pattern, FillPattern.WideDownwardDiagonal);
        }
```

### See Also

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


