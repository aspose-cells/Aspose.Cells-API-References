---
title: Chart.Legend
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the chart legend
type: docs
url: /net/aspose.cells.charts/chart/legend/
---
## Chart.Legend property

Gets the chart legend.

```csharp
public Legend Legend { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[1].Charts[0].Legend.IsAutomaticSize, false);
public void Chart_Property_Legend()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    workbook.Save(Constants.destPath + "example.xls");
    workbook = new Workbook(Constants.destPath + "example.xls");
    Assert.AreEqual(workbook.Worksheets[1].Charts[0].Legend.IsAutomaticSize, false);
}
```

### See Also

* class [Legend](../../legend/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


