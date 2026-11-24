---
title: "TwoColorGradient.Color1"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TwoColorGradient-Eigenschaft. Gibt die erste Verlauffarbe zurück und setzt sie"
type: docs
url: /de/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

Liest und setzt die erste Verlauffarbe.

```csharp
public Color Color1 { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor1Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Stil mit Farbverlauf erstellen
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // Zweifarbigen Farbverlauf initialisieren
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // Farbverlauf auf Zellenstil anwenden
            cell.SetStyle(style);
            
            // Anfangsfarbe auslesen
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // Farbverlauffarbe ändern und erneut anwenden
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // Aktualisierung überprüfen
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // Visuelle Demonstration in Ausgabedatei
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


