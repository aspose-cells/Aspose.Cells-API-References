---
title: Chart.Name
second_title: Aspose.Cells for .NET API Reference
description: Chart property. Gets and sets the name of the chart
type: docs
url: /net/aspose.cells.charts/chart/name/
---
## Chart.Name property

Gets and sets the name of the chart.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: Console.WriteLine(workbook.Worksheets[0].Charts[0].Name);
public void Chart_Property_Name()
{
    var workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Console.WriteLine(workbook.Worksheets[0].Charts[0].Name);
    Console.WriteLine(workbook.Worksheets[0].Charts[1].Name);

    workbook.Worksheets[0].Charts.Add(Aspose.Cells.Charts.ChartType.Column, 25, 0, 40, 5);

    Assert.AreEqual(workbook.Worksheets[0].Charts[2].Name, "Chart 2");
}
```

### See Also

* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


