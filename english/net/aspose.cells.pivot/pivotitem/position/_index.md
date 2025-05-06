---
title: PivotItem.Position
second_title: Aspose.Cells for .NET API Reference
description: PivotItem property. Specifying the position index in all the PivotItemsnot the PivotItems under the same parent node
type: docs
url: /net/aspose.cells.pivot/pivotitem/position/
---
## PivotItem.Position property

Specifying the position index in all the PivotItems,not the PivotItems under the same parent node.

```csharp
public int Position { get; set; }
```

### Examples

```csharp
// Called: pi.Position = 0;// THIS IS IMPORTANT
private static void Property_Position(Workbook workbook, String pivotTableName, String sheetName)
    {
        Worksheet worksheet = workbook.Worksheets[sheetName];
        Console.WriteLine(&quot;Refresh started..&quot;);

        if (worksheet != null)
        {
            PivotTable pivotTable = worksheet.PivotTables[pivotTableName];
            if (worksheet.PivotTables.Count &gt; 0)
            {
                if (pivotTable != null)
                {
                    Console.WriteLine(&quot;pivot&quot;);
                    for (int i = 0; i &lt; pivotTable.PageFields.Count; i++)
                    {
                        PivotField pf = pivotTable.PageFields[i];
                        for (int j = 0; j &lt; pf.PivotItems.Count; j++)
                        {
                            PivotItem pi = pf.PivotItems[j];
                            if (pi != null)
                            {
                                pi.Position = 0;// THIS IS IMPORTANT
                            }
                            else
                            {
                                Console.WriteLine(&quot;PivotItem is null&quot;);
                            }
                        }
                        pf.ShowAllItems = true;
                        Console.WriteLine(&quot;Field- &quot; + pf.Name);
                    }
                    pivotTable.RefreshData();
                    pivotTable.CalculateData();
                    pivotTable.RefreshDataOnOpeningFile = true;
                }
            }
        }

        workbook.CalculateFormula(true);
    }
```

### See Also

* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


