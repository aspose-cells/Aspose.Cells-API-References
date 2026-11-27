---
title: "PaneCollection.AcitvePaneType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PaneCollection-egenskap. Hämtar och anger den aktiva panelen"
type: docs
url: /sv/net/aspose.cells/panecollection/acitvepanetype/
---
## PaneCollection.AcitvePaneType property

Hämtar och anger den aktiva panelen.

```csharp
[Obsolete("Use PaneCollection.ActivePaneType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public RectangleAlignmentType AcitvePaneType { get; set; }
```

### Anmärkningar

OBS: Denna egenskap är nu föråldrad. Använd istället [`ActivePaneType`](../activepanetype/) egenskapen. Denna metod kommer att tas bort 12 månader senare från och med juli 2026. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PaneCollectionPropertyAcitvePaneTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för att demonstrera delning av paneler
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
                }
            }

            // Dela kalkylbladet i paneler
            worksheet.Split();

            // Hämta panelsamlingen
            PaneCollection panes = worksheet.GetPanes();

            // Visa aktuell aktiv panel
            Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);

            // Ställ in den aktiva panelen till BottomRight
            panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
            Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);

            // Ställ in första synliga rad/kolumn för nedre/höger paneler
            panes.FirstVisibleRowOfBottomPane = 15;
            panes.FirstVisibleColumnOfRightPane = 7;

            // Spara arbetsboken
            workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
        }
    }
}
```

### Se även

* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


