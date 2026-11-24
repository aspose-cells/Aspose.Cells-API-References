---
title: "PaneCollection.FirstVisibleRowOfBottomPane"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaneCollection-Eigenschaft. Liest und setzt die erste sichtbare Zeile des unteren Pane"
type: docs
url: /de/net/aspose.cells/panecollection/firstvisiblerowofbottompane/
---
## PaneCollection.FirstVisibleRowOfBottomPane property

Liest und setzt die erste sichtbare Zeile des unteren Panes.

```csharp
public int FirstVisibleRowOfBottomPane { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten hinzufügen, um ein scrollbares Pane zu erstellen
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Pane bei Zeile 10 einfrieren (dies erzeugt obere und untere Pane)
            worksheet.FreezePanes(10, 0, 10, 0);
            
            // Die Pane-Sammlung abrufen
            PaneCollection panes = worksheet.GetPanes();
            
            // Setzen Sie die erste sichtbare Zeile des unteren Pane
            panes.FirstVisibleRowOfBottomPane = 15;
            
            // Geben Sie die erste sichtbare Zeile des unteren Pane aus
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            
            // Speichere die Arbeitsmappe
            workbook.Save("PaneCollectionPropertyFirstVisibleRowOfBottomPaneDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


