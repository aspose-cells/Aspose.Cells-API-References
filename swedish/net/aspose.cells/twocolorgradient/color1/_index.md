---
title: "TwoColorGradient.Color1"
second_title: "Aspose.Cells för .NET API‑referens"
description: "TwoColorGradient-egenskap. Hämtar och anger den första gradientfärgen"
type: docs
url: /sv/net/aspose.cells/twocolorgradient/color1/
---
## TwoColorGradient.Color1 property

Hämtar och anger den första gradientfärgen.

```csharp
public Color Color1 { get; set; }
```

### Exempel

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
            
            // Skapa stil med gradientfyllning
            Style style = workbook.CreateStyle();
            style.Pattern = BackgroundType.Solid;
            
            // Initiera tvåfärgsgradient
            style.SetTwoColorGradient(
                Color.Red,
                Color.Blue,
                GradientStyleType.Vertical,
                variant: 1);
            
            // Applicera gradient på cellstil
            cell.SetStyle(style);
            
            // Läs initial färg
            TwoColorGradient gradient = style.GetTwoColorGradientSetting();
            Console.WriteLine("Current Color1 value: " + gradient.Color1);
            
            // Modifiera gradientfärg och återapplicera
            gradient.Color1 = Color.Lime;
            style.SetTwoColorGradient(gradient.Color1, gradient.Color2, gradient.GradientStyleType, gradient.Variant);
            
            // Verifiera uppdatering
            Console.WriteLine("Updated Color1 value: " + gradient.Color1);
            
            // Visuell demonstration i utdatafilen
            cell.PutValue("Color1 Gradient Demo");
            worksheet.AutoFitColumn(0);
            workbook.Save("TwoColorGradientPropertyColor1Demo.xlsx");
        }
    }
}
```

### Se även

* class [TwoColorGradient](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


