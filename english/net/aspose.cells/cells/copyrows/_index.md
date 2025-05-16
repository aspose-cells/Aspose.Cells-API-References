---
title: Cells.CopyRows
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Copies data and formats of some whole rows
type: docs
url: /net/aspose.cells/cells/copyrows/
---
## CopyRows(Cells, int, int, int) {#copyrows}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells, int sourceRowIndex, int destinationRowIndex, int rowNumber)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |

### Examples

```csharp
// Called: cells.CopyRows(sourcecells, 0,
public void Cells_Method_CopyRows()
{
         
    Workbook book = new Workbook(Constants.sourcePath + "example.xlsx");
    Workbook book2 = new Workbook(Constants.sourcePath + "example.xlsx");

    //Get the first worksheet 
    Worksheet sheet = book2.Worksheets[0];

    Cells cells, sourcecells;

    cells = book.Worksheets[0].Cells;
    sourcecells = sheet.Cells;

    // copy book2's contents to book's sheet at the end 
    cells.CopyRows(sourcecells, 0,
            cells.MaxDisplayRange.RowCount + 2,
            sourcecells.MaxDisplayRange.RowCount);

    Assert.AreEqual(book.Worksheets[0].SparklineGroups.Count, 2);
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions) {#copyrows_1}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |

### Examples

```csharp
// Called: aWkAsp.Worksheets[0].Cells.CopyRows(aWkAsp.Worksheets[0].Cells, 4, 5, 1, options);
public void Cells_Method_CopyRows()
{

    Aspose.Cells.Workbook aWkAsp = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count,2);

    aWkAsp.Worksheets[0].Cells.InsertRows(5, 1);
    aWkAsp.Worksheets[0].Cells.CopyRows(aWkAsp.Worksheets[0].Cells, 4, 5, 1);
    Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count,4);

    aWkAsp = new Aspose.Cells.Workbook(Constants.sourcePath + "example.xls");
    Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count, 2);
    CopyOptions options = new CopyOptions();
    options.ExtendToAdjacentRange = true;
    aWkAsp.Worksheets[0].Cells.InsertRows(5, 1);
    aWkAsp.Worksheets[0].Cells.CopyRows(aWkAsp.Worksheets[0].Cells, 4, 5, 1, options);
    Assert.AreEqual(aWkAsp.Worksheets[0].Hyperlinks.Count, 2);

}
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## CopyRows(Cells, int, int, int, CopyOptions, PasteOptions) {#copyrows_2}

Copies data and formats of some whole rows.

```csharp
public void CopyRows(Cells sourceCells0, int sourceRowIndex, int destinationRowIndex, 
    int rowNumber, CopyOptions copyOptions, PasteOptions pasteOptions)
```

| Parameter | Type | Description |
| --- | --- | --- |
| sourceCells0 | Cells | Source Cells object contains data and formats to copy. |
| sourceRowIndex | Int32 | Source row index. |
| destinationRowIndex | Int32 | Destination row index. |
| rowNumber | Int32 | The copied row number. |
| copyOptions | CopyOptions | The copy options. |
| pasteOptions | PasteOptions | the options of pasting. |

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo
{
    using Aspose.Cells;
    using System;

    public class CellsMethodCopyRowsWithCellsInt32Int32Int32CopyOptionDemo
    {
        public static void Run()
        {
            // Create a new workbook with two worksheets
            Workbook workbook = new Workbook();
            Worksheet sourceSheet = workbook.Worksheets[0];
            Worksheet destinationSheet = workbook.Worksheets.Add("DestinationSheet");

            // Populate source worksheet with sample data
            sourceSheet.Cells["A1"].PutValue("Source Row 1");
            sourceSheet.Cells["A2"].PutValue("Source Row 2");
            sourceSheet.Cells["A3"].PutValue("Source Row 3");

            try
            {
                // Create copy and paste options
                CopyOptions copyOptions = new CopyOptions();
                PasteOptions pasteOptions = new PasteOptions();

                // Copy 3 rows from source sheet starting at row 0 to destination sheet starting at row 5
                destinationSheet.Cells.CopyRows(
                    sourceSheet.Cells, // Source cells
                    0,                  // Source row index
                    5,                  // Destination row index
                    3,                  // Number of rows to copy
                    copyOptions,
                    pasteOptions
                );

                Console.WriteLine("Rows copied successfully from row 0-2 to row 5-7 in destination sheet");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CopyRows method: {ex.Message}");
            }

            // Save the result
            workbook.Save("CellsMethodCopyRowsWithOptionsDemo.xlsx");
        }
    }
}
```

### See Also

* class [CopyOptions](../../copyoptions/)
* class [PasteOptions](../../pasteoptions/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


