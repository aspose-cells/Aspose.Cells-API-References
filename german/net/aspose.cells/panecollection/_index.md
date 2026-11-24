---
title: "Klasse PaneCollection"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.PaneCollection Klasse. Stellt alle Pane-Objekte dar, die im angegebenen Fenster angezeigt werden"
type: docs
url: /de/net/aspose.cells/panecollection/
---
## PaneCollection class

Stellt alle Pane‑Objekte dar, die im angegebenen Fenster angezeigt werden.

```csharp
public class PaneCollection
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [AcitvePaneType](../../aspose.cells/panecollection/acitvepanetype/) { get; set; } | (**Obsolete.**) Liest und setzt das aktive Pane. |
| [ActivePaneType](../../aspose.cells/panecollection/activepanetype/) { get; set; } | Liest und setzt das aktive Pane. |
| [FirstVisibleColumnOfRightPane](../../aspose.cells/panecollection/firstvisiblecolumnofrightpane/) { get; set; } | Liest und setzt die erste sichtbare Spalte des rechten Panes. |
| [FirstVisibleRowOfBottomPane](../../aspose.cells/panecollection/firstvisiblerowofbottompane/) { get; set; } | Liest und setzt die erste sichtbare Zeile des unteren Panes. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassPaneCollectionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 5; j++)
                {
                    sheet.Cells[i, j].Value = $"Row {i}, Col {j}";
                }
            }
            
            // Fixiere Panes bei Zeile 5, Spalte 1
            sheet.FreezePanes(5, 1, 5, 1);
            
            // Hole Pane-Sammlung
            PaneCollection panes = sheet.GetPanes();
            
            // Ändere Pane-Einstellungen
            panes.FirstVisibleRowOfBottomPane = 5;
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Speichere die Arbeitsmappe
            workbook.Save("PaneCollectionDemo.xls", SaveFormat.Excel97To2003);
            
            Console.WriteLine("PaneCollection demo executed successfully.");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


