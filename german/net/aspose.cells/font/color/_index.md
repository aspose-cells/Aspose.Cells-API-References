---
title: "Font.Color"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Font-Eigenschaft. Liest oder setzt die Farbe der Schrift."
type: docs
url: /de/net/aspose.cells/font/color/
---
## Font.Color property

Ruft die Farbe der Schrift ab oder legt sie fest.

```csharp
public Color Color { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze HTML mit verschiedenen Schriftfarben und -stilen.
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font><font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
            
            // Hole die Rich-Text-Formatierung.
            FontSetting[] richText = cell.GetCharacters();
            
            // Überprüfe und demonstriere Farbeigenschaften.
            Console.WriteLine("First segment color: " + richText[0].Font.Color);
            Console.WriteLine("Second segment color: " + richText[1].Font.Color);
            Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
            
            // Speichere die Arbeitsmappe
            workbook.Save("FontColorDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


