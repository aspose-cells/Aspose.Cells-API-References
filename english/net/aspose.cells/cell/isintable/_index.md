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
namespace AsposeCellsExamples.CellPropertyIsInTableDemo
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class CellPropertyIsInTableDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Create sample data for table
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(1.8);

            // Create table from data range using correct Add parameters
            int startRow = 0;
            int startColumn = 0;
            int endRow = 2;
            int endColumn = 1;
            bool hasHeaders = true;
            int tableIndex = worksheet.ListObjects.Add(startRow, startColumn, endRow, endColumn, hasHeaders);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.DisplayName = "PriceTable"; // Use DisplayName instead of Name

            // Access cells to check IsInTable status
            Cell tableCell = worksheet.Cells["A2"];
            Cell nonTableCell = worksheet.Cells["D5"];

            Console.WriteLine($"Cell A2 IsInTable value: {tableCell.IsInTable}");  // True
            Console.WriteLine($"Cell D5 IsInTable value: {nonTableCell.IsInTable}");  // False

            // Expand table by adding a row
            int newRowIndex = table.EndRow + 1;
            worksheet.Cells[newRowIndex, table.StartColumn].PutValue("Orange");
            worksheet.Cells[newRowIndex, table.StartColumn + 1].PutValue(3.2);
            table.Resize(table.StartRow, table.StartColumn, newRowIndex, table.EndColumn, table.ShowHeaderRow);

            // Check IsInTable for new cell
            Cell newTableCell = worksheet.Cells["A4"];
            Console.WriteLine($"New cell A4 IsInTable value: {newTableCell.IsInTable}");  // True

            // Save the workbook
            workbook.Save("CellPropertyIsInTableDemo.xlsx");
        }
    }
}
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


