---
title: Axis.Title
second_title: Aspose.Cells for .NET API Reference
description: Axis property. Gets the axis title
type: docs
url: /net/aspose.cells.charts/axis/title/
---
## Axis.Title property

Gets the axis' title.

```csharp
public Title Title { get; }
```

### Examples

```csharp
// Called: chart.CategoryAxis.Title.Font.Name = "Arial";
public void Axis_Property_Title()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    for (int chartIndex = 0; chartIndex < workbook.Worksheets[0].Charts.Count; chartIndex++)
    {
        Chart chart = workbook.Worksheets[0].Charts[chartIndex];
        chart.Title.IsVisible = true;
        chart.CategoryAxis.Title.IsVisible = true;
        chart.ValueAxis.Title.IsVisible = true;
        chart.CategoryAxis.Title.Font.Name = "Arial";
        chart.ValueAxis.Title.Font.Name = "Aktiv Grotesk";
        chart.Title.Font.Name = "Aktiv Grotesk";
    }

    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(workbook.FileName);
    for (int chartIndex = 0; chartIndex < workbook.Worksheets[0].Charts.Count; chartIndex++)
    {
        Chart chart = workbook.Worksheets[0].Charts[chartIndex];
        Assert.AreEqual("Arial", chart.CategoryAxis.Title.Font.Name, "CategoryAxis Title Font Name");
        Assert.AreEqual("Aktiv Grotesk", chart.ValueAxis.Title.Font.Name, "ValueAxis Title Font Name");
        Assert.AreEqual("Aktiv Grotesk", chart.Title.Font.Name, "Chart Title Font Name");
    }

}
```

### See Also

* class [Title](../../title/)
* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


