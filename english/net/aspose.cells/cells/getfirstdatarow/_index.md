---
title: Cells.GetFirstDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells method. Gets the first row index of cell which contains data in the specified column
type: docs
url: /net/aspose.cells/cells/getfirstdatarow/
---
## Cells.GetFirstDataRow method

Gets the first row index of cell which contains data in the specified column.

```csharp
public int GetFirstDataRow(int column)
```

| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |

### Return Value

first row index.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsMethodGetFirstDataRowWithInt32Demo
    {
        public static void Run()
        {
            // Create a new workbook and access first worksheet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Clear existing data and format
            worksheet.Cells.Clear();

            // Add test data to column A (index 0)
            worksheet.Cells["A3"].PutValue("First Data");
            worksheet.Cells["A5"].PutValue("Second Data");
            worksheet.Cells["A7"].PutValue("Third Data");

            try
            {
                // Find first data row manually since GetFirstDataRow method isn't available
                int firstDataRowIndex = FindFirstDataRow(worksheet.Cells, 0);
                
                if (firstDataRowIndex == -1)
                {
                    Console.WriteLine("No data found in column A");
                    return;
                }

                // Display results
                Console.WriteLine($"First data row in column A: {firstDataRowIndex + 1}"); // Convert to 1-based index
                
                // Highlight result in spreadsheet
                Cell resultCell = worksheet.Cells[firstDataRowIndex, 0];
                Style style = resultCell.GetStyle();
                style.Font.Color = System.Drawing.Color.Red;
                resultCell.SetStyle(style);
                
                worksheet.Cells["B1"].PutValue($"First data at row: {firstDataRowIndex + 1}");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Save modified workbook
            workbook.Save("CellsMethodGetFirstDataRowWithInt32Demo.xlsx");
        }

        private static int FindFirstDataRow(Cells cells, int column)
        {
            for (int row = 0; row <= cells.MaxDataRow; row++)
            {
                Cell cell = cells[row, column];
                if (cell.Value != null)
                {
                    return row;
                }
            }
            return -1;
        }
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


