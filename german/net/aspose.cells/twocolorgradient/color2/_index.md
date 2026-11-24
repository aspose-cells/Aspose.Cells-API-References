---
title: "TwoColorGradient.Color2"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TwoColorGradient-Eigenschaft. Gibt die zweite Verlauffarbe zurück und setzt sie"
type: docs
url: /de/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

Liest und setzt die zweite Verlauffarbe.

```csharp
public Color Color2 { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyColor2Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle eine Instanz eines zweifarbigen Verlaufs
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // Erstelle den ersten Stil mit dem Anfangsverlauf
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // Aktuellen Color2-Wert anzeigen
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // Color2-Eigenschaft ändern
            gradient.Color2 = Color.Red;

            // Erstelle den zweiten Stil mit dem modifizierten Verlauf
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // Zeilen für Sichtbarkeit anpassen
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // Speichere die Arbeitsmappe
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


