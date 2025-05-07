---
title: Legend.GetLegendLabels
second_title: Aspose.Cells for .NET API Reference
description: Legend method. Gets the labels of the legend entries after call Chart.Calculate method
type: docs
url: /net/aspose.cells.charts/legend/getlegendlabels/
---
## Legend.GetLegendLabels method

Gets the labels of the legend entries after call Chart.Calculate() method.

```csharp
public string[] GetLegendLabels()
```

### Examples

```csharp
// Called: Assert.AreEqual("NWC2 ", chart.Legend.GetLegendLabels()[8], "Legend label");
[Test]
        public void Method_GetLegendLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET-48580.xlsx");
            Chart chart = workbook.Worksheets[1].Charts[0];
            chart.Calculate();
            Assert.AreEqual("NWC2 ", chart.Legend.GetLegendLabels()[8], "Legend label");
        }
```

### See Also

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


