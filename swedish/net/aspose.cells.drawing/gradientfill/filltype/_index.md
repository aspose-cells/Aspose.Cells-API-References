---
title: "GradientFill.FillType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientFill egenskap. Hämtar gradientens fyllningstyp"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/filltype/
---
## GradientFill.FillType property

Hämtar gradientfyllningstypen.

```csharp
public GradientFillType FillType { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class GradientFillPropertyFillTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form med gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            FillFormat fillFormat = shape.Fill;
            fillFormat.FillType = FillType.Gradient;
            
            // Ställ in gradientegenskaper
            GradientFill gradientFill = fillFormat.GradientFill;
            gradientFill.SetTwoColorGradient(System.Drawing.Color.Red, System.Drawing.Color.Blue, GradientStyleType.Horizontal, 1);
            
            // Visa gradientens fyllningstyp
            Console.WriteLine("Gradient Fill Type: " + gradientFill.FillType);
            
            // Ändra till radiell gradient
            gradientFill.SetGradient(GradientFillType.Radial, 45, GradientDirectionType.FromCenter);
            Console.WriteLine("Updated Gradient Fill Type: " + gradientFill.FillType);
            
            // Spara arbetsboken
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientFillType](../../gradientfilltype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


