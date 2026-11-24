---
title: "ScrollBar.Max"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScrollBar-Eigenschaft. Gibt den Maximalwert des Bereichs einer Bildlaufleiste oder eines Spinners zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/scrollbar/max/
---
## ScrollBar.Max property

Liest oder legt den Maximalwert eines Bildlaufleisten- oder Spinnerbereichs fest.

```csharp
public int Max { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyMaxDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Bildlaufleiste zum Arbeitsblatt hinzufügen
            Aspose.Cells.Drawing.ScrollBar scrollBar = (Aspose.Cells.Drawing.ScrollBar)worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Bildlaufleisten-Eigenschaften festlegen
            scrollBar.Min = 0;
            scrollBar.Max = 100; // Demonstrating Max property usage
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5;
            scrollBar.PageChange = 10;

            // Speichere die Arbeitsmappe
            workbook.Save("ScrollBarMaxDemo.xlsx");

            // Informationen anzeigen
            Console.WriteLine("ScrollBar created with Max value: " + scrollBar.Max.ToString());
            Console.WriteLine("File saved successfully.");
        }
    }
}
```

### Siehe auch

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


