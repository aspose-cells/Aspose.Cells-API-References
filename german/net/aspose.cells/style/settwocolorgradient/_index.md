---
title: "Style.SetTwoColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Methode. Legt die angegebene Füllung als Zweifarbverlauf fest"
type: docs
url: /de/net/aspose.cells/style/settwocolorgradient/
---
## Style.SetTwoColorGradient method

Setzt die angegebene Füllung auf einen Zweifarbverlauf.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType gradientStyleType, 
    int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | Farbe | Eine Gradientfarbe. |
| color2 | Farbe | Zwei Gradientfarben. |
| gradientStyleType | GradientStyleType | Gradient-Schattierungsstil. |
| Variante | Int32 | Die Gradientvariante. Kann einen Wert von 1 bis 4 haben, der einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fill Effects entspricht. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### Beispiele

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class StyleMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstellen Sie ein Stilobjekt
            Style style = workbook.CreateStyle();

            // Setze einen Zweifarbverlauf für den Stil
            style.SetTwoColorGradient(Color.Green, Color.Red, GradientStyleType.Vertical, 1);

            // Wende den Stil auf eine Zelle an
            Cell cell = worksheet.Cells["A1"];
            cell.SetStyle(style);
            cell.PutValue("Gradient Style Demo");

            // Überprüfe die Gradienteneinstellungen
            Color color1, color2;
            GradientStyleType gradientStyle;
            int variant;
            style.GetTwoColorGradient(out color1, out color2, out gradientStyle, out variant);

            Console.WriteLine("Color1: " + color1);
            Console.WriteLine("Color2: " + color2);
            Console.WriteLine("Gradient Style: " + gradientStyle);
            Console.WriteLine("Variant: " + variant);

            // Speichere die Arbeitsmappe
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientStyleType](../../../aspose.cells.drawing/gradientstyletype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


