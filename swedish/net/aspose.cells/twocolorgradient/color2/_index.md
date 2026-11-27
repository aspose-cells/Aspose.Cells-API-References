---
title: "TwoColorGradient.Color2"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TwoColorGradient-egenskap. Hämtar och anger den andra gradientfärgen"
type: docs
url: /sv/net/aspose.cells/twocolorgradient/color2/
---
## TwoColorGradient.Color2 property

Hämtar och anger den andra gradientfärgen.

```csharp
public Color Color2 { get; set; }
```

### Exempel

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
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en tvåfärgsgradient-instans
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.Green,
                GradientStyleType.Horizontal,
                1);

            // Skapa första stil med initial gradient
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].PutValue("Initial Gradient");
            worksheet.Cells["A1"].SetStyle(style1);

            // Visa aktuellt Color2-värde
            System.Console.WriteLine("Current Color2: " + gradient.Color2);

            // Ändra Color2-egenskap
            gradient.Color2 = Color.Red;

            // Skapa andra stil med modifierad gradient
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A2"].PutValue("Modified Gradient");
            worksheet.Cells["A2"].SetStyle(style2);

            // Justera rader för synlighet
            worksheet.Cells.SetRowHeight(0, 40);
            worksheet.Cells.SetRowHeight(1, 40);

            // Spara arbetsboken
            workbook.Save("TwoColorGradientColor2Demo.xlsx");
        }
    }
}
```

### Se även

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


