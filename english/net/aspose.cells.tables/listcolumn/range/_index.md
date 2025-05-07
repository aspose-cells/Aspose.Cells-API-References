---
title: ListColumn.Range
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets the range of this list column
type: docs
url: /net/aspose.cells.tables/listcolumn/range/
---
## ListColumn.Range property

Gets the range of this list column.

```csharp
public Range Range { get; }
```

### Examples

```csharp
// Called: Cell cellToApply = col.Range[1, 0];
private static void Property_Range(Workbook workbook, Worksheet sheet)
        {

            for (var i = 0; i < sheet.ListObjects[0].ListColumns.Count; i++)
            {
                try
                {
                    var col = sheet.ListObjects[0].ListColumns[i];

                    if (col != null)
                    {
                        Cell cellToApply = col.Range[1, 0];
                        //if (cellToApply is { Formula: { } })
                        if (cellToApply.Formula != null)
                        {
                            col.Formula = cellToApply.Formula;
                            //   break;
                        }

                    }
                }
                catch (Exception e)
                {
                    Console.WriteLine(e);
                }


            }
        }
```

### See Also

* class [Range](../../../aspose.cells/range/)
* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


