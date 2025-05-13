---
title: ListColumn.Formula
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Gets and sets the formula of the list column
type: docs
url: /net/aspose.cells.tables/listcolumn/formula/
---
## ListColumn.Formula property

Gets and sets the formula of the list column.

```csharp
public string Formula { get; set; }
```

### Examples

```csharp
// Called: col.Formula = cellToApply.Formula;
private static void ListColumn_Property_Formula(Workbook workbook, Worksheet sheet)
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

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


