---
title: ReferredArea.IsExternalLink
second_title: Aspose.Cells for .NET API Reference
description: ReferredArea property. Indicates whether this is an external link
type: docs
url: /net/aspose.cells/referredarea/isexternallink/
---
## ReferredArea.IsExternalLink property

Indicates whether this is an external link.

```csharp
public bool IsExternalLink { get; }
```

### Examples

```csharp
// Called: if (ra.IsExternalLink)
private void Property_IsExternalLink(ReferredArea ra)
            {
                if (ra.IsExternalLink)
                {
                    Console.WriteLine(&quot;External link is not supported.&quot;);
                    return;
                }
                Cells cells = _wb.Worksheets[ra.SheetName].Cells;
                int startRow = ra.StartRow;
                int startCol = ra.StartColumn;
                int endRow = ra.EndRow;
                int endCol = ra.EndColumn;
                for (int i = startRow; i &lt;= endRow; i++)
                {
                    for (int j = startCol; j &lt;= endCol; j++)
                    {
                        Cell cell = cells.CheckCell(i, j);
                        if (cell == null)
                        {
                            Console.WriteLine(CellsHelper.CellIndexToName(i, j) + &quot;: cell is null&quot;);
                        }
                        else
                        {
                            Console.WriteLine(cell.Name + &quot;.Value: &quot; + cell.Value);
                        }
                    }
                }
            }
```

### See Also

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


