---
title: Row.Item
second_title: Aspose.Cells for .NET API Reference
description: Row property. Gets the cell
type: docs
url: /net/aspose.cells/row/item/
---
## Row indexer

Gets the cell.

```csharp
public Cell this[int column] { get; }
```

| Parameter | Description |
| --- | --- |
| column | The column index |

### Examples

```csharp
// Called: row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
[Test]
        public void Property_Int32_()
        {
            var xls = new Workbook();
            var sheet = xls.Worksheets[0];
            var row = sheet.Cells.Rows[0];
            row[0].HtmlString = @"<span style=""color:#ffAb68;"">TEST</span>";
            row[1].HtmlString = @"<span style=""color:inherit;"">TEST</span>";
            Assert.AreEqual("ffffab68", row[0].GetStyle().Font.Color.Name);
            Assert.AreEqual("ff000000", row[1].GetStyle().Font.Color.Name);
        }
```

### See Also

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


