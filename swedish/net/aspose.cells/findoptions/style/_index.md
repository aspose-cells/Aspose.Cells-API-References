---
title: "FindOptions.Style"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-egenskap. Formatet att söka efter"
type: docs
url: /sv/net/aspose.cells/findoptions/style/
---
## FindOptions.Style property

Formatet att söka efter.

```csharp
public Style Style { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil med blått teckensnitt
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Blue;

            // Applicera stilen på cellen F2
            Cell cell = worksheet.Cells["F2"];
            cell.PutValue("SearchTarget");
            cell.SetStyle(style);

            // Skapa sökalternativ med stilen
            FindOptions options = new FindOptions();
            options.Style = style;

            // Hitta cell med matchande stil
            Cell foundCell = worksheet.Cells.Find(null, null, options);

            // Skriv ut den hittade cellens namn
            Console.WriteLine("Cell found with matching style: " + foundCell?.Name);
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


