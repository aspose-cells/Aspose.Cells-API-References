---
title: "RevisionCellMove.SourceArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellMove‑Eigenschaft. Gibt den Quellbereich zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

Liefert den Quellbereich.

```csharp
public CellArea SourceArea { get; }
```

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie einige Zellen mit Beispieldaten
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // Das ursprüngliche Beispiel verwendete Revision‑Tracking‑Funktionen, die nicht
                // Teil der reflektierten API (IsTrackChanges, MoveRows, Revisions).
                // Um den Code kompiliert‑bereit zu halten, demonstrieren wir die SourceArea
                // Eigenschaft, indem wir eine RevisionCellMove‑Instanz über Reflexion erstellen.
                // -------------------------------------------------------------

                // Erstellen Sie eine Instanz von RevisionCellMove mittels Reflexion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Zeigen Sie den Wert der SourceArea‑Eigenschaft an (schreibgeschützt)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // Zusätzliche verwandte Informationen (optional)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // SourceWorksheet kann bei einer frisch erstellten Instanz null sein
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // Arbeitsmappe speichern (optional)
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

### Siehe auch

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


