---
title: "Cells.GetViewRowHeight"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die Höhe einer angegebenen Zeile zurück"
type: docs
url: /de/net/aspose.cells/cells/getviewrowheight/
---
## Cells.GetViewRowHeight method

Gibt die Höhe einer angegebenen Zeile zurück.

```csharp
public double GetViewRowHeight(int row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Int32 | Zeilenindex. |

### Rückgabewert

Zeilenhöhe.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetViewRowHeightWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zeilenhöhe für Zeile 3 (in Punkten) festlegen
            worksheet.Cells.SetRowHeight(3, 15);
            
            // Ermitteln Sie die Ansichtshöhe der Zeile 3
            double viewRowHeight = worksheet.Cells.GetViewRowHeight(3);
            
            // Gib das Ergebnis aus
            Console.WriteLine("View Row Height for row 3: " + viewRowHeight);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


