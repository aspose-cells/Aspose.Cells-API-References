---
title: Cell.Column
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets column number zero based of the cell
type: docs
url: /net/aspose.cells/cell/column/
---
## Cell.Column property

Gets column number (zero based) of the cell.

```csharp
public int Column { get; }
```

### Examples

```csharp
// Called: if (cell.Row != sn || cell.Column != sn)
private void Cell_Property_Column(Workbook wb, string info, int styleCount)
        {
            IEnumerator enCell = wb.Worksheets[0].Cells.GetEnumerator();
            int sn = 0;
            while (enCell.MoveNext())
            {
                Cell cell = (Cell)enCell.Current;
                if (cell.Row != sn || cell.Column != sn)
                {
                    Assert.Fail(info + "Extra cell-" + cell.Name);
                }
                StyleProcessCell(cell, false, info);
                sn++;
            }
            if (wb.CountOfStylesInPool > styleCount)
            {
                Assert.Fail(info + "Extra styles, original count is " + styleCount + ", current is " + wb.CountOfStylesInPool);
            }
            //check string pool in debug mode here.
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


