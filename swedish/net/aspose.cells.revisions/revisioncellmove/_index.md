---
title: "Klass RevisionCellMove"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Revisions.RevisionCellMove klass. Representerar en revisionspost för en cell som har flyttats"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellmove/
---
## RevisionCellMove class

Representerar en revisionspost för en cell(er) som har flyttats.

```csharp
public class RevisionCellMove : Revision
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [DestinationArea](../../aspose.cells.revisions/revisioncellmove/destinationarea/) { get; } | Hämtar destinationsområdet. |
| [Id](../../aspose.cells.revisions/revision/id/) { get; } | Hämtar numret för denna revision.(Arv från [`Revision`](../revision/).) |
| [SourceArea](../../aspose.cells.revisions/revisioncellmove/sourcearea/) { get; } | Hämtar källområdet. |
| [SourceWorksheet](../../aspose.cells.revisions/revisioncellmove/sourceworksheet/) { get; } | Hämtar källarbetsbladet. |
| override [Type](../../aspose.cells.revisions/revisioncellmove/type/) { get; } | Representerar typen av revision. |
| [Worksheet](../../aspose.cells.revisions/revision/worksheet/) { get; } | Hämtar kalkylbladet.(Arv från [`Revision`](../revision/).) |

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en instans av RevisionCellMove-klassen med hjälp av reflektion
                // eftersom konstruktorn inte är direkt åtkomlig
                RevisionCellMove revisionCellMove = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Visa skrivskyddade egenskaper
                Console.WriteLine("Revision Type: " + revisionCellMove.Type);
                Console.WriteLine("Source Area: " + revisionCellMove.SourceArea);
                Console.WriteLine("Destination Area: " + revisionCellMove.DestinationArea);

                // Kontrollera om SourceWorksheet är tillgänglig
                if (revisionCellMove.SourceWorksheet != null)
                {
                    Console.WriteLine("Source Worksheet: " + revisionCellMove.SourceWorksheet.Name);
                }
                else
                {
                    Console.WriteLine("Source Worksheet: null");
                }

                // Spara arbetsboken
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

### Se även

* class [Revision](../revision/)
* namespace [Aspose.Cells.Revisions](../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../)


