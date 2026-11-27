---
title: "ShapePath.HeightPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath egenskap. Hämtar höjden på den här banan i enhet pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/heightpixel/
---
## ShapePath.HeightPixel property

Hämtar höjden på denna bana i enhet pixlar.

```csharp
public int HeightPixel { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyHeightPixelDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en ny formbana
                ShapePath shapePath = new ShapePath();

                // Skapa en enkel rektangelbana
                shapePath.MoveTo(10, 10);
                shapePath.LineTo(100, 10);
                shapePath.LineTo(100, 50);
                shapePath.LineTo(10, 50);
                shapePath.Close();

                // Visa det aktuella HeightPixel‑värdet
                Console.WriteLine("Initial HeightPixel value: " + shapePath.HeightPixel);

                // Ange ett nytt höjdvärde
                shapePath.HeightPixel = 200;
                Console.WriteLine("Updated HeightPixel value: " + shapePath.HeightPixel);

                // Lägg till formen i kalkylbladet
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                // Spara arbetsboken
                workbook.Save("HeightPixelDemo.xlsx");
                Console.WriteLine("HeightPixel property demonstrated successfully.");
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

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


