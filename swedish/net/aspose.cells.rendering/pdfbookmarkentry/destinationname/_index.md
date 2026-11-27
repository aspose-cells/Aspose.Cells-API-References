---
title: "PdfBookmarkEntry.DestinationName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PdfBookmarkEntry-egenskap. Hämtar eller anger namn på destination"
type: docs
url: /sv/net/aspose.cells.rendering/pdfbookmarkentry/destinationname/
---
## PdfBookmarkEntry.DestinationName property

Hämtar eller anger namn på destinationen.

```csharp
public string DestinationName { get; set; }
```

### Anmärkningar

Om destinationsnamnet är angivet kommer destinationen att definieras som en namngiven destination med detta namn.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class PdfBookmarkEntryPropertyDestinationNameDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempelinnehåll i celler
            worksheet.Cells["A1"].PutValue("Primary Content Section");
            worksheet.Cells["A2"].PutValue("Secondary Content Section");

            // Skapa huvud-PDF-bokmärkespost
            PdfBookmarkEntry mainEntry = new PdfBookmarkEntry
            {
                Text = "Main Section",
                Destination = worksheet.Cells["A1"],
                IsOpen = true
            };

            // Demonstrera läsning av initial DestinationName (null)
            Console.WriteLine($"Initial DestinationName: {mainEntry.DestinationName ?? "null"}");

            // Ange anpassat destinationsnamn för huvudposten
            mainEntry.DestinationName = "PrimaryDestination";
            Console.WriteLine($"Updated DestinationName: {mainEntry.DestinationName}");

            // Skapa underbokmärkespost
            PdfBookmarkEntry subEntry = new PdfBookmarkEntry
            {
                Text = "Sub Section",
                Destination = worksheet.Cells["A2"],
                DestinationName = "SecondaryDestination"
            };

            // Lägg till underpost till huvudbokmärket
            mainEntry.SubEntry = new System.Collections.ArrayList { subEntry };

            // Konfigurera PDF-sparalternativ med bokmärkesstruktur
            PdfSaveOptions pdfOptions = new PdfSaveOptions
            {
                Bookmark = mainEntry
            };

            // Spara arbetsboken med PDF-bokmärken
            workbook.Save("PdfBookmarkDestinationDemo.pdf", pdfOptions);

            Console.WriteLine("PDF created with custom bookmark destinations.");
        }
    }
}
```

### Se även

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


