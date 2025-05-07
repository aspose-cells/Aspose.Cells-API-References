---
title: Range.Item
second_title: Aspose.Cells for .NET API Reference
description: Range property. Gets Cell object in this range
type: docs
url: /net/aspose.cells/range/item/
---
## Range indexer

Gets [`Cell`](../../cell/) object in this range.

```csharp
public Cell this[int rowOffset, int columnOffset] { get; }
```

| Parameter | Description |
| --- | --- |
| rowOffset | Row offset in this range, zero based. |
| columnOffset | Column offset in this range, zero based. |

### Return Value

[`Cell`](../../cell/) object.

### Examples

```csharp
// Called: Assert.AreEqual(range[0,0].GetStyle().Borders[BorderType.TopBorder].LineStyle,CellBorderType.DashDot);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1:B3");
            range.SetOutlineBorder(BorderType.LeftBorder | BorderType.TopBorder,CellBorderType.DashDot,Color.Red);
            Assert.AreEqual(range[0,0].GetStyle().Borders[BorderType.LeftBorder].LineStyle,CellBorderType.DashDot);
            Assert.AreEqual(range[0,0].GetStyle().Borders[BorderType.TopBorder].LineStyle,CellBorderType.DashDot);

        }
```

### See Also

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


