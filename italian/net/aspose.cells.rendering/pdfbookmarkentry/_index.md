---
title: "Classe PdfBookmarkEntry"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Rendering.PdfBookmarkEntry. PdfBookmarkEntry è una voce nel segnalibro PDF. Se la proprietà Text dell'istanza corrente è null, l'istanza corrente sarà nascosta e i figli saranno inseriti al livello corrente."
type: docs
url: /it/net/aspose.cells.rendering/pdfbookmarkentry/
---
## PdfBookmarkEntry class

PdfBookmarkEntry è una voce nel segnalibro PDF. Se la proprietà Text dell'istanza corrente è null o "", l'istanza corrente sarà nascosta e i figli saranno inseriti al livello corrente.

```csharp
public class PdfBookmarkEntry
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [PdfBookmarkEntry](pdfbookmarkentry/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Destination](../../aspose.cells.rendering/pdfbookmarkentry/destination/) { get; set; } | La cella a cui è collegato il segnalibro. |
| [DestinationName](../../aspose.cells.rendering/pdfbookmarkentry/destinationname/) { get; set; } | Ottiene o imposta il nome della destinazione. |
| [IsCollapse](../../aspose.cells.rendering/pdfbookmarkentry/iscollapse/) { get; set; } | Quando questa proprietà è true, il bookmarkentry si chiuderà, altrimenti si espanderà. |
| [IsOpen](../../aspose.cells.rendering/pdfbookmarkentry/isopen/) { get; set; } | Quando questa proprietà è true, il bookmarkentry si espanderà, altrimenti si chiuderà. |
| [SubEntry](../../aspose.cells.rendering/pdfbookmarkentry/subentry/) { get; set; } | SubEntry di un segnalibro. |
| [Text](../../aspose.cells.rendering/pdfbookmarkentry/text/) { get; set; } | Titolo di un segnalibro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;
    using System.Collections;

    public class PdfBookmarkEntryDemo
    {
        public static void PdfBookmarkEntryExample()
        {
            // Crea una nuova cartella di lavoro e aggiungi fogli di lavoro
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            workbook.Worksheets.Add();

            // Ottieni le celle da ogni foglio di lavoro
            Cell cellInPage1 = workbook.Worksheets[0].Cells["A1"];
            Cell cellInPage2 = workbook.Worksheets[1].Cells["A1"];
            Cell cellInPage3 = workbook.Worksheets[2].Cells["A1"];

            // Inserisci valori nelle celle
            cellInPage1.PutValue("page1");
            cellInPage2.PutValue("page2");
            cellInPage3.PutValue("page3");

            // Crea il PdfBookmarkEntry radice
            PdfBookmarkEntry pbeRoot = new PdfBookmarkEntry
            {
                Text = "root",  // if pbeRoot.Text = null, all children of pbeRoot will be inserted on the top level in the bookmark.
                Destination = cellInPage1,
                SubEntry = new ArrayList(),
                IsOpen = false
            };

            // Crea PdfBookmarkEntries secondari
            PdfBookmarkEntry subPbe1 = new PdfBookmarkEntry
            {
                Text = "section1",
                Destination = cellInPage2
            };

            PdfBookmarkEntry subPbe2 = new PdfBookmarkEntry
            {
                Text = "section2",
                Destination = cellInPage3
            };

            // Aggiungi voci secondarie all'entry radice
            pbeRoot.SubEntry.Add(subPbe1);
            pbeRoot.SubEntry.Add(subPbe2);

            // Crea PdfSaveOptions e imposta il segnalibro
            PdfSaveOptions saveOptions = new PdfSaveOptions
            {
                Bookmark = pbeRoot
            };

            // Salva la cartella di lavoro come PDF con segnalibri
            workbook.Save("output_bookmark.pdf", saveOptions);
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)


