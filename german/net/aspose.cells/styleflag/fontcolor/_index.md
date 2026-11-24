---
title: "StyleFlag.FontColor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "StyleFlag-Eigenschaft. Die Einstellung für die Schriftfarbe wird angewendet"
type: docs
url: /de/net/aspose.cells/styleflag/fontcolor/
---
## StyleFlag.FontColor property

Die Einstellung für die Schriftfarbe wird angewendet.

```csharp
public bool FontColor { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyFontColorDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie einen benutzerdefinierten Stil.
            Style style = workbook.CreateStyle();
            style.Font.Color = System.Drawing.Color.Red;
            style.BackgroundColor = System.Drawing.Color.LightGray;
            
            // Erstelle ein StyleFlag und aktiviere Schriftfarbe und Zellenhintergrund
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.FontColor = true;
            styleFlag.CellShading = true;
            
            // Wende den Stil auf Zelle A1 mit den angegebenen Flags an
            worksheet.Cells["A1"].PutValue("Red Text on Gray Background");
            worksheet.Cells["A1"].SetStyle(style, styleFlag);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


