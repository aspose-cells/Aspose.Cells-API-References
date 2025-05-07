---
title: Range.UnMerge
second_title: Aspose.Cells for .NET API Reference
description: Range method. Unmerges merged cells of this range
type: docs
url: /net/aspose.cells/range/unmerge/
---
## Range.UnMerge method

Unmerges merged cells of this range.

```csharp
public void UnMerge()
```

### Examples

```csharp
// Called: selectedRange.UnMerge();
[Test]
        public void Method_UnMerge()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "Gics.xls");
            Aspose.Cells.Range selectedRange = workbook.Worksheets.GetRangeByName("Report_Title");
            selectedRange.UnMerge();
            Aspose.Cells.Cell cell = workbook.Worksheets[0].Cells["B10"];
            Assert.IsFalse(cell.IsMerged);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


