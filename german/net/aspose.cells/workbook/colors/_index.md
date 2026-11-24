---
title: "Workbook.Colors"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Eigenschaft. Gibt die Farben in der Palette für die Tabellenkalkulation zurück"
type: docs
url: /de/net/aspose.cells/workbook/colors/
---
## Workbook.Colors property

Gibt Farben in der Palette für die Tabelle zurück.

```csharp
public Color[] Colors { get; }
```

### Hinweise

Die Palette hat 56 Einträge, jeder dargestellt durch einen RGB-Wert.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class WorkbookPropertyColorsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();

            // Auf die Standardfarbpalette zugreifen
            Color[] colors = workbook.Colors;

            // Einige Farben in der Palette ändern
            colors[0] = System.Drawing.Color.Red;      // Modify first color to Red
            colors[1] = System.Drawing.Color.Green;    // Modify second color to Green
            colors[2] = System.Drawing.Color.Blue;    // Modify third color to Blue

            // Erstellen Sie ein Arbeitsblatt und fügen Sie einige Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Color Demo");
            
            // Die geänderten Farben auf Zellen anwenden
            Style style1 = workbook.CreateStyle();
            style1.ForegroundColor = colors[0];
            style1.Pattern = BackgroundType.Solid;
            worksheet.Cells["A2"].SetStyle(style1);
            
            Style style2 = workbook.CreateStyle();
            style2.ForegroundColor = colors[1];
            style2.Pattern = BackgroundType.Solid;
            worksheet.Cells["B2"].SetStyle(style2);
            
            Style style3 = workbook.CreateStyle();
            style3.ForegroundColor = colors[2];
            style3.Pattern = BackgroundType.Solid;
            worksheet.Cells["C2"].SetStyle(style3);

            // Speichere die Arbeitsmappe
            workbook.Save("WorkbookColorsDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


