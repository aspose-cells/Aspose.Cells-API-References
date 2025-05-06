---
title: SparklineGroup.Type
second_title: Aspose.Cells for .NET API Reference
description: SparklineGroup property. Indicates the sparkline type of the sparkline group
type: docs
url: /net/aspose.cells.charts/sparklinegroup/type/
---
## SparklineGroup.Type property

Indicates the sparkline type of the sparkline group.

```csharp
public SparklineType Type { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(SparklineType.Column,sparklineGroups[1].Type);
[Test]
        public void Property_Type()
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

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


