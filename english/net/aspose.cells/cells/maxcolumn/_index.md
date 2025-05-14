---
title: Cells.MaxColumn
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Maximum column index of those cells that have been instantiated in the collectiondoes not include the column where style is defined for the whole column but no cell has been instantiated in it
type: docs
url: /net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Maximum column index of those cells that have been instantiated in the collection(does not include the column where style is defined for the whole column but no cell has been instantiated in it).

```csharp
public int MaxColumn { get; }
```

### Remarks

Return -1 if there is no cell has been instantiated.

### Examples

```csharp
// Called: upgradingWorkbook.Worksheets[workSheet.Name].Cells.CopyColumns(workSheet.Cells, 0, 0, workSheet.Cells.MaxColumn + 1, new PasteOptions() { PasteType = PasteType.Formats }); // raises the exception
private static void Cells_Property_MaxColumn(Worksheet workSheet, Workbook upgradingWorkbook)
        {
            if (upgradingWorkbook.Worksheets[workSheet.Name] != null && upgradingWorkbook.Worksheets[workSheet.Name].Index != -1)
            {

                if (workSheet.Cells.MaxColumn >= 0)
                {
                    try
                    {
                        //Copy Columns is having issue in latest version of aspose
                        upgradingWorkbook.Worksheets[workSheet.Name].Cells.CopyColumns(workSheet.Cells, 0, 0, workSheet.Cells.MaxColumn + 1, new PasteOptions() { PasteType = PasteType.Formats }); // raises the exception
                    }
                    catch (Exception ex)
                    {
                        Console.WriteLine(ex.Message);
                    }

                    //Copy Rows works fine in any version
                    //upgradingWorkbook.Worksheets[workSheet.Name].Cells.CopyRows(workSheet.Cells, 0, 0, workSheet.Cells.MaxColumn + 1);
                    Aspose.Cells.Range range = workSheet.Cells.CreateRange(0, 0, workSheet.Cells.MaxRow + 1, workSheet.Cells.MaxColumn + 1);
                    Aspose.Cells.Range upgradeRange = upgradingWorkbook.Worksheets[workSheet.Name].Cells.CreateRange(0, 0, workSheet.Cells.MaxRow + 1, workSheet.Cells.MaxColumn + 1);
                    upgradeRange.CopyData(range);

                }
            }
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


