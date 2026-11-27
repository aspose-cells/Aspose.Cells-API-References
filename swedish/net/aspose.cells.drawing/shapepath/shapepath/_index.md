---
title: "ShapePath.ShapePath"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath-konstruktor. Initierar en ny instans av ShapePath-klassen"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/shapepath/
---
## ShapePath constructor

Initierar en ny instans av [`ShapePath`](../)-klassen.

```csharp
public ShapePath()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCtorDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Skapa en ny formväg med hjälp av #ctor-metoden
                ShapePath shapePath = new ShapePath();

                // Lägg till vägssegment för att skapa en enkel form
                shapePath.MoveTo(100, 100);
                shapePath.LineTo(200, 100);
                shapePath.LineTo(200, 200);
                shapePath.LineTo(100, 200);
                shapePath.Close();

                //lägg till fri form
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 200, 200, new ShapePath[] { shapePath });

                Console.WriteLine("ShapePath created and added to worksheet successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ShapePath constructor: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("ShapePathMethodCtorDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


