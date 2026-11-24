---
title: "ScrollBar.Min"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScrollBar-Eigenschaft. Gibt den Minimalwert einer Bildlaufleiste oder eines Drehfeldbereichs zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/scrollbar/min/
---
## ScrollBar.Min property

Liest oder legt den Minimalwert eines Bildlaufleisten- oder Spinnerbereichs fest.

```csharp
public int Min { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMinDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Bildlaufleiste zum Arbeitsblatt hinzufügen
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Bildlaufleisten-Eigenschaften festlegen
            scrollBar.Min = 10;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;  // Changed from Value to CurrentValue
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // Den Wert der Min-Eigenschaft anzeigen
            Console.WriteLine("ScrollBar Min Value: " + scrollBar.Min);

            // Speichere die Arbeitsmappe
            workbook.Save("ScrollBarMinDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


