---
title: "Klass GradientFill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.GradientFill-klass. Representerar gradientfyllning"
type: docs
url: /sv/net/aspose.cells.drawing/gradientfill/
---
## GradientFill class

Representerar gradientfyllning.

```csharp
public class GradientFill : Fill
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | Vinkeln för linjär fyllning. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | Hämtar gradientens riktningstyp. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | Hämtar gradientfyllningstypen. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | Representerar samlingen av gradientstopp. |

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Arv från [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Hämtar hashkoden.(Arv från [`Fill`](../fill/).) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | Ställ in gradientfyllningstyp och riktning. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en enfärgsgradient. Gäller endast för Excel 2007. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | Ställer in förinställd temagradientfyllning. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Ställer in den angivna fyllningen till en tvåfärgsgradient. Gäller endast för Excel 2007. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassGradientFillDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform i kalkylbladet med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);

            // Ställ in fyllningstyp till gradient för att komma åt gradientfyllningsegenskaper
            shape.Fill.FillType = FillType.Gradient;

            // Hämta den befintliga gradientfyllningsinstansen från formen
            GradientFill gradientFill = shape.Fill.GradientFill;

            // Konfigurera gradienten med två färger med hjälp av den befintliga instansen
            gradientFill.SetTwoColorGradient(
                Color.LightSkyBlue,  // First color
                Color.DarkBlue,      // Second color
                GradientStyleType.Horizontal, // Gradient style
                1                    // Variant
            );

            // Spara arbetsboken
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Se även

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


