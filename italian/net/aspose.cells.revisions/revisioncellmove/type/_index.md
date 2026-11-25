---
title: "RevisionCellMove.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà RevisionCellMove. Rappresenta il tipo di revisione"
type: docs
url: /it/net/aspose.cells.revisions/revisioncellmove/type/
---
## RevisionCellMove.Type property

Rappresenta il tipo di revisione.

```csharp
public override RevisionType Type { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellMovePropertyTypeDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e ottieni il primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Crea un'istanza di RevisionCellMove usando la riflessione
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Visualizza il valore della proprietà Type (sola lettura)
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Mostra contesto aggiuntivo (opzionale)
                Console.WriteLine("Source Area: " + cellMoveRev.SourceArea);
                Console.WriteLine("Destination Area: " + cellMoveRev.DestinationArea);

                // Salva la cartella di lavoro (opzionale)
                workbook.Save("RevisionCellMoveTypeDemo.xlsx");
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

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


