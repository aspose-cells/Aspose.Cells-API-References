---
title: Cells.MinDataRow
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Minimum row index of cell which contains data
type: docs
url: /net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Minimum row index of cell which contains data.

```csharp
public int MinDataRow { get; }
```

### Remarks

Return -1 if there is no cell which contains data.

### Examples

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // Create a workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Populate some data
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // Demonstrate MinDataRow usage
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // Save the workbook
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


