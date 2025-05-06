---
title: Chart.SwitchRowColumn
second_title: Aspose.Cells for .NET API Reference
description: Chart method. Switches row/column
type: docs
url: /net/aspose.cells.charts/chart/switchrowcolumn/
---
## Chart.SwitchRowColumn method

Switches row/column.

```csharp
public bool SwitchRowColumn()
```

### Return Value

False means switching row/column fails.

### Examples

```csharp
// Called: chart.SwitchRowColumn();
[Test]
        public void Method_SwitchRowColumn()
        {
            //=Sheet1!$A$1:$D$4
            //=Sheet1!$B$2:$D$2
            // = Sheet1!$A$1:$D$4
            //  = Sheet1!$B$2:$B$4
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET47806_40624.xlsx&quot;);

            Chart chart = workbook.Worksheets[0].Charts[0];

            String str = chart.GetChartDataRange();

            Assert.AreEqual(&quot;=Sheet1!$A$1:$D$4&quot;, str);
            Assert.AreEqual(&quot;=Sheet1!$B$2:$D$2&quot;, chart.NSeries[0].Values);


            chart.SwitchRowColumn();

            Assert.AreEqual(&quot;=Sheet1!$A$1:$D$4&quot;, str);
            Assert.AreEqual(&quot;=Sheet1!$B$2:$B$4&quot;, chart.NSeries[0].Values);
            workbook.Save(Constants.destPath + &quot;CELLSNET47806_40624.xlsx&quot;);
        }
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


