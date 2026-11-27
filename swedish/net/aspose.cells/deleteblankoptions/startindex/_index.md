---
title: "DeleteBlankOptions.StartIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DeleteBlankOptions egenskap. Anger startrad-/kolumnindex för området som ska kontrolleras och där tomma rader/kolumner ska tas bort"
type: docs
url: /sv/net/aspose.cells/deleteblankoptions/startindex/
---
## DeleteBlankOptions.StartIndex property

Specificerar startrad-/kolumnindex för området som ska kontrolleras och där tom rad/kolumn tas bort.

```csharp
public int StartIndex { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyStartIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Fyll i några celler med värden
            cells[2, 0].PutValue("Row 3");
            cells[5, 0].PutValue("Row 6");
            cells[9, 0].PutValue("Row 10");

            Console.WriteLine("Before deleting blank rows:");
            for (int i = 0; i <= 10; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }

            // Ta bort tomma rader från index 4 (Rad 5) till index 7 (Rad 8)
            DeleteBlankOptions options = new DeleteBlankOptions();
            options.StartIndex = 4;
            options.EndIndex = 7;
            cells.DeleteBlankRows(options);

            Console.WriteLine("\nAfter deleting blank rows from Row 5 to Row 8:");
            for (int i = 0; i <= 7; i++)
            {
                Console.WriteLine($"Row {i + 1}: {(cells[i, 0].Value ?? "empty")}");
            }
        }
    }
}
```

### Se även

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


