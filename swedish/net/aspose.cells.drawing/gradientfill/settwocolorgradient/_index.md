---
title: "GradientFill.SetTwoColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "GradientFill-metod. Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/settwocolorgradient/
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
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class GradientFillMethodSetTwoColorGradientWithColorColorGradientStyleTyInt32Demo
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

                // Anropa SetTwoColorGradient med realistiska parametrar
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    Color.Blue,         // color2
                    GradientStyleType.DiagonalDown,  // style
                    1);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, Blue, DiagonalDown, 1)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Spara arbetsboken för att demonstrera effekten
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
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

    public class GradientFillMethodSetTwoColorGradientWithColorDoubleColorDoubleGradient297116Demo
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

                // Anropa SetTwoColorGradient med realistiska parametrar
                gradientFill.SetTwoColorGradient(
                    Color.Red,          // color1
                    0.5,                // transparency1 (50% transparent)
                    Color.Blue,         // color2
                    0.3,                // transparency2 (30% transparent)
                    GradientStyleType.Horizontal,  // style
                    2);                 // variant

                Console.WriteLine("SetTwoColorGradient method called successfully with parameters (Red, 0.5, Blue, 0.3, Horizontal, 2)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTwoColorGradient: {ex.Message}");
            }

            // Spara arbetsboken för att demonstrera effekten
            workbook.Save("SetTwoColorGradientWithTransparencyDemo.xlsx");
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [GradientFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


