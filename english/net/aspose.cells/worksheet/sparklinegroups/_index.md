---
title: Worksheet.SparklineGroups
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the sparkline groups in the worksheet
type: docs
url: /net/aspose.cells/worksheet/sparklinegroups/
---
## Worksheet.SparklineGroups property

Gets the sparkline groups in the worksheet.

```csharp
public SparklineGroupCollection SparklineGroups { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].SparklineGroups.Count, 1);
public void Worksheet_Property_SparklineGroups()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsb");
    Assert.AreEqual(workbook.Worksheets[0].SparklineGroups.Count, 1);
    workbook.Save(Constants.destPath + "example.xlsb");
    workbook = new Workbook(Constants.destPath + "example.xlsb");
    Assert.AreEqual(workbook.Worksheets[0].SparklineGroups.Count, 1);
}
```

### See Also

* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


