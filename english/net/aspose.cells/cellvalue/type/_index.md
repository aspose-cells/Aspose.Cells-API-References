---
title: CellValue.Type
second_title: Aspose.Cells for .NET API Reference
description: CellValue property. Gets or sets the type of cell value
type: docs
url: /net/aspose.cells/cellvalue/type/
---
## CellValue.Type property

Gets or sets the type of cell value.

```csharp
public CellValueType Type { get; set; }
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellValuePropertyTypeDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Set different cell values with different types
            worksheet.Cells["A1"].PutValue("Text Value"); // Text type
            worksheet.Cells["A2"].PutValue(123.45);       // Numeric type
            worksheet.Cells["A3"].PutValue(true);        // Boolean type
            worksheet.Cells["A4"].PutValue("=1/0");       // Error type (will show #DIV/0!)

            // Process each cell and demonstrate Type property
            for (int i = 0; i < 4; i++)
            {
                Cell cell = worksheet.Cells[0, i];
                CellValue value = (CellValue)cell.Value;
                
                Console.WriteLine($"Cell {cell.Name} - Original Type: {value.Type}, Value: {value.Value}");

                // Demonstrate changing type for error values
                if (value.Type == CellValueType.IsError && "#DIV/0!".Equals(value.Value))
                {
                    value.Type = CellValueType.IsNull;
                    Console.WriteLine($"Changed error to null - New Type: {value.Type}");
                }
            }
        }
    }
}
```

### See Also

* enum [CellValueType](../../cellvaluetype/)
* class [CellValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


