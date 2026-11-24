---
title: "RevisionCellMove.SourceWorksheet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellMove‑Eigenschaft. Gibt das Quell‑Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellmove/sourceworksheet/
---
## RevisionCellMove.SourceWorksheet property

Liefert das Quell-Arbeitsblatt.

```csharp
public Worksheet SourceWorksheet { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Revisions;
    using System;

    public class RevisionCellMovePropertySourceWorksheetDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten hinzu, um das Beispiel sinnvoll zu machen.
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Erstellen Sie eine Instanz von RevisionCellMove mittels Reflexion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Zeigen Sie den Wert der SourceWorksheet‑Eigenschaft an (schreibgeschützt)
                Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet);

                // Zusätzlicher Kontext (optional)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea);
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea);
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Arbeitsmappe speichern (optional)
                workbook.Save("SourceWorksheetDemo.xlsx");
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

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


