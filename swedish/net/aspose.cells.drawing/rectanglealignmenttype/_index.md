---
title: "Enum RectangleAlignmentType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.RectangleAlignmentType enum. Representerar hur man positionerar två rektanglar i förhållande till varandra"
type: docs
url: /sv/net/aspose.cells.drawing/rectanglealignmenttype/
---
## RectangleAlignmentType enumeration

Representerar hur man placerar två rektanglar relativt varandra.

```csharp
public enum RectangleAlignmentType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Bottom | `0` | Botten |
| BottomLeft | `1` | Nedre vänster |
| BottomRight | `2` | Nedre höger |
| Center | `3` | Centrera |
| Left | `4` | Vänster |
| Right | `5` | Höger |
| Top | `6` | Topp |
| TopLeft | `7` | ToppVänster |
| TopRight | `8` | ToppHöger |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassRectangleAlignmentTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en rektangelform för att demonstrera justering
                Shape rectangle = worksheet.Shapes.AddRectangle(1, 0, 0, 200, 100, 100);

                // Demonstrera olika justeringstyper
                Console.WriteLine("Available RectangleAlignmentType values:");
                Console.WriteLine("Bottom: " + RectangleAlignmentType.Bottom);
                Console.WriteLine("BottomLeft: " + RectangleAlignmentType.BottomLeft);
                Console.WriteLine("BottomRight: " + RectangleAlignmentType.BottomRight);
                Console.WriteLine("Center: " + RectangleAlignmentType.Center);
                Console.WriteLine("Left: " + RectangleAlignmentType.Left);
                Console.WriteLine("Right: " + RectangleAlignmentType.Right);
                Console.WriteLine("Top: " + RectangleAlignmentType.Top);
                Console.WriteLine("TopLeft: " + RectangleAlignmentType.TopLeft);
                Console.WriteLine("TopRight: " + RectangleAlignmentType.TopRight);

                // Ställ in justering baserat på ett av enumvärdena
                rectangle.TextHorizontalAlignment = TextAlignmentType.Center;
                rectangle.TextVerticalAlignment = TextAlignmentType.Center;

                // Spara arbetsboken
                workbook.Save("RectangleAlignmentTypeDemo.xlsx");
                Console.WriteLine("RectangleAlignmentType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error demonstrating RectangleAlignmentType: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


