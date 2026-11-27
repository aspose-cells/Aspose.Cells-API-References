---
title: "ShapePath.MoveTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath‑metod. Startar en ny figur från den angivna punkten utan att stänga den aktuella figuren. Alla efterföljande punkter som läggs till i banan läggs till i denna nya figur. Enhet Pixel"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/moveto/
---
## ShapePath.MoveTo method

Startar en ny figur från den angivna punkten utan att stänga den aktuella figuren. Alla efterföljande punkter som läggs till i banan läggs till i denna nya figur.Enhet: Pixel.

```csharp
public void MoveTo(float x, float y)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| x | Single | X‑koordinaten för startpunkten i figuren (Enhet: Pixel). |
| y | Single | Y‑koordinaten för startpunkten i figuren (Enhet: Pixel). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodMoveToWithSingleSingleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                //Skapa en ny formbana
                ShapePath shapePath = new ShapePath();

                // Flytta till startpunkten
                shapePath.MoveTo(10, 10);

                // Anropa LineTo metod med (Single, Single) parametrar
                shapePath.LineTo(50.5f, 10.5f);
                shapePath.LineTo(50.5f, 50.5f);
                shapePath.LineTo(10.5f, 50.5f);
                shapePath.Close();

                //lägg till fri form
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("MoveTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
           
            
            // Spara resultatet
            workbook.Save("ShapePathMethodMoveToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


