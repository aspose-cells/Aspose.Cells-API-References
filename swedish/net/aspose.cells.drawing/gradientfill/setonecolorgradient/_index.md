---
title: "GradientFill.SetOneColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientFill method. Anger den specificerade fyllningen till en enfärgsgradient. Gäller endast för Excel 2007"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/setonecolorgradient/
---
## GradientFill.SetOneColorGradient method

Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast för Excel 2007.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| färg | Färg | En gradientfärg. |
| grad | Double | Gradientens grad. Kan vara ett värde från 0,0 (mörk) till 1,0 (ljus). |
| style | GradientStyleType | Gradientskuggningsstil. |
| variant | Int32 | Gradientvarianten. Kan vara ett värde från 1 till 4, motsvarande en av de fyra varianterna på fliken Gradient i dialogrutan Fylleffekter. Om stil är GradientStyle.FromCenter, kan Variant‑argumentet endast vara 1 eller 2. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en shape för att applicera gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Ställ in fyllningstypen till gradient
                shape.Fill.FillType = FillType.Gradient;

                // Hämta gradientfyllningen
                GradientFill gradientFill = shape.Fill.GradientFill;
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Anropa SetOneColorGradient med realistiska parametrar
                gradientFill.SetOneColorGradient(
                    Color.Green,        // color
                    0.7,                // degree (70% intensity)
                    GradientStyleType.DiagonalUp,  // style
                    1);                 // variant

                Console.WriteLine("SetOneColorGradient method called successfully with parameters (Green, 0.7, DiagonalUp, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }

            // Spara arbetsboken för att demonstrera effekten
            workbook.Save("SetOneColorGradientDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


