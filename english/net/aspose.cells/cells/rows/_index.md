---
title: Cells.Rows
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets the collection of Row objects that represents the individual rows in this worksheet
type: docs
url: /net/aspose.cells/cells/rows/
---
## Cells.Rows property

Gets the collection of [`Row`](../../row/) objects that represents the individual rows in this worksheet.

```csharp
public RowCollection Rows { get; }
```

### Examples

```csharp
// Called: checkRowStyle(cells.Rows[7].GetStyle());
private void Property_Rows(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            checkRangeStyle(cells);
            checkRowStyle(cells.Rows[7].GetStyle());
            checkColumnStyle(cells.Columns[5].GetStyle());
            checkColumnStyle(cells[6, 6].GetStyle());
            checkColumnStyle(cells[6, 7].GetStyle());
        }
```

### See Also

* class [RowCollection](../../rowcollection/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


