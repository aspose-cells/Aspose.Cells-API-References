---
title: Cell.GetRichValue
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets rich value of the cell
type: docs
url: /net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Gets rich value of the cell.

```csharp
public CellRichValue GetRichValue()
```

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // Create a new workbook
            Workbook wb = new Workbook();
            
            // Access first worksheet
            Worksheet ws = wb.Worksheets[0];
            
            // Set a rich text value in cell A1
            ws.Cells["A1"].PutValue("This is rich text");
            
            // Get the rich value from cell A1
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // Display the rich text value
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // Save the workbook
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### See Also

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


