---
title: Range.GetOffset
second_title: Aspose.Cells for .NET API Reference
description: Range method. Gets Range range by offset
type: docs
url: /net/aspose.cells/range/getoffset/
---
## Range.GetOffset method

Gets [`Range`](../) range by offset.

```csharp
public Range GetOffset(int rowOffset, int columnOffset)
```

| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | Int32 | Row offset in this range, zero based. |
| columnOffset | Int32 | Column offset in this range, zero based. |

### Examples

```csharp
// Called: Assert.AreEqual(&amp;quot;B2&amp;quot;, range.GetOffset(1, 1).Address);
[Test]
        public void Method_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange(&quot;A1&quot;);
            Assert.AreEqual(&quot;A1&quot;, range.Address);
            Assert.AreEqual(&quot;B2&quot;, range.GetOffset(1, 1).Address);
            Assert.AreEqual(&quot;1:1&quot;, range.EntireRow.Address);
            Assert.AreEqual(&quot;A:A&quot;, range.EntireColumn.Address);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


