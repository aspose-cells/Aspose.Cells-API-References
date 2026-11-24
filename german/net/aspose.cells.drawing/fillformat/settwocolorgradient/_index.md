---
title: "FillFormat.SetTwoColorGradient"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FillFormat-Methode. Setzt die angegebene Füllung auf einen zweifarbigen Farbverlauf. Gilt nur für Excel 2007"
type: docs
url: /de/net/aspose.cells.drawing/fillformat/settwocolorgradient/
---
## SetTwoColorGradient(Color, Color, GradientStyleType, int) {#settwocolorgradient_1}

Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, Color color2, GradientStyleType style, int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | Farbe | Eine Gradientfarbe. |
| color2 | Farbe | Zwei Gradientfarben. |
| Stil | GradientStyleType | Gradient-Schattierungsstil. |
| Variante | Int32 | Die Gradientvariante. Kann einen Wert von 1 bis 4 haben, der einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fill Effects entspricht. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### Beispiele

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

            // Erstelle eine einfache Form, um den Farbverlauf zu demonstrieren.
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 100, 100);

            // Lese das Füllformat der Form.
            FillFormat fillFormat = shape.Fill;

            // Setze zweifarbigen Farbverlauf mit angegebenen Parametern.
            fillFormat.SetTwoColorGradient(Color.Blue, Color.LightBlue, GradientStyleType.DiagonalDown, 1);

            // Speichere die Arbeitsmappe
            workbook.Save("TwoColorGradientDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)

---

## SetTwoColorGradient(Color, double, Color, double, GradientStyleType, int) {#settwocolorgradient}

Setzt die angegebene Füllung auf einen Zweifarbverlauf. Gilt nur für Excel 2007.

```csharp
public void SetTwoColorGradient(Color color1, double transparency1, Color color2, 
    double transparency2, GradientStyleType style, int variant)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| color1 | Farbe | Eine Gradientfarbe. |
| transparency1 | Double | Der Transparenzgrad von Farbe1 als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| color2 | Farbe | Zwei Gradientfarben. |
| transparency2 | Double | Der Transparenzgrad von Farbe2 als Wert von 0,0 (undurchsichtig) bis 1,0 (transparent). |
| Stil | GradientStyleType | Gradient-Schattierungsstil. |
| Variante | Int32 | Die Gradientvariante. Kann einen Wert von 1 bis 4 haben, der einer der vier Varianten auf der Registerkarte Gradient im Dialogfeld Fill Effects entspricht. Wenn style GradientStyle.FromCenter ist, kann das Variant-Argument nur 1 oder 2 sein. |

### Beispiele

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
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Erstelle ein Rechteck-Shape, um die Füllformatierung zu demonstrieren.
            var rectangle = worksheet.Shapes.AddRectangle(1, 0, 1, 5, 150, 100);
            FillFormat fillFormat = rectangle.Fill;

            try
            {
                // Bereite Parameter für SetTwoColorGradient vor.
                Color color1 = Color.Red;
                double transparency1 = 0.3;
                Color color2 = Color.Blue;
                double transparency2 = 0.7;
                GradientStyleType gradientStyle = GradientStyleType.Horizontal;
                int variant = 1;

                // Rufe SetTwoColorGradient mit spezifischen Parametern auf.
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

            // Arbeitsmappe speichern, um den Effekt zu zeigen
            workbook.Save("SetTwoColorGradientDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [GradientStyleType](../../gradientstyletype/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


