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
// Called: Assert.AreEqual(workbook2.Worksheets[0].SparklineGroups.Count, 1);
[Test]
        public void Property_SparklineGroups()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet41009.xlsx");
            Workbook workbook2 = new Workbook();
            workbook2.Copy(workbook);
            Assert.AreEqual(workbook2.Worksheets[0].SparklineGroups.Count, 1);
        }
```

### See Also

* class [SparklineGroupCollection](../../../aspose.cells.charts/sparklinegroupcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


