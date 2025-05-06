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
// Called: r.UnMerge();
[Test]
        public void Method_UnMerge()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Cells.Merge(3, 3, 3, 3);
            Aspose.Cells.Range r = workbook.Worksheets[0].Cells.MaxDisplayRange;
            r.UnMerge();
            Assert.AreEqual(0, workbook.Worksheets[0].Cells.GetMergedAreas().Length);
        }
```

### See Also

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


