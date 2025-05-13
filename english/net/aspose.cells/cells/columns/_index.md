---
title: Cells.Columns
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the collection of Column objects that represents the individual columns in this worksheet
type: docs
url: /net/aspose.cells/cells/columns/
---
## Cells.Columns property

Gets the collection of [`Column`](../../column/) objects that represents the individual columns in this worksheet.

```csharp
public ColumnCollection Columns { get; }
```

### Examples

```csharp
// Called: checkColumnStyle(cells.Columns[5].GetStyle());
private void Cells_Property_Columns(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            checkRangeStyle(cells);
            checkRowStyle(cells.Rows[7].GetStyle());
            checkColumnStyle(cells.Columns[5].GetStyle());
            checkColumnStyle(cells[8, 6].GetStyle());
            checkColumnStyle(cells[8, 7].GetStyle());
            checkColumnStyle(cells[9, 6].GetStyle());
            checkColumnStyle(cells[9, 7].GetStyle());
        }
```

### See Also

* class [ColumnCollection](../../columncollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


