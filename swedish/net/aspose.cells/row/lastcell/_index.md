---
title: "Row.LastCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Hämtar det sista cellobjektet i raden"
type: docs
url: /sv/net/aspose.cells/row/lastcell/
---
## Row.LastCell property

Hämtar det sista cellobjektet i raden.

```csharp
public Cell LastCell { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyLastCellDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata i celler
            worksheet.Cells["A1"].PutValue("First");
            worksheet.Cells["B1"].PutValue("Second");
            worksheet.Cells["C1"].PutValue("Last");

            // Hämta den första raden
            Row row = worksheet.Cells.Rows[0];

            // Åtkomst till den sista cellen i raden
            Cell lastCell = row.LastCell;
            
            // Skriv ut värdet på den sista cellen
            Console.WriteLine("Last cell value: " + lastCell.Value);
        }
    }
}
```

### Se även

* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


