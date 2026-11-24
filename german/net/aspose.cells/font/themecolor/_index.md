---
title: "Font.ThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Schriftart-Eigenschaft. Gibt die Themenfarbe zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/font/themecolor/
---
## Font.ThemeColor property

Liest und setzt die Themenfarbe.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Hinweise

Wenn die Schriftfarbe keine Themenfarbe ist, wird NULL zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FontPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf Zelle A1 zu und setzen Sie den Text
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Theme Color Demo");

            // Holen Sie den Stil und die Schriftart
            Style style = cell.GetStyle();
            Font font = style.Font;

            // Erstellen und setzen Sie die Themenfarbe
            font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);

            // Wenden Sie den Stil auf die Zelle an
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("ThemeColorDemo.xlsx");

            // Überprüfen Sie die Themenfarbe
            Font savedFont = worksheet.Cells["A1"].GetStyle().Font;
            Console.WriteLine("ThemeColor Type: " + savedFont.ThemeColor.ColorType);
            Console.WriteLine("ThemeColor Tint: " + savedFont.ThemeColor.Tint);
        }
    }
}
```

### Siehe auch

* class [ThemeColor](../../themecolor/)
* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


