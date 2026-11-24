---
title: "StyleFlag.Borders"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Alle Rahmen-Einstellungen werden angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/borders/
---
## StyleFlag.Borders property

Alle Rahmen-Einstellungen werden angewendet.

```csharp
public bool Borders { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyBordersDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Erstelle einen Stil mit Rahmen-Einstellungen
            Style style = workbook.CreateStyle();
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.TopBorder].Color = System.Drawing.Color.Red;
            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Thin;
            style.Borders[BorderType.BottomBorder].Color = System.Drawing.Color.Blue;

            // Erstelle ein StyleFlag und aktiviere Rahmen
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;

            // Wende den Stil auf Zelle A1 nur mit Rahmen an
            cells["A1"].PutValue("Borders Demo");
            cells["A1"].SetStyle(style, styleFlag);

            // Speichere die Arbeitsmappe
            workbook.Save("BordersDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


