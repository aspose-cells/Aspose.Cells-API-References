---
title: "ScrollBar.Shadow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScrollBar-Eigenschaft. Gibt an, ob die Form 3D-Schattierung hat"
type: docs
url: /de/net/aspose.cells.drawing/scrollbar/shadow/
---
## ScrollBar.Shadow property

Gibt an, ob die Form 3‑D‑Schattierung hat.

```csharp
public bool Shadow { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyShadowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine horizontale Bildlaufleiste hinzu
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);
            
            // Bildlaufleisten-Eigenschaften festlegen
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 20;
            scrollBar.CurrentValue = 50;
            scrollBar.IsHorizontal = true;
            
            // Shadow-Eigenschaft demonstrieren
            scrollBar.Shadow = true; // Enable 3D shadow effect
            
            // Erstelle eine weitere Bildlaufleiste zum Vergleich
            ScrollBar scrollBar2 = worksheet.Shapes.AddScrollBar(1, 2, 1, 1, 100, 20);
            scrollBar2.Shadow = false; // No shadow
            
            // Speichere die Arbeitsmappe
            workbook.Save("ScrollBarShadowDemo.xlsx");
            
            Console.WriteLine("ScrollBar Shadow demo completed. Check output file.");
        }
    }
}
```

### Siehe auch

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


