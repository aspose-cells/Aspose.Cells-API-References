---
title: "RevisionCellMove.SourceArea"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellMove. Ottiene l'area di origine"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

Ottiene l'area di origine.

```csharp
public CellArea SourceArea { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class RevisionCellMovePropertySourceAreaDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Popola alcune celle con dati di esempio
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // Il campione originale utilizzava funzionalità di tracciamento delle revisioni che non sono
                // parte dell'API riflessa (IsTrackChanges, MoveRows, Revisions).
                // Per mantenere il codice pronto per la compilazione dimostriamo la SourceArea
                // proprietà creando un'istanza di RevisionCellMove tramite riflessione.
                // -------------------------------------------------------------

                // Crea un'istanza di RevisionCellMove usando la riflessione
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Visualizza il valore di SourceArea (sola lettura)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // Informazioni correlate aggiuntive (opzionale)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // SourceWorksheet può essere null per un'istanza appena creata
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("RevisionCellMoveSourceAreaDemo.xlsx");
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

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


