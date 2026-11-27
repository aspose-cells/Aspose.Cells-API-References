---
title: "RevisionCellMove.SourceWorksheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellMove‑egenskap. Hämtar källarbetsbladet"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellmove/sourceworksheet/
---
## RevisionCellMove.SourceWorksheet property

Hämtar källarbetsbladet.

```csharp
public Worksheet SourceWorksheet { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Skapa en instans av RevisionCellMove med hjälp av reflektion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Visa SourceWorksheet‑egenskapens värde (skrivskyddad)
                Console.WriteLine("SourceWorksheet: " + cellMoveRev.SourceWorksheet);

                // Ytterligare sammanhang (valfritt)
                Console.WriteLine("SourceArea: " + cellMoveRev.SourceArea);
                Console.WriteLine("DestinationArea: " + cellMoveRev.DestinationArea);
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Spara arbetsboken (valfritt)
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

### Se även

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


