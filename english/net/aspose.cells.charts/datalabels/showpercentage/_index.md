---
title: DataLabels.ShowPercentage
second_title: Aspose.Cells for .NET API Reference
description: DataLabels property. Represents a specified charts data label percentage value display behavior. True displays the percentage value. False to hide
type: docs
url: /net/aspose.cells.charts/datalabels/showpercentage/
---
## DataLabels.ShowPercentage property

Represents a specified chart's data label percentage value display behavior. True displays the percentage value. False to hide.

```csharp
public bool ShowPercentage { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(chart.NSeries[0].Points[3].DataLabels.ShowPercentage, true);
public void DataLabels_Property_ShowPercentage()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlt");
    Chart chart = workbook.Worksheets[0].Charts[1];
    Aspose.Cells.Cells cells = workbook.Worksheets[0].Cells;
    cells["C32"].PutValue(1);
    cells["C33"].PutValue(1);
    Assert.AreEqual(chart.NSeries[0].Points[3].DataLabels.ShowPercentage, true);
    workbook.Save(Constants.destPath + "example.xls");
}
```

### See Also

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


