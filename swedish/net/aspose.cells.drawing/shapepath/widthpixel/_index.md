---
title: "ShapePath.WidthPixel"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath egenskap. Hämtar bredden på den här banan i enhet pixlar"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/widthpixel/
---
## ShapePath.WidthPixel property

Hämtar bredden på denna bana i enhet pixlar.

```csharp
public int WidthPixel { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPropertyWidthPixelDemo
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

                // Visa det initiala WidthPixel‑värdet
                Console.WriteLine("Initial WidthPixel value: " + shapePath.WidthPixel);

                // Ange ett nytt breddvärde
                shapePath.WidthPixel = 300;
                Console.WriteLine("Updated WidthPixel value: " + shapePath.WidthPixel);

                // Lägg till formen i kalkylbladet
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, shapePath.WidthPixel, 200, new ShapePath[] { shapePath });

                // Spara arbetsboken
                workbook.Save("WidthPixelDemo.xlsx");
                Console.WriteLine("WidthPixel property demonstrated successfully.");
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


