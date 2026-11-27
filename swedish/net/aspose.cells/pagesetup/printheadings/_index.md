---
title: "PageSetup.PrintHeadings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Representerar om rad- och kolumnrubriker skrivs ut på den här sidan"
type: docs
url: /sv/net/aspose.cells/pagesetup/printheadings/
---
## PageSetup.PrintHeadings property

Anger om rad- och kolumnrubriker skrivs ut med den här sidan.

```csharp
public bool PrintHeadings { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintHeadingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Ställ in exempeldata med rubriker
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.5);
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B3"].PutValue(1.8);

            // Aktivera utskrift av rubriker
            worksheet.PageSetup.PrintHeadings = true;
            worksheet.PageSetup.PrintArea = "A1:B3";

            // Spara som HTML för att demonstrera effekten
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportActiveWorksheetOnly = true,
                ExportPrintAreaOnly = true,
                ExportGridLines = true,
                ExportHeadings = true
            };

            workbook.Save("PrintHeadingsDemo.html", saveOptions);

            Console.WriteLine("Worksheet saved with PrintHeadings enabled.");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


