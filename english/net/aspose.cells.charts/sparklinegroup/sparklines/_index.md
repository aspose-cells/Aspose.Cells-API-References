---
title: SparklineGroup.Sparklines
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Gets the collection of Sparkline object
type: docs
url: /net/aspose.cells.charts/sparklinegroup/sparklines/
---
## SparklineGroup.Sparklines property

Gets the collection of [`Sparkline`](../../sparkline/) object.

```csharp
public SparklineCollection Sparklines { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;Sheet1!A1:D1&amp;quot;, sparklineGroups[0].Sparklines[0].DataRange);
[Test]
        public void Property_Sparklines()
        {
            Workbook source = new Workbook(Constants.sourcePath + &quot;CELLSNET53115.xlsx&quot;);


            source.Save(Constants.destPath + &quot;CELLSNET53115.ods&quot;);
            source = new Workbook(Constants.destPath + &quot;CELLSNET53115.ods&quot;);
            SparklineGroupCollection sparklineGroups = source.Worksheets[0].SparklineGroups;
            Assert.AreEqual(3, sparklineGroups.Count);
            Assert.AreEqual(SparklineType.Line, sparklineGroups[0].Type);
            Assert.AreEqual(&quot;Sheet1!A1:D1&quot;, sparklineGroups[0].Sparklines[0].DataRange);
            Assert.AreEqual(SparklineType.Column,sparklineGroups[1].Type);
            Assert.AreEqual(SparklineType.Stacked, sparklineGroups[2].Type);
            source.Save(Constants.destPath + &quot;CELLSNET53115.xlsx&quot;);
        }
```

### See Also

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


