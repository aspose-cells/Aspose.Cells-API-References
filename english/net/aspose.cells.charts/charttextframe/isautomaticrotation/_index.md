---
title: ChartTextFrame.IsAutomaticRotation
second_title: Aspose.Cells for .NET API Reference
description: ChartTextFrame property. Indicates whether the text of the chart is automatically rotated
type: docs
url: /net/aspose.cells.charts/charttextframe/isautomaticrotation/
---
## ChartTextFrame.IsAutomaticRotation property

Indicates whether the text of the chart is automatically rotated.

```csharp
public bool IsAutomaticRotation { get; }
```

### Examples

```csharp
// Called: Assert.IsFalse(chart.ValueAxis.Title.IsAutomaticRotation);
[Test]
        public void Property_IsAutomaticRotation()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet52639.xlsx&quot;);
            var newWorkbook = new Workbook();
            newWorkbook.Copy(workbook);
            Chart chart = newWorkbook.Worksheets[0].Charts[0];
            Assert.IsFalse(chart.ValueAxis.Title.IsAutomaticRotation);

        }
```

### See Also

* class [ChartTextFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


