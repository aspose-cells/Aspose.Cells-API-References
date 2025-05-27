---
title: CalculationCell.Worksheet
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell property. Gets the Worksheet object where the cell is in
type: docs
url: /net/aspose.cells/calculationcell/worksheet/
---
## CalculationCell.Worksheet property

Gets the Worksheet object where the cell is in.

```csharp
public Worksheet Worksheet { get; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CalculationCellPropertyWorksheetDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DemoSheet";
            
            // Create calculation cells by getting them from worksheet
            Cell cellA1 = worksheet.Cells[0, 0];
            Cell cellB2 = worksheet.Cells[1, 1];
            
            // Demonstrate Worksheet property usage
            Console.WriteLine("Cell A1 is in worksheet: " + cellA1.Worksheet.Name);
            Console.WriteLine("Cell B2 is in worksheet: " + cellB2.Worksheet.Name);
            
            // Verify both cells are in the same worksheet
            if (cellA1.Worksheet == cellB2.Worksheet)
            {
                Console.WriteLine("Both cells are in the same worksheet");
            }
            
            // Create another worksheet and cell
            Worksheet newSheet = workbook.Worksheets.Add("SecondSheet");
            Cell cellC3 = newSheet.Cells[2, 2];
            
            // Show different worksheet case
            Console.WriteLine("Cell C3 is in worksheet: " + cellC3.Worksheet.Name);
            if (cellA1.Worksheet != cellC3.Worksheet)
            {
                Console.WriteLine("Cell A1 and C3 are in different worksheets");
            }
        }
    }
}
```

### See Also

* class [Worksheet](../../worksheet/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


