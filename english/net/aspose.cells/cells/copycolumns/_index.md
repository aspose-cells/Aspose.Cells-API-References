---
title: Cells.CopyColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of a whole column
type: docs
url: /net/aspose.cells/cells/copycolumns/
---
## CopyColumns(Cells, int, int, int) {#copycolumns}

Copies data and formats of a whole column.

```csharp
public void CopyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| destinationColumnIndex | Int32 | Destination column index. |
| columnNumber | Int32 | The copied column number. |

### Examples

```csharp
// Called: cells.CopyColumns(cells, 4, 5, 1);
public void Cells_Method_CopyColumns()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Cells cells = wb.Worksheets[0].Cells;
    cells.CopyRows(cells, 1, 2, 1);
          
    cells.CopyColumns(cells, 4, 5, 1);
    Assert.AreEqual(wb.Worksheets[0].SparklineGroups.Count, 4);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, int) {#copycolumns_2}

Copies data and formats of the whole columns.

```csharp
public void CopyColumns(Cells sourceCells, int sourceColumnIndex, int sourceTotalColumns, 
    int destinationColumnIndex, int destinationTotalColumns)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| sourceTotalColumns | Int32 | The number of the source columns. |
| destinationColumnIndex | Int32 | Destination column index. |
| destinationTotalColumns | Int32 | The number of the destination columns. |

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyColumns(Cells, int, int, int, PasteOptions) {#copycolumns_1}

Copies data and formats of a whole column.

```csharp
public void CopyColumns(Cells sourceCells0, int sourceColumnIndex, int destinationColumnIndex, 
    int columnNumber, PasteOptions pasteOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceColumnIndex | Int32 | Source column index. |
| destinationColumnIndex | Int32 | Destination column index. |
| columnNumber | Int32 | The copied column number. |
| pasteOptions | PasteOptions | the options of pasting. |

### Examples

```csharp
// Called: upgradingWorkbook.Worksheets[workSheet.Name].Cells.CopyColumns(workSheet.Cells, 0, 0, workSheet.Cells.MaxColumn + 1, new PasteOptions() { PasteType = PasteType.Formats }); // raises the exception
private static void Cells_Method_CopyColumns(Worksheet workSheet, Workbook upgradingWorkbook)
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

* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


