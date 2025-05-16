---
title: Cells.ClearFormats
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Clears formatting of a range
type: docs
url: /net/aspose.cells/cells/clearformats/
---
## ClearFormats(CellArea) {#clearformats}

Clears formatting of a range.

```csharp
public void ClearFormats(CellArea range)
```

| Parameter | Type | Description |
| --- | --- | --- |
| range | CellArea | Range to be cleared. |

### Examples

```csharp
namespace AsposeCellsExamples.CellsMethodClearFormatsWithCellAreaDemo
{
    using Aspose.Cells;
    using System;

    public class CellsMethodClearFormatsWithCellAreaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Create sample data with formatting
            CellArea formatArea = new CellArea();
            formatArea.StartRow = 0;
            formatArea.StartColumn = 0;
            formatArea.EndRow = 2;
            formatArea.EndColumn = 2;

            // Apply formatting to cells
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = System.Drawing.Color.LightYellow;
            
            for (int row = formatArea.StartRow; row <= formatArea.EndRow; row++)
            {
                for (int col = formatArea.StartColumn; col <= formatArea.EndColumn; col++)
                {
                    cells[row, col].PutValue($"Formatted {row},{col}");
                    cells[row, col].SetStyle(style);
                }
            }

            // Define clear area
            CellArea clearArea = new CellArea();
            clearArea.StartRow = 1;
            clearArea.StartColumn = 1;
            clearArea.EndRow = 1;
            clearArea.EndColumn = 1;

            try
            {
                // Clear formats from center cell
                cells.ClearFormats(clearArea);
                Console.WriteLine($"Cleared formats in area: Row {clearArea.StartRow}-{clearArea.EndRow}, Column {clearArea.StartColumn}-{clearArea.EndColumn}");
                
                // Update cleared cell value to show effect
                cells[1, 1].PutValue("Cleared Format");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearFormats: {ex.Message}");
            }

            // Save result
            workbook.Save("CellsMethodClearFormatsWithCellAreaDemo.xlsx");
        }
    }
}
```

### See Also

* struct [CellArea](../../cellarea/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ClearFormats(int, int, int, int) {#clearformats_1}

Clears formatting of a range.

```csharp
public void ClearFormats(int startRow, int startColumn, int endRow, int endColumn)
```

| Parameter | Type | Description |
| --- | --- | --- |
| startRow | Int32 | Start row index. |
| startColumn | Int32 | Start column index. |
| endRow | Int32 | End row index. |
| endColumn | Int32 | End column index. |

### Examples

```csharp
// Called: cells.ClearFormats(1048575, 16383, 1048575, 16383);
public void Cells_Method_ClearFormats()
{
    caseName = "testClearFormats_Excel2007_002";
    Workbook workbook = new Workbook();
    Cells cells = workbook.Worksheets[0].Cells;
    Style style = GetStyle(workbook);
    cells[0, 0].SetStyle(style);
    cells[0, 16383].SetStyle(style);
    cells[1048575, 0].SetStyle(style);
    cells[1048575, 16383].SetStyle(style);

    cells.ClearFormats(1048575, 16383, 1048575, 16383);

    checkClearFormats_Excel2007_002(workbook);
    workbook.Save(Constants.destPath + "testClearFormats.xlsx");
    workbook = new Workbook(Constants.destPath + "testClearFormats.xlsx");
    checkClearFormats_Excel2007_002(workbook);
    workbook.Save(Constants.destPath + "testClearFormats.xml", SaveFormat.SpreadsheetML);
    workbook = new Workbook(Constants.destPath + "testClearFormats.xml");
    workbook.Save(Constants.destPath + "testClearFormats.xls");
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


