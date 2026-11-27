---
title: "Klass ShapeGuide"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapeGuide-klass. Inkapslar en formguide som specificerar närvaron av en formguide som kommer att användas för att styra geometrin för den angivna formen"
type: docs
url: /sv/net/aspose.cells.drawing/shapeguide/
---
## ShapeGuide class

Inkapslar en formguide som specificerar närvaron av en formguide som kommer att användas för att styra geometrin för den angivna formen

```csharp
public class ShapeGuide : BaseShapeGuide
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Value](../../aspose.cells.drawing/shapeguide/value/) { get; set; } | Hämtar eller anger värdet för denna guide |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapeGuideDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                var shape = worksheet.Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 100, 100, 100, 100);
                
                // Skapa och lägg till formguide med nödvändiga parametrar
                int guideIndex = shape.Geometry.ShapeAdjustValues.Add("Guide1", 0.2);
                ShapeGuide guide = shape.Geometry.ShapeAdjustValues[guideIndex];
                
                Console.WriteLine($"ShapeGuide created with Value: {guide.Value}");
                
                workbook.Save("DrawingClassShapeGuideDemo.xlsx");
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

* class [BaseShapeGuide](../baseshapeguide/)
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


