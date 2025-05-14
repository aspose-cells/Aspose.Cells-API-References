---
title: Chart.Title
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets the charts title
type: docs
url: /net/aspose.cells.charts/chart/title/
---
## Chart.Title property

Gets the chart's title.

```csharp
public Title Title { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("It is the title of the graph", chart.Title.Text);
public void Chart_Property_Title()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xls");
    Chart chart = workbook.Worksheets[0].Charts[0];
    Assert.AreEqual("It is the title of the graph", chart.Title.Text);
           
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [Title](../../title/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


