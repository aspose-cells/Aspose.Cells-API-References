---
title: "RevisionCellMove.Type"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellMove-Eigenschaft. Stellt den Typ der Revision dar"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellmove/type/
---
## RevisionCellMove.Type property

Stellt den Typ der Revision dar.

```csharp
public override RevisionType Type { get; }
```

### Beispiele

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
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Erstellen Sie eine Instanz von RevisionCellMove mittels Reflexion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Zeigen Sie den Wert der Type‑Eigenschaft an (schreibgeschützt)
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Zusätzlichen Kontext anzeigen (optional)
                Console.WriteLine("Source Area: " + cellMoveRev.SourceArea);
                Console.WriteLine("Destination Area: " + cellMoveRev.DestinationArea);

                // Arbeitsmappe speichern (optional)
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

### Siehe auch

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


