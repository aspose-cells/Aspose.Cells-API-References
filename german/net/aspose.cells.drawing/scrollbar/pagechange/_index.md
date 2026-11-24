---
title: "ScrollBar.PageChange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ScrollBar-Eigenschaft. Gibt den Seitenwechsel zurück oder legt ihn fest"
type: docs
url: /de/net/aspose.cells.drawing/scrollbar/pagechange/
---
## ScrollBar.PageChange property

Liest oder legt den Seitenwechsel fest

```csharp
public int PageChange { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ScrollBarPropertyPageChangeDemo
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
            scrollBar.IncrementalChange = 1;
            scrollBar.PageChange = 10; // Demonstrate PageChange property
            scrollBar.LinkedCell = "A1";

            // Speichere die Arbeitsmappe
            workbook.Save("ScrollBarPropertyPageChangeDemo.xlsx");

            // Laden der gespeicherten Arbeitsmappe, um Eigenschaften zu überprüfen
            Workbook verifyWorkbook = new Workbook("ScrollBarPropertyPageChangeDemo.xlsx");
            ScrollBar verifyScrollBar = (ScrollBar)verifyWorkbook.Worksheets[0].Shapes[0];

            // Gib den Wert der PageChange-Eigenschaft aus, um zu zeigen, dass er korrekt gespeichert/geladen wurde
            Console.WriteLine("ScrollBar PageChange value: " + verifyScrollBar.PageChange);
        }
    }
}
```

### Siehe auch

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


