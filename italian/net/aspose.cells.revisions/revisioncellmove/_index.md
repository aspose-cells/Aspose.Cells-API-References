---
title: "Classe RevisionCellMove"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.Revisions.RevisionCellMove classe. Rappresenta un record di revisione su una cella che è stata spostata"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellmove/
---
## RevisionCellMove class

Rappresenta un record di revisione su una/e cella/e che è/sono stata/e spostata/e.

```csharp
public class RevisionCellMove : Revision
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [DestinationArea](../../aspose.cells.revisions/revisioncellmove/destinationarea/) { get; } | Ottiene l'area di destinazione. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ottiene il numero di questa revisione.(Ereditato da [`Revision`](../revision/).) |
| [SourceArea](../../aspose.cells.revisions/revisioncellmove/sourcearea/) { get; } | Ottiene l'area di origine. |
| [SourceWorksheet](../../aspose.cells.revisions/revisioncellmove/sourceworksheet/) { get; } | Ottiene il foglio di lavoro di origine. |
| override [Type](../../aspose.cells.revisions/revisioncellmove/type/) { get; } | Rappresenta il tipo di revisione. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ottiene il foglio di lavoro.(Ereditato da [`Revision`](../revision/).) |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionsClassRevisionCellMoveDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Crea un'istanza della classe RevisionCellMove usando la riflessione
                // poiché il costruttore non è direttamente accessibile
                RevisionCellMove revisionCellMove = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Visualizza le proprietà di sola lettura
                Console.WriteLine("Revision Type: " + revisionCellMove.Type);
                Console.WriteLine("Source Area: " + revisionCellMove.SourceArea);
                Console.WriteLine("Destination Area: " + revisionCellMove.DestinationArea);

                // Verifica se SourceWorksheet è disponibile
                if (revisionCellMove.SourceWorksheet != null)
                {
                    Console.WriteLine("Source Worksheet: " + revisionCellMove.SourceWorksheet.Name);
                }
                else
                {
                    Console.WriteLine("Source Worksheet: null");
                }

                // Salva la cartella di lavoro
                workbook.Save("RevisionCellMoveDemo.xlsx");
                Console.WriteLine("RevisionCellMove demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with RevisionCellMove: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


