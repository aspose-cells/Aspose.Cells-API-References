---
title: FormatCondition.AboveAverage
second_title: Aspose.Cells for .NET API Reference
description: FormatCondition property. Get the conditional formattings AboveAverage instance. The default instances rule highlights cells that are above the average for all values in the range. Valid only for type  AboveAverage
type: docs
url: /net/aspose.cells/formatcondition/aboveaverage/
---
## FormatCondition.AboveAverage property

Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage.

```csharp
public AboveAverage AboveAverage { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(cfs[2][0].AboveAverage.IsAboveAverage);
[Test]
        public void Property_AboveAverage()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;ConditionalFormattings/CELLSNET47107.xlsx&quot;);
            ConditionalFormattingCollection cfs = workbook.Worksheets[0].ConditionalFormattings;
            Assert.IsTrue(cfs[0][0].AboveAverage.IsAboveAverage);
            Assert.IsFalse(cfs[1][0].AboveAverage.IsAboveAverage);
            Assert.IsTrue(cfs[2][0].AboveAverage.IsAboveAverage);
            Assert.IsFalse(cfs[3][0].AboveAverage.IsAboveAverage);
            workbook.Save(Constants.destPath + &quot;CELLSNET47107.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET47107.xlsx&quot;);
            cfs = workbook.Worksheets[0].ConditionalFormattings;
            Assert.IsTrue(cfs[0][0].AboveAverage.IsAboveAverage);
            Assert.IsFalse(cfs[1][0].AboveAverage.IsAboveAverage);
            Assert.IsTrue(cfs[2][0].AboveAverage.IsAboveAverage);
            Assert.IsFalse(cfs[3][0].AboveAverage.IsAboveAverage);
        }
```

### See Also

* class [AboveAverage](../../aboveaverage/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


