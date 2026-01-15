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

            // Access the first worksheet
            Worksheet worksheet = workbook.Worksheets[0];

            // Add sample data to create a table
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue(20);

            // Create a table/list object
            int tableIndex = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[tableIndex];

            // Add an array formula to the second column
            listObject.ListColumns[1].Formula = "{=SUM(A2:A3*B2:B3)}";

            try
            {
                // Access the IsArrayFormula property (read-only)
                bool isArrayFormula = listObject.ListColumns[1].IsArrayFormula;

                // Display the value
                Console.WriteLine("IsArrayFormula value: " + isArrayFormula);

                // Save the workbook
                workbook.Save("IsArrayFormulaDemo.xlsx");
                Console.WriteLine("Demo completed successfully.");
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

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


