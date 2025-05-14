---
title: SparklineGroup.SparklineCollection
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets the collection of Sparkline object
type: docs
url: /net/aspose.cells.charts/sparklinegroup/sparklinecollection/
---
## SparklineGroup.SparklineCollection property

Gets the collection of [`Sparkline`](../../sparkline/) object.

```csharp
[Obsolete("Use SparklineGroup.Sparklines property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SparklineCollection SparklineCollection { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use SparklineGroup.Sparklines property. This property will be removed 12 months later since November 2022. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: workbook.Worksheets[0].SparklineGroups[0].SparklineCollection.Add("E6:P6", 5, 16);
public void SparklineGroup_Property_SparklineCollection()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    workbook.Worksheets[0].SparklineGroups[0].SparklineCollection.Add("E6:P6", 5, 16);
    workbook.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


