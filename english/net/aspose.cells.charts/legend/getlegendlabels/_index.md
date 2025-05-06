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
// Called: string[] _legendLabels = _legend.GetLegendLabels();
[Test]
        public void Method_GetLegendLabels()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;Charts/ChartAPI/CELLSJAVA-42410.xlsx&quot;);
            Chart chart = workbook.Worksheets[0].Charts[0];
            chart.Calculate();
            Legend _legend = chart.Legend;

            string[] _legendLabels = _legend.GetLegendLabels();
            Assert.AreEqual(2, _legendLabels.Length);
            Assert.AreEqual(&quot;12m forward dividend yield (LHS)&quot;, _legendLabels[0]);
            Assert.AreEqual(&quot;Dividend cover (RHS)&quot;, _legendLabels[1]);
        }
```

### See Also

* class [Legend](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


