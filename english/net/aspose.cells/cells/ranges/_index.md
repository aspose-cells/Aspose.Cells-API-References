---
title: Cells.Ranges
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the collection of Range objects created at run time
type: docs
url: /net/aspose.cells/cells/ranges/
---
## Cells.Ranges property

Gets the collection of [`Range`](../../range/) objects created at run time.

```csharp
public RangeCollection Ranges { get; }
```

### Examples

```csharp
// Called: worksheet.Cells.Ranges.Add(cellRange);
[Test]
        public void Property_Ranges()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Aspose.Cells.Range cellRange = worksheet.Cells.CreateRange(0, 0, 3, 1);
            worksheet.Cells.Ranges.Add(cellRange);
            worksheet.Cells.InsertRows(2, 2, true);
            Assert.AreEqual(5, cellRange.RowCount);
        }
```

### See Also

* class [RangeCollection](../../rangecollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


