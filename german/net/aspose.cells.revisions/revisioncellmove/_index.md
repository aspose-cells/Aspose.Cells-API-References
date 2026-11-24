---
title: "Klasse RevisionCellMove"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Revisions.RevisionCellMove Klasse. Stellt einen Revisionsdatensatz für Zellen dar, die verschoben wurden"
type: docs
url: /de/net/aspose.cells.revisions/revisioncellmove/
---
## RevisionCellMove class

Stellt einen Revisionsdatensatz über eine verschobene Zelle(n) dar.

```csharp
public class RevisionCellMove : Revision
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [DestinationArea](../../aspose.cells.revisions/revisioncellmove/destinationarea/) { get; } | Liefert den Zielbereich. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Ermittelt die Nummer dieser Revision.(Vererbt von [`Revision`](../revision/).) |
| [SourceArea](../../aspose.cells.revisions/revisioncellmove/sourcearea/) { get; } | Liefert den Quellbereich. |
| [SourceWorksheet](../../aspose.cells.revisions/revisioncellmove/sourceworksheet/) { get; } | Liefert das Quell-Arbeitsblatt. |
| override [Type](../../aspose.cells.revisions/revisioncellmove/type/) { get; } | Stellt den Typ der Revision dar. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Ermittelt das Arbeitsblatt.(Vererbt von [`Revision`](../revision/).) |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Erstelle eine Instanz der RevisionCellMove-Klasse mittels Reflexion
                // da der Konstruktor nicht direkt zugänglich ist
                RevisionCellMove revisionCellMove = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Zeige die schreibgeschützten Eigenschaften an
                Console.WriteLine("Revision Type: " + revisionCellMove.Type);
                Console.WriteLine("Source Area: " + revisionCellMove.SourceArea);
                Console.WriteLine("Destination Area: " + revisionCellMove.DestinationArea);

                // Prüfe, ob SourceWorksheet verfügbar ist
                if (revisionCellMove.SourceWorksheet != null)
                {
                    Console.WriteLine("Source Worksheet: " + revisionCellMove.SourceWorksheet.Name);
                }
                else
                {
                    Console.WriteLine("Source Worksheet: null");
                }

                // Speichere die Arbeitsmappe
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

### Siehe auch

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


