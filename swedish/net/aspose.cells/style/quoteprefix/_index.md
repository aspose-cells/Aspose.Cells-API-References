---
title: "Style.QuotePrefix"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-egenskap. Anger om cellens värde börjar med ett enkelt citattecken"
type: docs
url: /sv/net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Indikerar om cellens värde börjar med enkelfnutt.

```csharp
public bool QuotePrefix { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Få åtkomst till cell B10 och sätt dess värde
            Cell cell = worksheet.Cells["B10"];
            cell.PutValue("'12345"); // Note the single quote prefix

            // Hämta cellens stil och aktivera QuotePrefix
            Style style = cell.GetStyle();
            style.QuotePrefix = true;
            cell.SetStyle(style);

            // Spara arbetsboken
            workbook.Save("output.xlsx");

            // Verifiera QuotePrefix-egenskapen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
            Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
        }
    }
}
```

### Se även

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


