---
title: "RevisionLogCollection.Item"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionLogCollection. Ottiene RevisionLog per indice"
type: docs
url: /it/net/aspose.cells.revisions/revisionlogcollection/item/
---
## RevisionLogCollection indexer

Ottiene [`RevisionLog`](../../revisionlog/) per indice.

```csharp
public RevisionLog this[int index] { get; }
```

| Parametro | Descrizione |
| --- | --- |
| indice | L'indice. |

### Valore di ritorno

Restituisce l'oggetto [`RevisionLog`](../../revisionlog/).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionLogCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();

            // Abilita la cartella di lavoro condivisa per supportare le revisioni
            workbook.Settings.Shared = true;

            // Accedi alla raccolta dei log delle revisioni
            RevisionLogCollection revisionLogs = workbook.Worksheets.RevisionLogs;

            try
            {
                // Verifica se ci sono log di revisione
                if (revisionLogs.Count > 0)
                {
                    // Accedi al primo registro delle revisioni usando la proprietà Item
                    RevisionLog firstLog = revisionLogs[0];

                    // Visualizza le informazioni di base sul registro delle revisioni
                    Console.WriteLine("First revision log accessed via Item property:");
                    Console.WriteLine($"Revision count: {firstLog.Revisions.Count}");
                }
                else
                {
                    Console.WriteLine("No revision logs available in the workbook.");
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionLogItemDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [RevisionLog](../../revisionlog/)
* class [RevisionLogCollection](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


