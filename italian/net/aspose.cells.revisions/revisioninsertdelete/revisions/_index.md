---
title: "RevisionInsertDelete.Revisions"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionInsertDelete. Ottiene l'elenco delle revisioni per questa operazione"
type: docs
url: /it/net/aspose.cells.revisions/revisioninsertdelete/revisions/
---
## RevisionInsertDelete.Revisions property

Ottiene l'elenco delle revisioni per questa operazione.

```csharp
public RevisionCollection Revisions { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionInsertDeletePropertyRevisionsDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook e abilita il tracciamento delle revisioni
            Workbook workbook = new Workbook();
            workbook.Worksheets.RevisionLogs.DaysPreservingHistory = 30;

            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];

            // Esegui operazioni per generare revisioni
            worksheet.Cells.InsertRows(0, 1);
            worksheet.Cells.DeleteRows(1, 1);

            // Ottieni i registri delle revisioni
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            // Itera attraverso tutti i registri delle revisioni
            foreach (RevisionLog revisionLog in revisionLogs)
            {
                foreach (Revision revision in revisionLog.Revisions)
                {
                    if (revision is RevisionInsertDelete)
                    {
                        RevisionInsertDelete revisionInsertDelete = (RevisionInsertDelete)revision;

                        // Accedi alla proprietà Revisions (sola lettura)
                        RevisionCollection revisions = revisionInsertDelete.Revisions;

                        // Visualizza le informazioni sulle revisioni
                        Console.WriteLine("Revision Type: " + revisionInsertDelete.Type);
                        Console.WriteLine("Action Type: " + revisionInsertDelete.ActionType);
                        Console.WriteLine("Cell Area: " + revisionInsertDelete.CellArea);
                        Console.WriteLine("Number of related revisions: " + revisions.Count);

                        // Dimostra l'uso della collezione Revisions
                        foreach (Revision relatedRevision in revisions)
                        {
                            Console.WriteLine(" - Related revision ID: " + relatedRevision.Id);
                            if (relatedRevision is RevisionInsertDelete)
                            {
                                RevisionInsertDelete relatedInsertDelete = (RevisionInsertDelete)relatedRevision;
                                Console.WriteLine("   Action Type: " + relatedInsertDelete.ActionType);
                                Console.WriteLine("   Cell Area: " + relatedInsertDelete.CellArea);
                            }
                        }
                    }
                }
            }

            // Salva la cartella di lavoro con le revisioni
            workbook.Save("RevisionInsertDeletePropertyRevisionsDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [RevisionCollection](../../revisioncollection/)
* class [RevisionInsertDelete](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


