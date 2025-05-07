---
title: CellArea.StartColumn
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the start column of this area
type: docs
url: /net/aspose.cells/cellarea/startcolumn/
---
## CellArea.StartColumn field

Gets or set the start column of this area.

```csharp
public int StartColumn;
```

### Examples

```csharp
// Called: for (int col = ca.StartColumn; col <= ca.EndColumn; col++)
public static void Field_StartColumn(CellValueType[] types, string[] vals, Cells cells, CellArea ca, string msgHeader)
        {
            int pos = 0;
            for (int row = ca.StartRow; row <= ca.EndRow; row++)
            {
                for (int col = ca.StartColumn; col <= ca.EndColumn; col++)
                {
                    Cell cell = cells[row, col];
                    if (types[pos] != cell.Type || vals[pos] != cell.StringValue)
                    {
                        Cell c = cells[row, col];
                        Assert.Fail((string.IsNullOrEmpty(msgHeader) ? "" : msgHeader + ": ")
                        + c.Formula + " at " + c.Name + " - expected " + vals[pos]
                        + "(" + types[pos] + ") but was " + c.StringValue + "(" + cell.Type + ")");
                    }
                    pos++;
                }
            }
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


