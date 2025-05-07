---
title: ReferredArea.EndColumn
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. The end column of the area
type: docs
url: /net/aspose.cells/referredarea/endcolumn/
---
## ReferredArea.EndColumn property

The end column of the area.

```csharp
public int EndColumn { get; }
```

### Examples

```csharp
// Called: && rd.EndRow - rd.StartRow + 1 == rs.RowCount && rd.EndColumn - rd.StartColumn == rs.ColumnCount
public bool Property_EndColumn(object src, object comparedDest)
        {
            if (comparedDest == null)
            {
                return src == null;
            }
            ReferredArea rd = (ReferredArea)comparedDest;
            if (rd.IsExternalLink || src is string)
            {
                return rd.ToString().Equals(src);
            }
            Aspose.Cells.Range rs = (Aspose.Cells.Range)src;
            return rd.StartRow == rs.FirstRow && rd.StartColumn == rs.FirstColumn
                && rd.EndRow - rd.StartRow + 1 == rs.RowCount && rd.EndColumn - rd.StartColumn == rs.ColumnCount
                && rs.Worksheet.Name.Equals(rd.SheetName);
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


