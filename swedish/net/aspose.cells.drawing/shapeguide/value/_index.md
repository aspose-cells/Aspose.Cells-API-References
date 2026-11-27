---
title: "ShapeGuide.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ShapeGuide property. Hämtar eller anger värdet för denna guide"
type: docs
url: /sv/net/aspose.cells.drawing/shapeguide/value/
---
## ShapeGuide.Value property

Hämtar eller anger värdet för denna guide

```csharp
public double Value { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapeGuidePropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en form som använder justeringsguider
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RightArrowCallout, 2, 0, 2, 0, 200, 150);

            
            // Åtkomst till formens samling av justeringsguider via Geometry
            ShapeGuideCollection shapeGuides = shape.Geometry.ShapeAdjustValues;

            // Lägg till nya guider i samlingen
            shapeGuides.Add("adj1", 25.5);
            shapeGuides.Add("adj2", 30);
            shapeGuides.Add("adj3", 25.5);
            shapeGuides.Add("adj4", 35);

            // Demonstrera läsning av guidevärden (Name-egenskapen är inte tillgänglig i den angivna definitionen)
            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);


            Console.WriteLine("Updated adjustment values");

            shapeGuides[0].Value = 25.5;
            shapeGuides[1].Value = 25.5;
            shapeGuides[2].Value = 25.5;
            shapeGuides[3].Value = 25.5;            

            Console.WriteLine("First guide value: " + shapeGuides[0].Value);
            Console.WriteLine("Second guide value: " + shapeGuides[1].Value);
            Console.WriteLine("third guide value: " + shapeGuides[2].Value);
            Console.WriteLine("fourth guide value: " + shapeGuides[3].Value);
            
            // Spara den modifierade arbetsboken
            workbook.Save("ShapeGuideValueDemo.xlsx");
        }
    }
}
```

### Se även

* class [ShapeGuide](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


