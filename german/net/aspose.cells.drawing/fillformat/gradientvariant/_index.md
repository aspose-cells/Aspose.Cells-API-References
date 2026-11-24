---
title: "FillFormat.GradientVariant"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Eigenschaft. Gibt die Farbverlauf-Variante für die angegebene Füllung zurück. Gilt nur für Excel 2007"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/gradientvariant/
---
## FillFormat.GradientVariant property

Gibt die Farbverlaufsvariante für die angegebene Füllung zurück. Gilt nur für Excel 2007.

```csharp
public int GradientVariant { get; }
```

### Hinweise

Kann nur ein Wert von 1 bis 4 sein, entsprechend einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fill Effects. Wenn der Stil GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein.

### Beispiele

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

### Siehe auch

* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


