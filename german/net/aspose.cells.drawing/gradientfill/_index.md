---
title: "Klasse GradientFill"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.GradientFill-Klasse. Stellt die Verlauffüllung dar"
type: docs
url: /de/net/aspose.cells.drawing/gradientfill/
---
## GradientFill class

Stellt die Farbverlauffüllung dar.

```csharp
public class GradientFill : Fill
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Angle](../../aspose.cells.drawing/gradientfill/angle/) { get; set; } | Der Winkel der linearen Füllung. |
| [DirectionType](../../aspose.cells.drawing/gradientfill/directiontype/) { get; } | Liest den Verlauf-Richtungstyp. |
| [FillType](../../aspose.cells.drawing/gradientfill/filltype/) { get; } | Liest den Verlauf-Fülltyp. |
| [GradientStops](../../aspose.cells.drawing/gradientfill/gradientstops/) { get; } | Stellt die Sammlung von Gradient-Stops dar. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | /(Geerbt von [`Fill`](../fill/).) |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Liest den Hash‑Code. (Geerbt von [`Fill`](../fill/).) |
| [SetGradient](../../aspose.cells.drawing/gradientfill/setgradient/)(GradientFillType, double, GradientDirectionType) | Legen Sie den Verlauffülltyp und die Richtung fest. |
| [SetOneColorGradient](../../aspose.cells.drawing/gradientfill/setonecolorgradient/)(Color, double, GradientStyleType, int) | Setzt die angegebene Füllung auf einen einfarbigen Farbverlauf. Gilt nur für Excel 2007. |
| [SetPresetThemeGradient](../../aspose.cells.drawing/gradientfill/setpresetthemegradient/)(PresetThemeGradientType, ThemeColorType) | Legt die voreingestellte Themenverlauffüllung fest. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient_1)(Color, Color, GradientStyleType, int) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007. |
| [SetTwoColorGradient](../../aspose.cells.drawing/gradientfill/settwocolorgradient/#settwocolorgradient)(Color, double, Color, double, GradientStyleType, int) | Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie dem Arbeitsblatt eine Rechteckform mit allen erforderlichen Parametern hinzu
            Shape shape = worksheet.Shapes.AddRectangle(5, 5, 0, 0, 150, 100);

            // Setzen Sie den Fülltyp auf Verlauf, um auf die Eigenschaften der Verlauffüllung zuzugreifen
            shape.Fill.FillType = FillType.Gradient;

            // Holen Sie die vorhandene Verlauffüllungsinstanz aus der Form
            GradientFill gradientFill = shape.Fill.GradientFill;

            // Konfigurieren Sie den Verlauf mit zwei Farben unter Verwendung der vorhandenen Instanz
            gradientFill.SetTwoColorGradient(
                Color.LightSkyBlue,  // First color
                Color.DarkBlue,      // Second color
                GradientStyleType.Horizontal, // Gradient style
                1                    // Variant
            );

            // Speichere die Arbeitsmappe
            workbook.Save("GradientFillDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Fill](../fill/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


