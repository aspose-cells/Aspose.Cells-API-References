---
title: "ScrollBar.CurrentValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScrollBar-Eigenschaft. Gibt den aktuellen Wert zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/scrollbar/currentvalue/
---
## ScrollBar.CurrentValue property

Liest oder legt den aktuellen Wert fest.

```csharp
public int CurrentValue { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyCurrentValueDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Bildlaufleiste zum Arbeitsblatt hinzufügen
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Bildlaufleisten-Eigenschaften mit den korrekten Eigenschaftsnamen festlegen
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;

            // CurrentValue-Eigenschaft festlegen und demonstrieren
            scrollBar.CurrentValue = 50;
            Console.WriteLine("ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Den aktuellen Wert ändern
            scrollBar.CurrentValue = 75;
            Console.WriteLine("Updated ScrollBar CurrentValue: " + scrollBar.CurrentValue);

            // Speichere die Arbeitsmappe
            workbook.Save("ScrollBarCurrentValueDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


