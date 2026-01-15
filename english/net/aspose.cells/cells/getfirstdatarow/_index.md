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
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some sample data to demonstrate the method
            worksheet.Cells["A1"].Value = "Header";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["A3"].Value = "Data2";
            worksheet.Cells["B5"].Value = "Data3";
            worksheet.Cells["C7"].Value = "Data4";

            try
            {
                // Get the Cells collection from the worksheet
                Cells cells = worksheet.Cells;

                // Call GetFirstDataRow for column A (index 0)
                int firstDataRowA = cells.GetFirstDataRow(0);
                Console.WriteLine($"First data row in column A: {firstDataRowA}");

                // Call GetFirstDataRow for column B (index 1)
                int firstDataRowB = cells.GetFirstDataRow(1);
                Console.WriteLine($"First data row in column B: {firstDataRowB}");

                // Call GetFirstDataRow for column C (index 2)
                int firstDataRowC = cells.GetFirstDataRow(2);
                Console.WriteLine($"First data row in column C: {firstDataRowC}");

                // Save the workbook
                workbook.Save("GetFirstDataRowDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


