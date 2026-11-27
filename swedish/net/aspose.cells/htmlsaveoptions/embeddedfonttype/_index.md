---
title: "HtmlSaveOptions.EmbeddedFontType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HtmlSaveOptions-egenskap. Hämtar eller anger typen av inbäddad teckensnittfil i HTML‑filen. Standardvärdet är None, vilket indikerar att inget teckensnitt kommer att bäddas in i HTML"
type: docs
url: /sv/net/aspose.cells/htmlsaveoptions/embeddedfonttype/
---
## HtmlSaveOptions.EmbeddedFontType property

Hämtar eller anger typen av inbäddning av teckensnittsfiler i html‑filen. Standardvärdet är None vilket indikerar att inget teckensnitt kommer att bäddas in i html.

```csharp
public HtmlEmbeddedFontType EmbeddedFontType { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertyEmbeddedFontTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Sample Text with Font");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.Font.Name = "Arial";
            worksheet.Cells["A1"].SetStyle(style);

            try
            {
                // Skapa HTML-sparalternativ
                HtmlSaveOptions options = new HtmlSaveOptions();

                // Visa standardvärdet för EmbeddedFontType
                Console.WriteLine("Default EmbeddedFontType: " + options.EmbeddedFontType);

                // Ställ in EmbeddedFontType till Woff
                options.EmbeddedFontType = HtmlEmbeddedFontType.Woff;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Spara arbetsboken med WOFF-typsnittsinbäddning
                workbook.Save("EmbeddedFontType_Woff.html", options);

                // Återställ till Ingen
                options.EmbeddedFontType = HtmlEmbeddedFontType.None;
                Console.WriteLine("EmbeddedFontType set to: " + options.EmbeddedFontType);

                // Spara arbetsboken utan typsnittsinbäddning
                workbook.Save("EmbeddedFontType_None.html", options);

                Console.WriteLine("EmbeddedFontType demonstration completed successfully.");
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

* enum [HtmlEmbeddedFontType](../../../aspose.cells.rendering/htmlembeddedfonttype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


