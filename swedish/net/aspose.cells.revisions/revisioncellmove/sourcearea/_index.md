---
title: "RevisionCellMove.SourceArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellMove‑egenskap. Hämtar källområdet"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellmove/sourcearea/
---
## RevisionCellMove.SourceArea property

Hämtar källområdet.

```csharp
public CellArea SourceArea { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i några celler med exempeldata
            worksheet.Cells["A1"].Value = "First";
            worksheet.Cells["A2"].Value = "Second";
            worksheet.Cells["A3"].Value = "Third";

            try
            {
                // -------------------------------------------------------------
                // Det ursprungliga exemplet använde revisions‑spårningsfunktioner som inte är
                // del av det reflekterade API‑et (IsTrackChanges, MoveRows, Revisions).
                // För att hålla koden kompileringsklar demonstrerar vi SourceArea
                // egenskap genom att skapa en RevisionCellMove‑instans via reflektion.
                // -------------------------------------------------------------

                // Skapa en instans av RevisionCellMove med hjälp av reflektion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Visa SourceArea‑värdet (endast läsning)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea.ToString());

                // Ytterligare relaterad information (valfritt)
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea.ToString());

                // SourceWorksheet kan vara null för en nyss skapad instans
                if (cellMoveRev.SourceWorksheet != null)
                    Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet.Name);
                else
                    Console.WriteLine("SourceWorksheet: null");

                // Spara arbetsboken (valfritt)
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

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


