---
title: "ShapePath.LineTo"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath-metod. Lägger till ett linjesegment till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren. Enhet Pixel"
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/lineto/
---
## ShapePath.LineTo method

Lägger till ett linjesegment till den aktuella figuren. Startpunkten är slutpunkten för den aktuella figuren.Enhet: Pixel.

```csharp
public void LineTo(float x, float y)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| x | Single | X-koordinaten för slutpunkten av linjesegmentet (Enhet: Pixel). |
| y | Single | Y-koordinaten för slutpunkten av linjesegmentet (Enhet: Pixel). |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodLineToWithSingleSingleDemo
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

                Console.WriteLine("LineTo method executed successfully with parameters (Single, Single)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing LineTo method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("ShapePathMethodLineToWithSingleSingleDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


