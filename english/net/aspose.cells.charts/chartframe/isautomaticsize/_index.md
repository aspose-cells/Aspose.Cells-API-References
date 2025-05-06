---
title: ChartFrame.IsAutomaticSize
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Indicates whether the chart frame is automatic sized
type: docs
url: /net/aspose.cells.charts/chartframe/isautomaticsize/
---
## ChartFrame.IsAutomaticSize property

Indicates whether the chart frame is automatic sized.

```csharp
public virtual bool IsAutomaticSize { get; set; }
```

### Examples

```csharp
// Called: Assert.IsFalse(chart.NSeries[0].Points[0].DataLabels.IsAutomaticSize);
[Test]
        public void Property_IsAutomaticSize()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET46963.xlsx&quot;);
            Chart chart = wb.Worksheets[&quot;Composition of revenues&quot;].Charts[1];
            Assert.IsFalse(chart.NSeries[0].Points[0].DataLabels.IsAutomaticSize);

            wb.Save(Constants.destPath + &quot;CELLSNET46963.xlsx&quot;);

            wb = new Workbook(Constants.destPath + &quot;CELLSNET46963.xlsx&quot;);
            chart = wb.Worksheets[&quot;Composition of revenues&quot;].Charts[1];
            Assert.IsFalse(chart.NSeries[0].Points[0].DataLabels.IsAutomaticSize);

            wb.Save(Constants.destPath + &quot;CELLSNET46963.xlsx&quot;);
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


