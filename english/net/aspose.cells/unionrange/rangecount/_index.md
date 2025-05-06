---
title: UnionRange.RangeCount
second_title: Aspose.Cells for .NET API Reference
description: UnionRange property. Gets the count of the ranges
type: docs
url: /net/aspose.cells/unionrange/rangecount/
---
## UnionRange.RangeCount property

Gets the count of the ranges.

```csharp
public int RangeCount { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(r.RangeCount, 2);
[Test]
        public void Property_RangeCount()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range t = cells.CreateRange(&quot;B1:C10&quot;);
            UnionRange r = t.UnionRanges(new Aspose.Cells.Range[] { cells.CreateRange(&quot;C2:D10&quot;) });
            Assert.AreEqual(r.RangeCount, 2);
        }
```

### See Also

* class [UnionRange](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


