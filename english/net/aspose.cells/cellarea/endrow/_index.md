---
title: CellArea.EndRow
second_title: Aspose.Cells for .NET API Reference
description: CellArea field. Gets or set the end row of this area
type: docs
url: /net/aspose.cells/cellarea/endrow/
---
## CellArea.EndRow field

Gets or set the end row of this area.

```csharp
public int EndRow;
```

### Examples

```csharp
// Called: CellsHelper.CellNameToIndex(strCellRange[1], out area.EndRow, out column);
public CellArea Field_EndRow(string s)
        {
            CellArea area = new CellArea();
            string[] strCellRange = s.Replace(&quot;$&quot;, &quot;&quot;).Split(&apos;:&apos;);
            int column;
            CellsHelper.CellNameToIndex(strCellRange[0], out area.StartRow, out column);
            area.StartColumn = column;
            if (strCellRange.Length == 1)
            {
                area.EndRow = area.StartRow;
                area.EndColumn = area.StartColumn;
            }
            else
            {
                CellsHelper.CellNameToIndex(strCellRange[1], out area.EndRow, out column);
                area.EndColumn = column;
            }
            return area;
        }
```

### See Also

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


