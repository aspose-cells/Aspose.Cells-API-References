---
title: "Classe RevisionQueryTable"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.Revisions.RevisionQueryTable. Rappresenta una revisione di una modifica al campo di una tabella di query"
type: docs
url: /it/net/aspose.cells.revisions/revisionquerytable/
---
## RevisionQueryTable class

Rappresenta una revisione di una modifica al campo della tabella di query.

```csharp
public class RevisionQueryTable : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [CellArea](../../aspose.cells.revisions/revisionquerytable/cellarea/) { get; } | Ottiene la posizione della tabella di query interessata. |
| [FieldId](../../aspose.cells.revisions/revisionquerytable/fieldid/) { get; } | Ottiene l'ID del campo specifico della tabella di query che è stato rimosso. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| override [Type](../../aspose.cells.revisions/revisionquerytable/type/) { get; } | Rappresenta il tipo della revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionQueryTableDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Aggiungi dati di esempio per creare un contesto per la tabella di query
                worksheet.Cells["A1"].Value = "Product";
                worksheet.Cells["B1"].Value = "Price";
                worksheet.Cells["A2"].Value = "Apple";
                worksheet.Cells["B2"].Value = 1.20;

                // Nota: le istanze di RevisionQueryTable sono tipicamente ottenute dalle revisioni della cartella di lavoro
                // Questa è una dimostrazione concettuale poiché non possiamo istanziare direttamente RevisionQueryTable

                // In uno scenario reale, accederesti alle revisioni in questo modo:
                // RevisionCollection revisions = workbook.Worksheets.Revisions;
                // foreach (Revision revision in revisions)
                // {
                //     if (revision is RevisionQueryTable queryTableRevision)
                //     {
                //         // Access properties
                //     }
                // }

                // Per dimostrazione, mostreremo come lavorare con le proprietà di RevisionQueryTable
                // se avessimo un'istanza
                Console.WriteLine("RevisionQueryTable properties demonstration:");
                Console.WriteLine("Type property would return: " + RevisionType.QueryTable);
                Console.WriteLine("FieldId property would return an integer ID of the affected field");
                Console.WriteLine("CellArea property would return the location of the query table");

                // Salva la cartella di lavoro
                workbook.Save("RevisionQueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionQueryTable: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


