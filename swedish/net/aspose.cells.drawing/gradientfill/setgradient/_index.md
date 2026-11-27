---
title: "GradientFill.SetGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientFill-metod. Ställ in gradientfyllningstyp och riktning"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/setgradient/
---
## GradientFill.SetGradient method

Ställ in gradientfyllningstyp och riktning.

```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| typ | GradientFillType | Gradientfyllningstyp. |
| angle | Double | Vinkeln. Gäller endast för GradientFillType.Linear. |
| direction | GradientDirectionType | Riktnings typ. Gäller endast för GradientFillType.Radial och GradientFillType.Rectangle. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class GradientFillMethodSetGradientWithGradientFillTypeDoubleGradientDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en shape för att applicera gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);

            try
            {
                // Hämta figurens fyllningsgradient
                GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Anropa SetGradient med specifika parametrar: Linjär fyllning, 90 grader, FromCenter-riktning
                gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
                
                Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
            }
            
            // Spara arbetsboken för att demonstrera effekten
            workbook.Save("GradientFillSetGradientDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


