---
title: "TwoColorGradient.Variant"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TwoColorGradient-egenskap. Hämtar och anger gradientvarianten"
type: docs
url: /sv/net/aspose.cells/twocolorgradient/variant/
---
## TwoColorGradient.Variant property

Hämtar och anger gradientvarianten.

```csharp
public int Variant { get; set; }
```

### Exempel

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

            // Skapa tvåfärgsgradient med initial variant
            TwoColorGradient gradient = new TwoColorGradient(
                Color.LightBlue,
                Color.DarkBlue,
                GradientStyleType.Horizontal,
                1
            );

            // Skapa och tillämpa stil på cell A1
            Style style1 = workbook.CreateStyle();
            style1.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Variant 1");

            // Visa aktuellt variantvärde
            System.Console.WriteLine("Current Variant value: " + gradient.Variant);

            // Ändra variantvärde
            gradient.Variant = 2;

            // Skapa och tillämpa modifierad stil på cell B1
            Style style2 = workbook.CreateStyle();
            style2.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Variant 2");

            // Gör cellerna högre för att visualisera gradienter
            worksheet.Cells.Rows[0].Height = 150;

            workbook.Save("TwoColorGradientVariantDemo.xlsx");
        }
    }
}
```

### Se även

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


