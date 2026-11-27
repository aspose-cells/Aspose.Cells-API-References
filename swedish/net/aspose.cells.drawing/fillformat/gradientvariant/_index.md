---
title: "FillFormat.GradientVariant"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-egenskap. Returnerar gradientvarianten för den angivna fyllningen. Gäller endast för Excel 2007"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/gradientvariant/
---
## FillFormat.GradientVariant property

Returnerar gradientvarianten för den angivna fyllningen. Gäller endast för Excel 2007.

```csharp
public int GradientVariant { get; }
```

### Anmärkningar

Kan endast vara ett värde från 1 till 4, motsvarande en av de fyra varianterna på Gradient-fliken i dialogrutan Fill Effects. Om stilen är GradientStyle.FromCenter, kan Variant-argumentet endast vara 1 eller 2.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatPropertyGradientVariantDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 200, 150);
            FillFormat fillFormat = rectangle.Fill;
            
            fillFormat.SetTwoColorGradient(Color.LightBlue, Color.DarkBlue, GradientStyleType.Horizontal, 2);
            Console.WriteLine("GradientVariant after SetTwoColorGradient: " + fillFormat.GradientVariant);
            
            fillFormat.SetPresetColorGradient(GradientPresetType.Gold, GradientStyleType.FromCorner, 4);
            Console.WriteLine("GradientVariant after SetPresetColorGradient: " + fillFormat.GradientVariant);
        }
    }
}
```

### Se även

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


