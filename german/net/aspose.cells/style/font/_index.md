---
title: "Style.Font"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt ein Font-Objekt zurück"
type: docs
url: /de/net/aspose.cells/style/font/
---
## Style.Font property

Gibt ein `Font`-Objekt zurück.

```csharp
public Font Font { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyFontDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Greifen Sie auf Zelle B4 zu und setzen Sie deren Schrift auf fett.
            Cell b4 = cells["B4"];
            Style b4Style = b4.GetStyle();
            b4Style.Font.IsBold = true;
            b4.SetStyle(b4Style);

            // Greifen Sie auf Zelle C4 zu und stellen Sie sicher, dass deren Schrift nicht fett ist.
            Cell c4 = cells["C4"];
            Style c4Style = c4.GetStyle();
            c4Style.Font.IsBold = false;
            c4.SetStyle(c4Style);

            // Greifen Sie auf Zelle D4 zu und setzen Sie deren Schrift auf fett mit einer anderen Farbe.
            Cell d4 = cells["D4"];
            Style d4Style = d4.GetStyle();
            d4Style.Font.IsBold = true;
            d4Style.Font.Color = Color.Red;
            d4.SetStyle(d4Style);

            // Überprüfen Sie die Schriftart-Eigenschaften.
            Console.WriteLine("B4 Font Bold: " + b4.GetStyle().Font.IsBold);
            Console.WriteLine("C4 Font Bold: " + c4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Bold: " + d4.GetStyle().Font.IsBold);
            Console.WriteLine("D4 Font Color: " + d4.GetStyle().Font.Color);

            // Speichere die Arbeitsmappe
            workbook.Save("FontPropertyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Font](../../font/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


