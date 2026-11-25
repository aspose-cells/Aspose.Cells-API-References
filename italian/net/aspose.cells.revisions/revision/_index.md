---
title: "Classe Revision"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.Revision. Rappresenta la revisione"
type: docs
url: /it/net/aspose.cells.revisions/revision/
---
## Revision class

Rappresenta la revisione.

```csharp
public abstract class Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione. |
| virtual [Type](../../aspose.cells.revisions/revision/type/) { get; } | Rappresenta il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi alcuni dati per potenzialmente creare revisioni
                worksheet.Cells["A1"].PutValue("Original Value");

                // Salva il workbook per stabilire una base di riferimento
                workbook.Save("RevisionDemo_Baseline.xlsx");

                // Carica il workbook e apporta una modifica
                Workbook modifiedWorkbook = new Workbook("RevisionDemo_Baseline.xlsx");
                modifiedWorkbook.Worksheets[0].Cells["A1"].PutValue("Modified Value");

                // Verifica se ci sono log di revisione
                if (modifiedWorkbook.Worksheets.RevisionLogs.Count > 0)
                {
                    RevisionLog log = modifiedWorkbook.Worksheets.RevisionLogs[0];
                    if (log.Revisions.Count > 0)
                    {
                        // Ottieni la prima revisione
                        Revision revision = log.Revisions[0];

                        // Visualizza le proprietà in sola lettura
                        Console.WriteLine($"Revision ID: {revision.Id}");
                        Console.WriteLine($"Revision Type: {revision.Type}");
                        Console.WriteLine($"Worksheet Name: {revision.Worksheet.Name}");

                        // Salva la cartella di lavoro modificata
                        modifiedWorkbook.Save("RevisionDemo_Modified.xlsx");
                    }
                    else
                    {
                        Console.WriteLine("No revisions found in the log");
                    }
                }
                else
                {
                    Console.WriteLine("No revision logs available");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with Revision: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


