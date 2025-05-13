---
title: Sparkline.DataRange
second_title: Aspose.Cells for .NET API Reference
description: Sparkline property. Represents the data range of the sparkline
type: docs
url: /net/aspose.cells.charts/sparkline/datarange/
---
## Sparkline.DataRange property

Represents the data range of the sparkline.

```csharp
public string DataRange { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook2.Worksheets[1].SparklineGroups[0].SparklineCollection[0].DataRange, "Sheet2!A2:D2");
public void Sparkline_Property_DataRange()
{
    Workbook workbook1 = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook workbook2 = new Workbook();

    workbook2.Combine(workbook1);
    Assert.AreEqual(workbook2.Worksheets[1].SparklineGroups[0].SparklineCollection[0].DataRange, "Sheet2!A2:D2");
}
```

### See Also

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


