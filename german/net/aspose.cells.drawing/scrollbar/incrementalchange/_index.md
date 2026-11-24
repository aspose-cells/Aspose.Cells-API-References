---
title: "ScrollBar.IncrementalChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScrollBar-Eigenschaft. Gibt die Menge zurück oder legt sie fest, um die die Bildlaufleiste oder der Spinner bei einem Zeilen-Scroll erhöht wird"
type: docs
url: /de/net/aspose.cells.drawing/scrollbar/incrementalchange/
---
## ScrollBar.IncrementalChange property

Liest oder legt den Betrag fest, um den die Bildlaufleiste oder der Spinner bei einem Zeilen-Scroll erhöht wird.

```csharp
public int IncrementalChange { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyIncrementalChangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine Bildlaufleiste zum Arbeitsblatt hinzufügen
            ScrollBar scrollBar = worksheet.Shapes.AddScrollBar(1, 0, 1, 1, 100, 20);

            // Bildlaufleisten-Eigenschaften festlegen
            scrollBar.Min = 0;
            scrollBar.Max = 100;
            scrollBar.CurrentValue = 50;
            scrollBar.IncrementalChange = 5; // This is the key property we're demonstrating
            scrollBar.PageChange = 20;

            // Zeige die Bildlaufleisten-Eigenschaften an
            Console.WriteLine("Scroll Bar Properties:");
            Console.WriteLine("Min: " + scrollBar.Min);
            Console.WriteLine("Max: " + scrollBar.Max);
            Console.WriteLine("Current Value: " + scrollBar.CurrentValue);
            Console.WriteLine("Incremental Change: " + scrollBar.IncrementalChange);
            Console.WriteLine("Page Change: " + scrollBar.PageChange);

            // Ändere die inkrementelle Änderung
            scrollBar.IncrementalChange = 10;
            Console.WriteLine("\nModified Incremental Change: " + scrollBar.IncrementalChange);

            // Speichere die Arbeitsmappe
            workbook.Save("ScrollBarDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


