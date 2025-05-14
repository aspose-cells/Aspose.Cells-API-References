---
title: Series.DisplayName
second_title: Aspose.Cells for .NET API Reference
description: Series property. Gets the seriess name that displays on the chart graph
type: docs
url: /net/aspose.cells.charts/series/displayname/
---
## Series.DisplayName property

Gets the series's name that displays on the chart graph.

```csharp
public string DisplayName { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual("Prix départ", chart.NSeries[0].DisplayName);
public void Series_Property_DisplayName()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.numbers");
    //wb.Save(Constants.destPath + @"example.xlsx");
    wb = Util.ReSave(wb, SaveFormat.Xlsx);
    Chart chart = wb.Worksheets["Depart"].Charts[0];
    Assert.AreEqual(1, chart.NSeries.Count);
    Assert.AreEqual("=Depart!$D$1", chart.NSeries[0].Name);
    Assert.AreEqual("Prix départ", chart.NSeries[0].DisplayName);
    Assert.AreEqual("=(Depart!$B$7,Depart!$B$3,Depart!$B$4,Depart!$B$2,Depart!$B$6,Depart!$B$5,Depart!$B$22,Depart!$A$9:$B$9,Depart!$B$8)", chart.NSeries.CategoryData);
}
```

### See Also

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


