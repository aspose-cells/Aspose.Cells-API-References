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
private static void PivotItem_Property_Position(Workbook workbook, String pivotTableName, String sheetName)
    {
        Worksheet worksheet = workbook.Worksheets[sheetName];
        Console.WriteLine("Refresh started..");

        if (worksheet != null)
        {
            PivotTable pivotTable = worksheet.PivotTables[pivotTableName];
            if (worksheet.PivotTables.Count > 0)
            {
                if (pivotTable != null)
                {
                    Console.WriteLine("pivot");
                    for (int i = 0; i < pivotTable.PageFields.Count; i++)
                    {
                        PivotField pf = pivotTable.PageFields[i];
                        for (int j = 0; j < pf.PivotItems.Count; j++)
                        {
                            PivotItem pi = pf.PivotItems[j];
                            if (pi != null)
                            {
                                pi.Position = 0;// THIS IS IMPORTANT
                            }
                            else
                            {
                                Console.WriteLine("PivotItem is null");
                            }
                        }
                        pf.ShowAllItems = true;
                        Console.WriteLine("Field- " + pf.Name);
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


