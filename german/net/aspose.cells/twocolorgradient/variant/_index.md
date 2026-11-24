---
title: "TwoColorGradient.Variant"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TwoColorGradient-Eigenschaft. Gibt und setzt die Gradientvariante"
type: docs
url: /de/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

Liest und setzt die Verlaufvariante.

```csharp
public int Variant { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class TwoColorGradientPropertyVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Zweifarbigen Verlauf mit anfänglicher Variante erstellen
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // Stil erstellen und auf Zelle A1 anwenden
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // Aktuellen Variantenwert anzeigen
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // Variantenwert ändern
            gradient.Variant = 2;

            // Erstelle und wende den modifizierten Stil auf Zelle B1 an
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // Zellen höher machen, um Verläufe zu visualisieren
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


