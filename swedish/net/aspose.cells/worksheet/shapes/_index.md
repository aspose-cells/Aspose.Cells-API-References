---
title: "Worksheet.Shapes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet-egenskap. Returnerar alla ritningsformer i detta kalkylblad"
type: docs
url: /sv/net/aspose.cells/worksheet/shapes/
---
## Worksheet.Shapes property

Returnerar alla ritningsformer i detta arbetsblad.

```csharp
public ShapeCollection Shapes { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyShapesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Lägg till några former i kalkylbladet
            sheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            sheet.Shapes.AddLine(2, 0, 100, 100, 100, 1);
            
            // Ändra formegenskaper
            for (int i = 0; i < sheet.Shapes.Count; i++)
            {
                Aspose.Cells.Drawing.Shape shape = sheet.Shapes[i];
                Console.WriteLine($"Shape {i}: Type={shape.Type}, Name={shape.Name}");
                
                // Uppdatera egenskaper för den första formen
                if (i == 0)
                {
                    shape.Name = "MyRectangle";
                    shape.FillFormat.ForeColor = System.Drawing.Color.Red;
                }
            }
            
            // Spara arbetsboken
            workbook.Save("ShapesDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeCollection](../../../aspose.cells.drawing/shapecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


