---
title: "PdfBookmarkEntry.DestinationName"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà PdfBookmarkEntry. Ottiene o imposta il nome della destinazione"
type: docs
url: /it/net/aspose.cells.rendering/pdfbookmarkentry/destinationname/
---
## PdfBookmarkEntry.DestinationName property

Ottiene o imposta il nome della destinazione.

```csharp
public string DestinationName { get; set; }
```

### Osservazioni

Se il nome della destinazione è impostato, la destinazione verrà definita come destinazione nominata con questo nome.

### Esempi

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
            // Crea una nuova cartella di lavoro e accedi al primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi contenuto di esempio alle celle
            worksheet.Cells["A1"].PutValue("Primary Content Section");
            worksheet.Cells["A2"].PutValue("Secondary Content Section");

            // Crea voce principale di segnalibro PDF
            PdfBookmarkEntry mainEntry = new PdfBookmarkEntry
            {
                Text = "Main Section",
                Destination = worksheet.Cells["A1"],
                IsOpen = true
            };

            // Dimostrare la lettura del DestinationName iniziale (null)
            Console.WriteLine($"Initial DestinationName: {mainEntry.DestinationName ?? "null"}");

            // Impostare un nome di destinazione personalizzato per la voce principale
            mainEntry.DestinationName = "PrimaryDestination";
            Console.WriteLine($"Updated DestinationName: {mainEntry.DestinationName}");

            // Creare una voce di sottosegno
            PdfBookmarkEntry subEntry = new PdfBookmarkEntry
            {
                Text = "Sub Section",
                Destination = worksheet.Cells["A2"],
                DestinationName = "SecondaryDestination"
            };

            // Aggiungere una sotto‑voce al segno principale
            mainEntry.SubEntry = new System.Collections.ArrayList { subEntry };

            // Configurare le opzioni di salvataggio PDF con la struttura dei segnalibri
            PdfSaveOptions pdfOptions = new PdfSaveOptions
            {
                Bookmark = mainEntry
            };

            // Salvare la cartella di lavoro con i segnalibri PDF
            workbook.Save("PdfBookmarkDestinationDemo.pdf", pdfOptions);

            Console.WriteLine("PDF created with custom bookmark destinations.");
        }
    }
}
```

### Vedi anche

* class [PdfBookmarkEntry](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


