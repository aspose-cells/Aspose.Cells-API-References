---
title: "FillFormat.SetTwoColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FillFormat-metod. Anger den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007"
type: docs
url: /sv/net/aspose.cells.drawing/fillformat/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | Färg | En gradientfärg. |
| color2 | Färg | Två gradientfärger. |
| style | GradientStyleType | Gradientskuggningsstil. |
| variant | Int32 | Gradientvarianten. Kan vara ett värde från 1 till 4, motsvarande en av de fyra varianterna på fliken Gradient i dialogrutan Fylleffekter. Om stil är GradientStyle.FromCenter, kan Variant‑argumentet endast vara 1 eller 2. |

### Exempel

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FillFormatMethodSetTwoColorGradientWithColorColorGradientStyleTypeIntDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en enkel form för att demonstrera gradientfyllning
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 100, 100);

            // Hämta fyllningsformatet för formen
            FillFormat fillFormat = shape.Fill;

            // Ställ in tvåfärgsgradient med angivna parametrar
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);

            // Spara arbetsboken
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| color1 | Färg | En gradientfärg. |
| transparency1 | Double | Grad av transparens för färg1 som ett värde från 0.0 (opak) till 1.0 (klar). |
| color2 | Färg | Två gradientfärger. |
| transparency2 | Double | Grad av transparens för färg2 som ett värde från 0.0 (opak) till 1.0 (klar). |
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

    public class FillFormatMethodSetTwoColorGradientWithColorDoubleColorDoubleGradientDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en rektangulär form för att demonstrera fyllningsformatering
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 150, 100);
            FillFormat fillFormat = rectangle.Fill;

            try
            {
                // Förbered parametrar för SetTwoColorGradient
                Color color1 = Color.Red;
                double transparency1 = 0.3;
                Color color2 = Color.Blue;
                double transparency2 = 0.7;
                GradientStyleType gradientStyle = GradientStyleType.Horizontal;
                int variant = 1;

                // Anropa SetTwoColorGradient med specifika parametrar
                fillFormat.SetTwoColorGradient(
                    color1, 
                    transparency1, 
                    color2, 
                    transparency2, 
                    gradientStyle, 
                    variant
                );

                Console.WriteLine("SetTwoColorGradient executed successfully with parameters (Color, Double, Color, Double, GradientStyleType, Int32)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTwoColorGradient: {ex.Message}");
            }

            // Spara arbetsboken för att visa effekten
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


