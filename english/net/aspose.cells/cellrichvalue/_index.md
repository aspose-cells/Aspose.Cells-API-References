---
title: Class CellRichValue
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.CellRichValue class. Represents the rich value of the cell
type: docs
url: /net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Represents the rich value of the cell.

```csharp
public abstract class CellRichValue
```

## Properties

| Name | Description |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Gets the alt text associated with the image. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Gets the error value type of the cell. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Gets the image data of the cell. |

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            
            // Access first worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Set a rich value in cell A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // Get the rich value from cell A1
            CellRichValue richValue = cell.GetRichValue();
            
            // Display the rich value properties
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // Save the workbook
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


