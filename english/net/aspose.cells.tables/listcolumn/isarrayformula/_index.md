---
title: ListColumn.IsArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: ListColumn property. Indicates whether the fomula is array formula
type: docs
url: /net/aspose.cells.tables/listcolumn/isarrayformula/
---
## ListColumn.IsArrayFormula property

Indicates whether the fomula is array formula.

```csharp
public bool IsArrayFormula { get; }
```

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListColumnPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Add sample data
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);
            
            // Create a table
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            
            // Get the first list column
            ListColumn listColumn = table.ListColumns[0];
            
            // Set an array formula for the column
            listColumn.Formula = "=A2:A3*2";
            
            // Display the current formula of the column
            Console.WriteLine("Current formula: " + listColumn.Formula);
            
            // Show the effect of the array formula
            Console.WriteLine("Array formula applied to column:");
            Console.WriteLine("Cell A2 value: " + worksheet.Cells["A2"].Value);
            Console.WriteLine("Cell A3 value: " + worksheet.Cells["A3"].Value);
            
            // Clear the formula
            listColumn.Formula = "";
            Console.WriteLine("\nAfter clearing the formula:");
            Console.WriteLine("Current formula: " + listColumn.Formula);
            
            // Save the result
            workbook.Save("ListColumnPropertyIsArrayFormulaDemo.xlsx");
        }
    }
}
```

### See Also

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


