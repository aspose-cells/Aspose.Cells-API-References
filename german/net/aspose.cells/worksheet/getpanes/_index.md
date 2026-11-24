---
title: "Worksheet.GetPanes"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Gibt die Fensterbereiche zurück"
type: docs
url: /de/net/aspose.cells/worksheet/getpanes/
---
## Worksheet.GetPanes method

Liest die Fensterbereiche.

```csharp
public PaneCollection GetPanes()
```

### Hinweise

Falls das Fenster nicht geteilt oder fixiert ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetPanesDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Bereiche bei Zeile 5 und Spalte 3 fixieren
            worksheet.FreezePanes(5, 3, 5, 3);
            
            // Bereichsinformationen abrufen
            PaneCollection panes = worksheet.GetPanes();
            
            // Bereichsinformationen anzeigen
            Console.WriteLine("First visible row of bottom pane: " + panes.FirstVisibleRowOfBottomPane);
            Console.WriteLine("First visible column of right pane: " + panes.FirstVisibleColumnOfRightPane);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [PaneCollection](../../panecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


