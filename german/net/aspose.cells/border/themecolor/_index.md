---
title: "Border.ThemeColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Border-Eigenschaft. Gibt die Themenfarbe des Rahmens zurück und legt sie fest"
type: docs
url: /de/net/aspose.cells/border/themecolor/
---
## Border.ThemeColor property

Liest und setzt die Designfarbe des Rands.

```csharp
public ThemeColor ThemeColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class BorderPropertyThemeColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf eine Zelle zu und rufen Sie ihren Stil ab
            Style style = worksheet.Cells["A1"].GetStyle();

            // Setzen Sie die Themenfarbe des Rahmens
            style.Borders[BorderType.BottomBorder].ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;

            // Wenden Sie den Stil auf die Zelle an
            worksheet.Cells["A1"].SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("BorderThemeColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [ThemeColor](../../themecolor/)
* class [Border](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


