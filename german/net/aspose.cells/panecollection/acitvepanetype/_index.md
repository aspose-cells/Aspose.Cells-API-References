---
title: "PaneCollection.AcitvePaneType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaneCollection-Eigenschaft. Liest und setzt das aktive Pane"
type: docs
url: /de/net/aspose.cells/panecollection/acitvepanetype/
---
## PaneCollection.AcitvePaneType property

Liest und setzt das aktive Pane.

```csharp
[Obsolete("Use PaneCollection.ActivePaneType property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public RectangleAlignmentType AcitvePaneType { get; set; }
```

### Hinweise

HINWEIS: Diese Eigenschaft ist jetzt veraltet. Verwenden Sie stattdessen die [`ActivePaneType`](../activepanetype/)-Eigenschaft. Diese Methode wird 12 Monate später, seit Juli 2026, entfernt werden. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sind.

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten hinzufügen, um das Aufteilen von Pane zu demonstrieren
            for (int i = 0; i < 20; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Row {i + 1}, Col {j + 1}";
                }
            }

            // Das Arbeitsblatt in Pane aufteilen
            worksheet.Split();

            // Abrufen der Pane-Sammlung
            PaneCollection panes = worksheet.GetPanes();

            // Aktuelles aktives Pane anzeigen
            Console.WriteLine("Current ActivePaneType: " + panes.AcitvePaneType);

            // Aktives Pane auf BottomRight setzen
            panes.AcitvePaneType = RectangleAlignmentType.BottomRight;
            Console.WriteLine("Changed ActivePaneType to: " + panes.AcitvePaneType);

            // Erste sichtbare Zeile/Spalte für bottom/right Panes festlegen
            panes.FirstVisibleRowOfBottomPane = 15;
            panes.FirstVisibleColumnOfRightPane = 7;

            // Speichere die Arbeitsmappe
            workbook.Save("PaneCollectionActivePaneTypeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [RectangleAlignmentType](../../../aspose.cells.drawing/rectanglealignmenttype/)
* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


