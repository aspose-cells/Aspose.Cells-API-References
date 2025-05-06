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
// Called: Assert.IsTrue(destRange[0, 0].GetStyle().Font.IsBold);
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet44456_SourceVar.xlsx&quot;);
            string sourcefileName = Constants.sourcePath  + &quot;CellsNet44456_SourceVar.xlsx&quot;;
            string destfileName = Constants.sourcePath  + &quot;CellsNet44456_DestVar.xlsx&quot;;

            var sourceWorkbook = new Workbook(sourcefileName);
            var destWorkbook = new Workbook(destfileName);

            var destRange = destWorkbook.Worksheets[&quot;Sheet1&quot;].Cells.CreateRange(&quot;A1&quot;, &quot;C2&quot;);
            var sourceRange = sourceWorkbook.Worksheets[&quot;Sheet1&quot;].Cells.CreateRange(&quot;A5&quot;, &quot;C6&quot;);

            destWorkbook.Worksheets[&quot;Sheet1&quot;].Cells.ClearContents(destRange.FirstRow, destRange.FirstColumn,
                                                            destRange.FirstRow + destRange.RowCount - 1,
                                                           destRange.FirstColumn + destRange.ColumnCount - 1);

            destRange.CopyData(sourceRange);
            Assert.IsTrue(destRange[0, 0].GetStyle().Font.IsBold);
            destWorkbook.Save(Constants.destPath + &quot;dest.xlsx&quot;);
        }
```

### See Also

* class [Cell](../../cell/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


