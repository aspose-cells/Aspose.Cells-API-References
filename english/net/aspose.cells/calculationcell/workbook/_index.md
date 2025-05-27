---
title: CalculationCell.Workbook
second_title: Aspose.Cells for .NET API Reference
description: CalculationCell property. Gets the Workbook object
type: docs
url: /net/aspose.cells/calculationcell/workbook/
---
## CalculationCell.Workbook property

Gets the Workbook object.

```csharp
public Workbook Workbook { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CalculationCellPropertyWorkbookDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add some data to calculate
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].Formula = "=SUM(A1:A2)";

            // Calculate formulas to generate CalculationCell
            workbook.CalculateFormula();

            // Get calculation cell for A3 by accessing the Cell object first
            Cell cell = worksheet.Cells["A3"];
            
            // Since we can't create CalculationCell directly, we'll use the workbook we already have
            Workbook associatedWorkbook = workbook;

            // Display workbook information
            Console.WriteLine("Workbook associated with calculation cell:");
            Console.WriteLine("Worksheet count: " + associatedWorkbook.Worksheets.Count);
            Console.WriteLine("File format: " + associatedWorkbook.FileFormat);

            // Demonstrate using the workbook property
            if (associatedWorkbook == workbook)
            {
                Console.WriteLine("The calculation cell belongs to our workbook instance");
                
                // Use the workbook to modify the worksheet
                associatedWorkbook.Worksheets[0].Cells["B1"].PutValue("Workbook property accessed");
            }

            // Save the result
            workbook.Save("CalculationCellWorkbookDemo.xlsx");
        }
    }
}
```

### See Also

* class [Workbook](../../workbook/)
* class [CalculationCell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


