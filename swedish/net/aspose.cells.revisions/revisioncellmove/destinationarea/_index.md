---
title: "RevisionCellMove.DestinationArea"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RevisionCellMove‑egenskap. Hämtar destinationsområdet"
type: docs
url: /sv/net/aspose.cells.revisions/revisioncellmove/destinationarea/
---
## RevisionCellMove.DestinationArea property

Hämtar destinationsområdet.

```csharp
public CellArea DestinationArea { get; }
```

### Exempel

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
            // Skapa en arbetsbok för att ha en giltig miljö (valfritt för demonstrationen)
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Demo";

            try
            {
                // Instansiera RevisionCellMove via reflektion (parameterlös konstruktor)
                RevisionCellMove revMove = (RevisionCellMove)Activator.CreateInstance(typeof(RevisionCellMove));

                // Läs och visa DestinationArea‑egenskapen (endast läsning)
                CellArea destination = revMove.DestinationArea;
                Console.WriteLine("DestinationArea: " + destination.ToString());

                // Ytterligare sammanhang (valfritt)
                Console.WriteLine("SourceArea: " + revMove.SourceArea.ToString());
                Console.WriteLine("Revision Type: " + revMove.Type);

                // Spara arbetsbok (valfritt)
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

### Se även

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [RevisionCellMove](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


