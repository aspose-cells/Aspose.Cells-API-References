---
title: "Font.ArgbColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Liest und setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert."
type: docs
url: /de/net/aspose.cells/font/argbcolor/
---
## Font.ArgbColor property

Liest und setzt die Farbe mit einem 32‑Bit‑ARGB‑Wert.

```csharp
public int ArgbColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Greife auf Zellen zu und setze Werte mit unterschiedlichen Schriftfarben.
            Cell cell1 = worksheet.Cells["A1"];
            cell1.PutValue("Red Text");
            Style style1 = cell1.GetStyle();
            style1.Font.ArgbColor = unchecked((int)0xFFFF0000); // Red
            cell1.SetStyle(style1);

            Cell cell2 = worksheet.Cells["A2"];
            cell2.PutValue("Blue Text");
            Style style2 = cell2.GetStyle();
            style2.Font.ArgbColor = unchecked((int)0xFF0000FF); // Blue
            cell2.SetStyle(style2);

            Cell cell3 = worksheet.Cells["A3"];
            cell3.PutValue("Green Text");
            Style style3 = cell3.GetStyle();
            style3.Font.ArgbColor = unchecked((int)0xFF00FF00); // Green
            cell3.SetStyle(style3);

            // Überprüfe und gib die Farben aus.
            Console.WriteLine("Cell A1 Font Color: 0x{0:X8}", worksheet.Cells["A1"].GetStyle().Font.ArgbColor);
            Console.WriteLine("Cell A2 Font Color: 0x{0:X8}", worksheet.Cells["A2"].GetStyle().Font.ArgbColor);
            Console.WriteLine("Cell A3 Font Color: 0x{0:X8}", worksheet.Cells["A3"].GetStyle().Font.ArgbColor);
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


