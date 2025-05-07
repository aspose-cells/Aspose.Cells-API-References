---
title: HorizontalPageBreak.Row
second_title: Aspose.Cells for .NET API Reference
description: HorizontalPageBreak property. Gets the zero based row index
type: docs
url: /net/aspose.cells/horizontalpagebreak/row/
---
## HorizontalPageBreak.Row property

Gets the zero based row index.

```csharp
public int Row { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[0].HorizontalPageBreaks[0].Row, 3);
[Test]
        public void Property_Row()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].HorizontalPageBreaks.Add(5, 5);
            Cells cells = workbook.Worksheets[0].Cells;
            cells.DeleteRows(0, 2);
            Assert.AreEqual(workbook.Worksheets[0].HorizontalPageBreaks[0].Row, 3);

        }
```

### See Also

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


