---
title: CellArea.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the end column of this area
type: docs
url: /net/aspose.cells/cellarea/endcolumn/
---
## CellArea.EndColumn field

Gets or set the end column of this area.

```csharp
public int EndColumn;
```

### Examples

```csharp
// Called: for (int i = area.StartColumn; i <= area.EndColumn; i++)
private void CellArea_Field_EndColumn(string cellAreaName, Color color, Worksheet _sheet)
        {
            CellArea area = GetCellAreaByName(cellAreaName);
            int k = 0;
            for (int i = area.StartColumn; i <= area.EndColumn; i++)
            {
                for (int j = area.StartRow; j <= area.EndRow; j++)
                {
                    Cell c = _sheet.Cells[j, i];
                    if (!color.IsEmpty)
                    {

                        Style s = c.GetStyle();
                        s.ForegroundColor = color;
                        s.Pattern = BackgroundType.Solid;
                        c.SetStyle(s);
                    }
                    //Set some random values to the cells in the cellarea range
                    int value = j + i + k;
                    c.PutValue(value);
                    k++;
                }
            }

        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


