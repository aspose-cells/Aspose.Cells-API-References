---
title: "Row.IsBlank"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row egenskap. Anger om raden innehåller någon data"
type: docs
url: /sv/net/aspose.cells/row/isblank/
---
## Row.IsBlank property

Anger om raden innehåller någon data

```csharp
public bool IsBlank { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyIsBlankDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Hämta första raden (initialt tom)
            Row row1 = worksheet.Cells.Rows[0];
            Console.WriteLine("Row 1 IsBlank: " + row1.IsBlank); // True
            
            // Lägg till data i första raden
            worksheet.Cells["A1"].PutValue("Test");
            Console.WriteLine("Row 1 IsBlank after adding data: " + row1.IsBlank); // False
            
            // Skapa en annan tom rad
            Row row2 = worksheet.Cells.Rows[1];
            Console.WriteLine("Row 2 IsBlank: " + row2.IsBlank); // True
            
            // Jämför radens tomma status
            Console.WriteLine("Rows have same IsBlank status: " + (row1.IsBlank == row2.IsBlank)); // False
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


