---
title: "RevisionCellMove.DestinationArea"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RevisionCellMove-Eigenschaft. Gibt den Zielbereich zurück"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellmove/destinationarea/
---
## RevisionCellMove.DestinationArea property

Liefert den Zielbereich.

```csharp
public CellArea DestinationArea { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Revisions;

    public class RevisionCellMovePropertyDestinationAreaDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe, um eine gültige Umgebung zu erhalten (optional für die Demo)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Demo";

            try
            {
                // Instanziieren Sie RevisionCellMove mittels Reflexion (parameterloser Konstruktor)
                RevisionCellMove revMove = (RevisionCellMove)Activator.CreateInstance(typeof(RevisionCellMove));

                // Lesen und anzeigen Sie die DestinationArea-Eigenschaft (schreibgeschützt)
                CellArea destination = revMove.DestinationArea;
                Console.WriteLine("DestinationArea: " + destination.ToString());

                // Zusätzlicher Kontext (optional)
                Console.WriteLine("SourceArea: " + revMove.SourceArea.ToString());
                Console.WriteLine("Revision Type: " + revMove.Type);

                // Arbeitsmappe speichern (optional)
                workbook.Save("RevisionCellMoveDestinationAreaDemo.xlsx");
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


