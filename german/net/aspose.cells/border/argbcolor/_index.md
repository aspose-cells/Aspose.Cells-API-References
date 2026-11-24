---
title: "Border.ArgbColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Border-Eigenschaft. Gibt die Farbe zurück und legt sie mit einem 32‑Bit‑ARGB‑Wert fest"
type: docs
url: /de/net/aspose.cells/border/argbcolor/
---
## Border.ArgbColor property

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
    public class BorderPropertyArgbColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf die Zelle B2 zu und setzen Sie einen Wert
            Cell cell = worksheet.Cells["B2"];
            cell.PutValue("Border ARGB Color Demo");

            // Rufen Sie den Stil und die Rahmen ab
            Style style = cell.GetStyle();
            Border border = style.Borders[BorderType.TopBorder];

            // Setzen Sie Rahmen-Eigenschaften einschließlich ARGB‑Farbe
            border.LineStyle = CellBorderType.Thick;
            unchecked
            {
                border.ArgbColor = (int)0xFFFF0000; // Red color in ARGB format with unchecked cast
            }

            // Wende den geänderten Stil auf die Zelle an
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("BorderArgbColorDemo.xlsx");

            // Überprüfen Sie, ob die ARGB‑Farbe korrekt gesetzt wurde
            Border savedBorder = workbook.Worksheets[0].Cells["B2"].GetStyle().Borders[BorderType.TopBorder];
            Console.WriteLine("ARGB Color of top border: " + savedBorder.ArgbColor.ToString("X8"));
        }
    }
}
```

### Siehe auch

* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


