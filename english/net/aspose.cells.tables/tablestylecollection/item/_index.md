---
title: TableStyleCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: TableStyleCollection property. Gets the table style by the index
type: docs
url: /net/aspose.cells.tables/tablestylecollection/item/
---
## TableStyleCollection indexer (1 of 2)

Gets the table style by the index.

```csharp
public TableStyle this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The position of the table style in the list. |

### Return Value

The table style object.

### Examples

```csharp
// Called: TableStyle style = workbook.Worksheets.TableStyles[0];
[Test]
        public void Property_Int32_()
        {
            //-2171174
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet45252.xls");
            TableStyle style = workbook.Worksheets.TableStyles[0];
            Style eStyle = style.TableStyleElements[TableStyleElementType.WholeTable].GetElementStyle();
            Assert.AreEqual(eStyle.Borders[BorderType.Horizontal].Color.ToArgb(), -2171174);
            Assert.AreEqual(eStyle.Borders[BorderType.Horizontal].LineStyle, CellBorderType.Medium);
            workbook.Save(Constants.destPath + "CellsNet45252.xlsx");
        }
```

### See Also

* class [TableStyle](../../tablestyle/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)

---

## TableStyleCollection indexer (2 of 2)

Gets the table style by the name.

```csharp
public TableStyle this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The table style name. |

### Return Value

The table style object.

### See Also

* class [TableStyle](../../tablestyle/)
* class [TableStyleCollection](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


