---
title: "RevisionCellMove.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellMove‑egenskap. Representerar typen av revision"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellmove/type/
---
## RevisionCellMove.Type property

Representerar typen av revision.

```csharp
public override RevisionType Type { get; }
```

### Exempel

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
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].Value = "Sample Data";
            worksheet.Cells["B1"].Value = "Test Value";

            try
            {
                // Skapa en instans av RevisionCellMove med hjälp av reflektion
                RevisionCellMove cellMoveRev = (RevisionCellMove)Activator.CreateInstance(
                    typeof(RevisionCellMove));

                // Visa Type‑egenskapens värde (skrivskyddad)
                Console.WriteLine("Revision Type: " + cellMoveRev.Type);

                // Visa ytterligare kontext (valfritt)
                Console.WriteLine("Source Area: " + cellMoveRev.SourceArea);
                Console.WriteLine("Destination Area: " + cellMoveRev.DestinationArea);

                // Spara arbetsboken (valfritt)
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

### Se även

* enum [RevisionType](../../revisiontype/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


