---
title: SparklineCollection.Add
second_title: Aspose.Cells for .NET API Reference
description: SparklineCollection method. Add a sparkline
type: docs
url: /net/aspose.cells.charts/sparklinecollection/add/
---
## SparklineCollection.Add method

Add a sparkline.

```csharp
public int Add(string dataRange, int row, int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| dataRange | String | Specifies the new data range of the sparkline. |
| row | Int32 | The row index of the location. |
| column | Int32 | The column index of the location. |

### Examples

```csharp
// Called: int index = group.Sparklines.Add("D5:O5", 4, 15);
public void SparklineCollection_Method_Add()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    // Access first worksheet
    Worksheet worksheet = workbook.Worksheets[0];

    // Access the first sparkline group
    SparklineGroup group = worksheet.SparklineGroups[0];

    // Add Data Ranges and Locations inside this sparkline group
    int index = group.Sparklines.Add("D5:O5", 4, 15);
    Assert.AreEqual("Sheet1!D5:O5", group.Sparklines[index].DataRange);
    //group.Sparklines.Add("D6:O6", 5, 15);
    //group.Sparklines.Add("D7:O7", 6, 15);
    //group.Sparklines.Add("D8:O8", 7, 15);

    // Save the workbook
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    group = worksheet.SparklineGroups[0];
    Assert.AreEqual(PlotEmptyCellsType.NotPlotted, group.PlotEmptyCellsType);
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    group = worksheet.SparklineGroups[0];
    Assert.AreEqual(PlotEmptyCellsType.NotPlotted, group.PlotEmptyCellsType);
}
```

### See Also

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


