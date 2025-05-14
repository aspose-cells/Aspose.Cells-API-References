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
// Called: Assert.AreEqual("B2", range.GetOffset(1, 1).Address);
public void Range_Method_GetOffset()
{
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Aspose.Cells.Range range = cells.CreateRange("A1");
    Assert.AreEqual("A1", range.Address);
    Assert.AreEqual("B2", range.GetOffset(1, 1).Address);
    Assert.AreEqual("1:1", range.EntireRow.Address);
    Assert.AreEqual("A:A", range.EntireColumn.Address);
}
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


