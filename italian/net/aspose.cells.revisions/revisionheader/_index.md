---
title: "Classe RevisionHeader"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Revisions.RevisionHeader class. Rappresenta un elenco di modifiche specifiche avvenute per questa cartella di lavoro"
type: docs
url: /it/net/aspose.cells.revisions/revisionheader/
---
## RevisionHeader class

Rappresenta un elenco di modifiche specifiche che si sono verificate per questa cartella di lavoro.

```csharp
public class RevisionHeader
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [RevisionHeader](revisionheader/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [SavedTime](../../aspose.cells.revisions/revisionheader/savedtime/) { get; set; } | Ottiene e imposta la data e l'ora in cui questo insieme di revisioni è stato salvato. |
| [UserName](../../aspose.cells.revisions/revisionheader/username/) { get; set; } | Ottiene e imposta il nome dell'utente che effettua la revisione. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionHeaderDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea un'istanza della classe RevisionHeader
                RevisionHeader revisionHeader = new RevisionHeader();

                // Imposta le proprietà essenziali
                revisionHeader.SavedTime = DateTime.Now;
                revisionHeader.UserName = "TestUser";

                // Dimostra la funzionalità di base
                Console.WriteLine($"Revision saved by: {revisionHeader.UserName}");
                Console.WriteLine($"Revision saved at: {revisionHeader.SavedTime}");

                // Salva la cartella di lavoro
                workbook.Save("RevisionHeaderDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with revision header information.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionHeader: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


