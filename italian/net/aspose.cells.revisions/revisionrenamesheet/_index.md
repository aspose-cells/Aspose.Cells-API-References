---
title: "Classe RevisionRenameSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionRenameSheet. Rappresenta una revisione della rinomina del foglio"
type: docs
url: /it/net/aspose.cells.revisions/revisionrenamesheet/
---
## RevisionRenameSheet class

Rappresenta una revisione della rinomina del foglio.

```csharp
public class RevisionRenameSheet : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| [NewName](../../aspose.cells.revisions/revisionrenamesheet/newname/) { get; } | Ottiene il nuovo nome del foglio di lavoro. |
| [OldName](../../aspose.cells.revisions/revisionrenamesheet/oldname/) { get; } | Ottiene il vecchio nome del foglio di lavoro. |
| override [Type](../../aspose.cells.revisions/revisionrenamesheet/type/) { get; } | Rappresenta il tipo della revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionRenameSheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Memorizza il nome originale e rinomina il foglio
                string originalName = worksheet.Name;
                worksheet.Name = "RenamedSheet";

                // Salva in un flusso di memoria per generare revisioni
                System.IO.MemoryStream ms = new System.IO.MemoryStream();
                workbook.Save(ms, SaveFormat.Xlsx);

                // Riapri la cartella di lavoro per accedere ai registri delle revisioni
                workbook = new Workbook(ms);

                // Verifica i registri delle revisioni per l'operazione di rinomina
                foreach (RevisionLog log in workbook.Worksheets.RevisionLogs)
                {
                    foreach (Revision rv in log.Revisions)
                    {
                        if (rv.Type == RevisionType.RenameSheet)
                        {
                            RevisionRenameSheet renameSheet = (RevisionRenameSheet)rv;
                            Console.WriteLine("Revision Type: " + renameSheet.Type);
                            Console.WriteLine("Old Sheet Name: " + renameSheet.OldName);
                            Console.WriteLine("New Sheet Name: " + renameSheet.NewName);
                        }
                    }
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionRenameSheetDemo.xlsx");
                Console.WriteLine("RevisionRenameSheet demo completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in RevisionRenameSheet demo: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


