---
title: "Shape.GetActualBox"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape method. Hämta den faktiska positionen och storleken på shape efter att rotation, spegling etc. har tillämpats"
type: docs
url: /sv/net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

Hämta den faktiska positionen och storleken på formen (efter att rotation, vändning etc. har tillämpats).

```csharp
public float[] GetActualBox()
```

### Returvärde

Returnerar positionen och storleken i ordningen x, y, w, h

### Anmärkningar

Obs: Gränssnittet är inte fullt funktionellt, särskilt är positionsinformationen inte korrekt. Det rekommenderas att inte använda detta gränssnitt förrän funktionen är klar.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodGetActualBoxDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangelform
            Shape rectangle = worksheet.Shapes.AddRectangle(10, 10, 100, 80, 0, 0);

            // Hämta de faktiska lådimåtten för formen
            float[] box = rectangle.GetActualBox();

            // Skriv ut lådimåtten
            Console.WriteLine("Actual Box Dimensions:");
            Console.WriteLine($"Left: {box[0]}");
            Console.WriteLine($"Top: {box[1]}");
            Console.WriteLine($"Right: {box[2]}");
            Console.WriteLine($"Bottom: {box[3]}");

            // Spara arbetsboken
            workbook.Save("ShapeGetActualBoxDemo.xlsx");
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


