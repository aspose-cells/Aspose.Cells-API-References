---
title: "Style.ForegroundArgbColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Liest und setzt die Vordergrundfarbe mit einem 32-Bit-ARGB-Wert"
type: docs
url: /de/net/aspose.cells/style/foregroundargbcolor/
---
## Style.ForegroundArgbColor property

Liest und setzt die Vordergrundfarbe mit einem 32‑Bit‑ARGB‑Wert.

```csharp
public int ForegroundArgbColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyForegroundArgbColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Stil mit einer bestimmten Vordergrundfarbe
            Style style = workbook.CreateStyle();
            style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
            style.Pattern = BackgroundType.Solid;
            
            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            
            // Lese und zeige den Vordergrund-ARGB-Farbwert an
            int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
            Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
            
            // Speichere die Arbeitsmappe
            workbook.Save("ForegroundColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


