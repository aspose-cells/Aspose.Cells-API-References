---
title: "PaneCollection.FirstVisibleColumnOfRightPane"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PaneCollection-Eigenschaft. Gibt die erste sichtbare Spalte des rechten Panes zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/panecollection/firstvisiblecolumnofrightpane/
---
## PaneCollection.FirstVisibleColumnOfRightPane property

Liest und setzt die erste sichtbare Spalte des rechten Panes.

```csharp
public int FirstVisibleColumnOfRightPane { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PaneCollectionPropertyFirstVisibleColumnOfRightPaneDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Panen einfrieren, indem Zeilen- und Spaltenindizes (5, 3) angegeben werden
            sheet.FreezePanes(5, 3, 5, 3);
            
            // Die Pane-Sammlung abrufen
            PaneCollection panes = sheet.GetPanes();
            
            // Setze die erste sichtbare Spalte des rechten Panes
            panes.FirstVisibleColumnOfRightPane = 1;
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [PaneCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


