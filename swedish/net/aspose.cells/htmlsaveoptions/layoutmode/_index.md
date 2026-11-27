---
title: "HtmlSaveOptions.LayoutMode"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Hämtar eller anger layoutläget när du sparar till HTML. Standardvärdet är Normal"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/layoutmode/
---
## HtmlSaveOptions.LayoutMode property

Hämtar eller anger layoutläge när du sparar till HTML. Standardvärdet är Normal

```csharp
public HtmlLayoutMode LayoutMode { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyLayoutModeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Layout Mode Test");

            try
            {
                // Skapa en HtmlSaveOptions-instans
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Visa det aktuella LayoutMode‑värdet
                Console.WriteLine("Current LayoutMode: " + options.LayoutMode);

                // Ställ in LayoutMode till Print
                options.LayoutMode = HtmlLayoutMode.Print;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Spara arbetsboken med Print‑layoutläge
                workbook.Save("LayoutModePrint.html", options);

                // Ställ in LayoutMode till Normal
                options.LayoutMode = HtmlLayoutMode.Normal;
                Console.WriteLine("LayoutMode set to: " + options.LayoutMode);

                // Spara arbetsboken med Normal‑layoutläge
                workbook.Save("LayoutModeNormal.html", options);

                Console.WriteLine("HTML files saved with different LayoutMode settings.");
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

* enum [HtmlLayoutMode](../../../aspose.cells.rendering/htmllayoutmode/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


