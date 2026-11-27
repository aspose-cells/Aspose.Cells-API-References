---
title: "CellsColor-metod. Ange nyansen för formens färg"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Hämta formens fyllningsfärg"
type: docs
url: /sv/net/aspose.cells/cellscolor/settintofshapecolor/
---
## CellsColor.SetTintOfShapeColor method

Ställ in nyansen för formens färg

```csharp
public void SetTintOfShapeColor(double tint)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyans | Double |  |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class CellsColorMethodSetTintOfShapeColorWithDoubleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en form i kalkylbladet
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);

            try
            {
                // Ange färgen som ska behandlas som formfärg
                CellsColor shapeColor = shape.Fill.SolidFill.CellsColor;
                
                // Ange nyansen för formens färg (giltigt intervall är -1,0 till 1,0)
                shapeColor.IsShapeColor = true;
                
                // Visa effekten genom att ändra formens fyllningsfärg
                shapeColor.SetTintOfShapeColor(0.5); // Lighten the color by 50%
                
                Console.WriteLine("SetTintOfShapeColor method executed successfully with parameter 0.5");
                
                // Visa effekten genom att ändra figurens fyllningsfärg
                shape.Fill.SolidFill.Color = System.Drawing.Color.Blue;
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing SetTintOfShapeColor method: {ex.Message}");
            }
            
            // Spara resultatet
            workbook.Save("SetTintOfShapeColorWithDoubleDemo.xlsx");
        }
    }
}
```

### Se även

* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


