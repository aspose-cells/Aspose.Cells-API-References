---
title: Cell.IsInTable
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Indicates whether this cell is part of table formula
type: docs
url: /net/aspose.cells/cell/isintable/
---
## Cell.IsInTable property

Indicates whether this cell is part of table formula.

```csharp
[Obsolete("Use IsTableFormula instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsInTable { get; }
```

### Remarks

NOTE: This class is now obsolete. Instead, please use Cell.IsTableFormula to check whether the cell formula is part of table formula. This property will be removed 12 months later since May 2018. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellPropertyIsInTableDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to the worksheet
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(0.8);

            // Create a table from the data range
            int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];

            try
            {
                // Check IsInTable property for cells inside and outside the table
                Cell cellInTable = worksheet.Cells["A2"];
                Cell cellOutsideTable = worksheet.Cells["C2"];

                Console.WriteLine("Cell A2 (inside table):");
                Console.WriteLine("  Value: " + cellInTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellInTable.IsInTable);

                Console.WriteLine("\nCell C2 (outside table):");
                Console.WriteLine("  Value: " + cellOutsideTable.StringValue);
                Console.WriteLine("  IsInTable: " + cellOutsideTable.IsInTable);

                // Save the workbook
                workbook.Save("IsInTableDemo.xlsx");
                Console.WriteLine("\nWorkbook saved successfully.");
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

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


