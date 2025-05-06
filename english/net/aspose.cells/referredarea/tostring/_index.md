---
title: ReferredArea.ToString
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea method. Returns the reference address of this area. Generally it is the address of the reference which may be used in formula such as Sheet1A1C3
type: docs
url: /net/aspose.cells/referredarea/tostring/
---
## ReferredArea.ToString method

Returns the reference address of this area. Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3".

```csharp
public override string ToString()
```

### Return Value

the reference address of this area.

### Examples

```csharp
// Called: return rd.ToString().Equals(src);
public bool Method_ToString(object src, object comparedDest)
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
            return rd.StartRow == rs.FirstRow &amp;&amp; rd.StartColumn == rs.FirstColumn
                &amp;&amp; rd.EndRow - rd.StartRow + 1 == rs.RowCount &amp;&amp; rd.EndColumn - rd.StartColumn == rs.ColumnCount
                &amp;&amp; rs.Worksheet.Name.Equals(rd.SheetName);
        }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


