---
title: "ShadowEffect.Color"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShadowEffect property. Hämtar och anger färgen på skuggan"
type: docs
url: /sv/net/aspose.cells.drawing/shadoweffect/color/
---
## ShadowEffect.Color property

Hämtar och anger färgen på skuggan.

```csharp
public CellsColor Color { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class ShadowEffectPropertyColorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform för att demonstrera skuggeffekten
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Hämta skuggeffekten från formen
                ShadowEffect shadowEffect = shape.ShadowEffect;

                // Skapa ett nytt CellsColor-objekt
                CellsColor shadowColor = workbook.CreateCellsColor();

                // Ställ in färgen till röd med RGB-värden
                shadowColor.Color = Color.Red;

                // Applicera färgen på skuggeffekten
                shadowEffect.Color = shadowColor;

                // Visa det aktuella färgvärdet
                Console.WriteLine("Shadow Color (RGB): " + shadowEffect.Color.Color.ToString());
                Console.WriteLine("Shadow Color (ARGB): " + shadowEffect.Color.Argb);

                // Spara arbetsboken för att demonstrera effekten
                workbook.Save("ShadowEffectColorDemo.xlsx");

                // Läs in arbetsboken igen för att verifiera att färgen sparades
                Workbook loadedWorkbook = new Workbook("ShadowEffectColorDemo.xlsx");
                ShadowEffect loadedShadowEffect = loadedWorkbook.Worksheets[0].Shapes[0].ShadowEffect;

                // Visa det inlästa färgvärdet
                Console.WriteLine("Loaded Shadow Color (RGB): " + loadedShadowEffect.Color.Color.ToString());
                Console.WriteLine("Loaded Shadow Color (ARGB): " + loadedShadowEffect.Color.Argb);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


