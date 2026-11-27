---
title: "Klass Fill"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.Fill-klass. Representerar fyllningsformatet för formen"
type: docs
url: /sv/net/aspose.cells.drawing/fill/
---
## Fill class

Representerar fyllningsformatet för formen.

```csharp
public abstract class Fill
```

## Metoder

| Namn | Beskrivning |
| --- | --- |
| override [Equals](../../aspose.cells.drawing/fill/equals/)(object) | / |
| override [GetHashCode](../../aspose.cells.drawing/fill/gethashcode/)() | Hämtar hash‑koden. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System.Drawing;

    public class DrawingClassFillDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Shape rectangle = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 150);
            // Ställ in fyllningstyp till solid och ändra färg
            rectangle.Fill.FillType = FillType.Solid;
            rectangle.Fill.SolidFill.Color = Color.LightBlue;

            Shape oval = worksheet.Shapes.AddOval(2, 0, 0, 0, 100, 150);
            // Använd gradientfyllningsmetod direkt på FillFormat
            oval.Fill.SetTwoColorGradient(Color.DarkBlue, Color.SkyBlue, GradientStyleType.Vertical, 0);

            workbook.Save("DrawingClassFillDemo.xlsx");
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


