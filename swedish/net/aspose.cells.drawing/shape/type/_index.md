---
title: "Shape.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar den automatiska formtypen"
type: docs
url: /sv/net/aspose.cells.drawing/shape/type/
---
## Shape.Type property

Hämtar auto‑formstypen.

```csharp
public AutoShapeType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddAutoShape(AutoShapeType.Rectangle, 1, 1, 100, 150, 0, 0);

            // Hämta och visa formtypen
            AutoShapeType autoShapeType = shape.Type;
            Console.WriteLine("Shape Type: " + autoShapeType);

            // Kan inte ändra formtypen eftersom Type-egenskapen är skrivskyddad
            // Skapa istället en ny form med annan typ
            Shape ovalShape = worksheet.Shapes.AddAutoShape(AutoShapeType.Oval, 1, 1, 100, 150, 0, 0);
            Console.WriteLine("New Shape Type: " + ovalShape.Type);
        }
    }
}
```

### Se även

* enum [AutoShapeType](../../autoshapetype/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


