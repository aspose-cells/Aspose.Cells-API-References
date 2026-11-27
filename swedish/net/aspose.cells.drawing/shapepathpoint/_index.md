---
title: "Klass ShapePathPoint"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapePathPoint-klass. Ange positionskoordinater eller vinkelmarkörer. Positionskoordinater representerar koordinaterna för en bana i ett koordinatrum, t.ex. X/Y. Vinkelmarkörer indikerar vinkeländringar i en bana, t.ex. start- och svängvinklarna för en båge"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpoint/
---
## ShapePathPoint class

Specificera positionskoordinater eller vinkelmarkörer. Positionskoordinater representerar koordinaterna för en väg i ett koordinatrum (t.ex. X/Y). Vinkelmarkörer indikerar vinkeländringar i en väg (t.ex. start- och svängvinklarna för en båge).

```csharp
public class ShapePathPoint
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Type](../../aspose.cells.drawing/shapepathpoint/type/) { get; } | Anger värdetypen för det aktuella objektet. |
| [X](../../aspose.cells.drawing/shapepathpoint/x/) { get; set; } | (**Obsolete.**) Hämtar och anger x‑koordinaten för denna positionskoordinat. Enhet EMUs. |
| [XAngle](../../aspose.cells.drawing/shapepathpoint/xangle/) { get; set; } | När objektet är en vinkelmarkör, hämta eller ange den första vinkeln i grader. |
| [XPixel](../../aspose.cells.drawing/shapepathpoint/xpixel/) { get; set; } | När objektet är en positionskoordinat, hämta eller ange x‑koordinaten i pixlar. |
| [Y](../../aspose.cells.drawing/shapepathpoint/y/) { get; set; } | (**Obsolete.**) Hämtar y‑koordinaten för denna positionskoordinat. Enhet EMUs. |
| [YAngle](../../aspose.cells.drawing/shapepathpoint/yangle/) { get; set; } | När objektet är en vinkelmarkör, hämta eller ange den andra vinkeln i grader. |
| [YPixel](../../aspose.cells.drawing/shapepathpoint/ypixel/) { get; set; } | När objektet är en positionskoordinat, hämta eller ange y‑koordinaten i pixlar. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            try
            {
                // Lägg till en form som kommer att innehålla banpunkter med alla nödvändiga parametrar
                Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 10, 10, 200, 200);
                
                // Hämta geometribana‑punkterna
                CustomGeometry geometry = shape.Geometry as CustomGeometry;
                if (geometry != null && geometry.Paths.Count > 0)
                {
                    ShapePath path = geometry.Paths[0];
                    
                    // Åtkomst till en befintlig banpunkt (om tillgänglig)
                    if (path.PathSegementList.Count > 0)
                    {
                        // Hämta den första punkten (den faktiska implementeringen kan variera beroende på segmenttyp)
                        ShapePathPoint point = path.PathSegementList[0].Points[0];
                        
                        // Visa punktkoordinaterna
                        Console.WriteLine($"ShapePathPoint at X: {point.X}, Y: {point.Y}");
                    }
                }
                
                // Spara arbetsboken
                workbook.Save("ShapePathPointDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPoint: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


