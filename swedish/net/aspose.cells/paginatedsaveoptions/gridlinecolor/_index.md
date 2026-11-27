---
title: "PaginatedSaveOptions.GridlineColor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaginatedSaveOptions-egenskap. Hämtar eller anger färg på rutlinjer"
type: docs
url: /sv/net/aspose.cells/paginatedsaveoptions/gridlinecolor/
---
## PaginatedSaveOptions.GridlineColor property

Hämtar eller anger färg på rutnätslinjer.

```csharp
public Color GridlineColor { get; set; }
```

### Anmärkningar

Den kommer att ignorera inställningarna för rutlinjefärg i källfilen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class PaginatedSaveOptionsPropertyGridlineColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Gridline Color Demo";
            worksheet.Cells["A2"].Value = "Sample Data";

            try
            {
                // Skapa PDF-sparalternativ
                PdfSaveOptions options = new PdfSaveOptions();

                // Visa standardvärdet för GridlineColor
                Console.WriteLine("Default GridlineColor: " + options.GridlineColor);

                // Ange en ny färg för rutnätslinjen
                options.GridlineColor = Color.Red;

                // Visa det uppdaterade värdet för GridlineColor
                Console.WriteLine("Updated GridlineColor: " + options.GridlineColor);

                // Spara arbetsboken med inställningen för rutnätslinjens färg
                workbook.Save("GridlineColorDemo.pdf", options);

                Console.WriteLine("PDF saved with custom gridline color.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [PaginatedSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


