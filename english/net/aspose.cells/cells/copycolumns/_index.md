---
title: Cells.CopyColumns
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of the whole columns
type: docs
url: /net/aspose.cells/cells/copycolumns/
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
private static void Method_PasteOptions_(Worksheet workSheet, Workbook upgradingWorkbook)
        {
            if (upgradingWorkbook.Worksheets[workSheet.Name] != null &amp;&amp; upgradingWorkbook.Worksheets[workSheet.Name].Index != -1)
            {

                if (workSheet.Cells.MaxColumn &gt;= 0)
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
// Called: destCells.CopyColumns(sourceCells, 0, 0, colsToCopy);
[Test]
        public void Method_Int32_()
        {
            Workbook source = new Workbook(Constants.sourcePath + &quot;intermediate-source.xlsx&quot;);
            Workbook dest = new Workbook(Constants.sourcePath + &quot;intermediate-destination.xlsx&quot;);
            Worksheet sourceSheet = source.Worksheets[&quot;IT FX&quot;];
            Worksheet destSheet = dest.Worksheets[&quot;IT FX&quot;];

            Cells sourceCells = sourceSheet.Cells;
            Cells destCells = destSheet.Cells;
            int colsToCopy = sourceCells.MaxDataColumn + 2;
            destCells.CopyColumns(sourceCells, 0, 0, colsToCopy);
            Assert.AreEqual(sourceSheet.Cells[&quot;O11&quot;].Formula, destSheet.Cells[&quot;O11&quot;].Formula);

            Util.ReSave(dest, SaveFormat.Xlsx);
            //dest.Save(Constants.destPath + &quot;CellsJava41922.xlsx&quot;);
            Util.SaveManCheck(dest, &quot;Shape&quot;, &quot;CellsJava41922.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


