---
title: Row.LastDataCell
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the last nonblank cell in the row
type: docs
url: /net/aspose.cells/row/lastdatacell/
---
## Row.LastDataCell property

Gets the last non-blank cell in the row.

```csharp
public Cell LastDataCell { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(cells.Rows[0].LastDataCell.Name, &amp;quot;A1&amp;quot;);
[Test]
        public void Property_LastDataCell()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            cells[&quot;A1&quot;].PutValue(&quot;1&quot;);
            Cell cell = cells[&quot;A2&quot;];
            Assert.AreEqual(cells.Rows[0].LastDataCell.Name, &quot;A1&quot;);
        }
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


