---
title: "Shape.SoftEdges"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger radien för suddighet som ska tillämpas på kanterna i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing/shape/softedges/
---
## Shape.SoftEdges property

Hämtar och anger radien för oskärpa som ska tillämpas på kanterna, i enheten punkter.

```csharp
public double SoftEdges { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertySoftEdgesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform med korrekta parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 0);

            // Ställ in mjuka kanter-effekt med radie på 5 punkter (0.5d = 5 punkter)
            shape.SoftEdges = 0.5d;

            // Spara arbetsboken
            workbook.Save("SoftEdgesDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


