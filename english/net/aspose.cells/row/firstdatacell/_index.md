---
title: Row.FirstDataCell
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the first nonblank cell in the row
type: docs
url: /net/aspose.cells/row/firstdatacell/
---
## Row.FirstDataCell property

Gets the first non-blank cell in the row.

```csharp
public Cell FirstDataCell { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(cells["B2"], cells.Rows[1].FirstDataCell);
[Test]
        public void Property_FirstDataCell()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells["B2"].PutValue("sdfsdf");
            Assert.AreEqual(cells["B2"], cells.Rows[1].FirstDataCell);
        }
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


