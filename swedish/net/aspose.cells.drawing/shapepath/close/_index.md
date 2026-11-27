---
title: "ShapePath.Close"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapePath‑metod. Stänger den aktuella figuren och startar en ny figur. Om den aktuella figuren innehåller en sekvens av sammanhängande linjer och kurvor stänger metoden loopen genom att ansluta en linje från slutpunkten till startpunkten."
type: docs
url: /sv/net/aspose.cells.drawing/shapepath/close/
---
## ShapePath.Close method

Stänger den aktuella figuren och startar en ny figur. Om den aktuella figuren innehåller en sekvens av sammanhängande linjer och kurvor, stänger metoden loopen genom att ansluta en linje från slutpunkten till startpunkten.

```csharp
public void Close()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathMethodCloseDemo
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
                shapePath.MoveTo(60, 45);
                shapePath.ArcTo(25, 25, 0, 270);

                // Stäng banan 
                shapePath.Close();

                shapePath.MoveTo(60, 20);
                shapePath.LineTo(110, 70);
                shapePath.LineTo(125, 155.5f);
                shapePath.ArcTo(35.5f, 35.5f, 0, 270);

                // Stäng banan 
                shapePath.Close();

                //lägg till fri form
                worksheet.Shapes.AddFreeform(1, 0, 1, 0, 300, 200, new ShapePath[] { shapePath });

                Console.WriteLine("Close method called successfully to complete the shape path");
                
                // Spara arbetsboken
                workbook.Save("ShapePathMethodCloseDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling Close method: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [ShapePath](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


