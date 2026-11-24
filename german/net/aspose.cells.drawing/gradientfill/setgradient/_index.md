---
title: "GradientFill.SetGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "GradientFill-Methode. Setzt den Verlauffülltyp und die Richtung."
type: docs
url: /de/net/aspose.cells.drawing/gradientfill/setgradient/
---
## GradientFill.SetGradient method

Legen Sie den Verlauffülltyp und die Richtung fest.

```csharp
public void SetGradient(GradientFillType type, double angle, GradientDirectionType direction)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Typ | GradientFillType | Verlauffülltyp. |
| angle | Double | Der Winkel. Gilt nur für GradientFillType.Linear. |
| direction | GradientDirectionType | Der Richtungstyp. Gilt nur für GradientFillType.Radial und GradientFillType.Rectangle. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge eine Form hinzu, um einen Farbverlauf anzuwenden
            Shape shape = worksheet.Shapes.AddRectangle(0, 0, 100, 100, 200, 100);

            try
            {
                // Erhalte den Füllverlauf der Form.
                GradientFill gradientFill = shape.Fill.GradientFill; // Fixed property name from Gradient to GradientFill
                if (gradientFill == null)
                {
                    Console.WriteLine("Cannot set gradient: The shape's fill is not a GradientFill.");
                    return;
                }

                // Rufe SetGradient mit spezifischen Parametern auf: lineare Füllung, 90 Grad, FromCenter-Richtung.
                gradientFill.SetGradient(GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter);
                
                Console.WriteLine("SetGradient method executed successfully with parameters (GradientFillType.Linear, 90.0, GradientDirectionType.FromCenter)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetGradient method: {ex.Message}");
            }
            
            // Speichere die Arbeitsmappe, um die Wirkung zu demonstrieren
            workbook.Save("GradientFillSetGradientDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientFillType](../../gradientfilltype/)
* enum [GradientDirectionType](../../gradientdirectiontype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


