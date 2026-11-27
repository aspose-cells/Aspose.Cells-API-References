---
title: "Shape.IsInGroup"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Anger om formen är grupperad"
type: docs
url: /sv/net/aspose.cells.drawing/shape/isingroup/
---
## Shape.IsInGroup property

Anger om formen är grupperad.

```csharp
public bool IsInGroup { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePropertyIsInGroupDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till några former med alla nödvändiga parametrar (upperLeftRow, upperLeftColumn, height, width, imageWidth, imageHeight)
            Shape shape1 = worksheet.Shapes.AddRectangle(2, 0, 2, 0, 50, 100);
            Shape shape2 = worksheet.Shapes.AddRectangle(6, 0, 2, 0, 50, 100);
            Shape shape3 = worksheet.Shapes.AddRectangle(3, 0, 5, 0, 50, 100);

            // Gruppera formerna med korrekta parametrar
            GroupShape group = worksheet.Shapes.Group(new Shape[] { shape1, shape2, shape3 });

            // Kontrollera om formerna är i en grupp
            Console.WriteLine("Shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("Shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("Shape3 IsInGroup: " + shape3.IsInGroup);
            Console.WriteLine("GroupShape IsInGroup: " + group.IsInGroup);

            // Lägg till en icke-grupperad form
            Shape ungroupedShape = worksheet.Shapes.AddRectangle(10, 0, 2, 0, 50, 100);
            Console.WriteLine("Ungrouped shape IsInGroup: " + ungroupedShape.IsInGroup);

            // Spara resultatet
            workbook.Save("ShapePropertyIsInGroupDemo.xlsx");

            // Avgruppera formerna och hämta de avgrupperade formerna från gruppen
            group.Ungroup();
            Console.WriteLine("After ungrouping, shape1 IsInGroup: " + shape1.IsInGroup);
            Console.WriteLine("After ungrouping, shape2 IsInGroup: " + shape2.IsInGroup);
            Console.WriteLine("After ungrouping, shape3 IsInGroup: " + shape3.IsInGroup);

            // Spara resultatet
            workbook.Save("ShapePropertyIsInGroupDemo2.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


