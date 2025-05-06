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
// Called: Assert.AreEqual(workbook2.Worksheets[1].SparklineGroups[0].SparklineCollection[0].DataRange, &amp;quot;Sheet2!A2:D2&amp;quot;);
[Test]
        public void Property_SparklineCollection()
        {
            Workbook workbook1 = new Workbook(Constants.sourcePath + &quot;CELLSJAVA41018.xlsx&quot;);
            Workbook workbook2 = new Workbook();

            workbook2.Combine(workbook1);
            Assert.AreEqual(workbook2.Worksheets[1].SparklineGroups[0].SparklineCollection[0].DataRange, &quot;Sheet2!A2:D2&quot;);
        }
```

### See Also

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


