---
title: "PdfBookmarkEntry.DestinationName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PdfBookmarkEntry-Eigenschaft. Liest oder setzt den Namen des Ziels"
type: docs
url: /de/net/aspose.cells.rendering/pdfbookmarkentry/destinationname/
---
## PdfBookmarkEntry.DestinationName property

Liest oder setzt den Namen des Ziels.

```csharp
public string DestinationName { get; set; }
```

### Hinweise

Wenn der Zielname festgelegt ist, wird das Ziel als benanntes Ziel mit diesem Namen definiert.

### Beispiele

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
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispielinhalt zu Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Primary Content Section");
            worksheet.Cells["A2"].PutValue("Secondary Content Section");

            // Haupt-PDF-Lesezeicheneintrag erstellen
            PdfBookmarkEntry mainEntry = new PdfBookmarkEntry
            {
                Text = "Main Section",
                Destination = worksheet.Cells["A1"],
                IsOpen = true
            };

            // Demonstration des Lesens des anfänglichen DestinationName (null)
            Console.WriteLine($"Initial DestinationName: {mainEntry.DestinationName ?? "null"}");

            // Benutzerdefinierten Zielnamen für den Haupteintrag festlegen
            mainEntry.DestinationName = "PrimaryDestination";
            Console.WriteLine($"Updated DestinationName: {mainEntry.DestinationName}");

            // Unter-Lesezeicheneintrag erstellen
            PdfBookmarkEntry subEntry = new PdfBookmarkEntry
            {
                Text = "Sub Section",
                Destination = worksheet.Cells["A2"],
                DestinationName = "SecondaryDestination"
            };

            // Unter-Eintrag zum Hauptlesezeichen hinzufügen
            mainEntry.SubEntry = new System.Collections.ArrayList { subEntry };

            // PDF-Speicheroptionen mit Lesezeichenstruktur konfigurieren
            PdfSaveOptions pdfOptions = new PdfSaveOptions
            {
                Bookmark = mainEntry
            };

            // Arbeitsmappe mit PDF-Lesezeichen speichern
            workbook.Save("PdfBookmarkDestinationDemo.pdf", pdfOptions);

            Console.WriteLine("PDF created with custom bookmark destinations.");
        }
    }
}
```

### Siehe auch

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


